import javax.swing.*;
import java.awt.*;
import java.util.ArrayList;

/**
 * Koch Snowflake is drawn using recursive calls to collect all end points of
 * snowflake and draw lines between them. Distance is computed using a
 * recursive formula.
 *
 * Author: Ievgen O. Borovenskyi & Nick Enbar-Salo
 * Version: 04.02.25
 */
public class SnowFlake extends JPanel {

    /**
     * The size of the window where image is drawn.
     */
    public static final int PANEL_SIZE = 600;

    /**
     * Recursion level for the snowflake.
     */
    private final int level;

    /**
     * Side length of the base triangle.
     */
    private final int length;

    /**
     * X-coordinate of the bottom-left corner of the triangle.
     */
    private final int initialX;

    /**
     * Y-coordinate of the bottom-left corner of the triangle.
     */
    private final int initialY;

    /**
     * Represents a 2D point with integer coordinates.
     */
    static class Point {

        /**
         * Represents an x coordinates of a starting point.
         */
        private int x;

        /**
         * Represents an y coordinates of a starting point.
         */
        private int y;

        /**
         * Creates an object for a point for given x and y coordinates.
         *
         * @param x the x-coordinate
         * @param y the y-coordinate
         */
        Point(int x, int y) {
            this.x = x;
            this.y = y;
        }
        @Override
        public String toString() {
            return "(" + x + ", " + y + ")";
        }

    }

    /**
     * Constructs a Koch Snowflake object with given parameters.
     *
     * @param level recursion depth
     * @param length side length of triangle
     * @param x bottom-left x coordinate
     * @param y bottom-left y coordinate
     */
    public SnowFlake(int level, int length, int x, int y) {
        this.level = level;
        this.length = length;
        this.initialX = x;
        this.initialY = y;
    }

    /**
     * The main function of the class that is responsible for building the
     * snowflake, drawing it, and printing total perimeter.
     *
     * @param g the Graphics context used for drawing
     */
    @Override
    protected void paintComponent(Graphics g) {
        super.paintComponent(g);
        Graphics2D g2 = (Graphics2D) g;

        // build base triangle points using unit-circle trigonometry
        // finds height using sin(pi/3)
        int height = (int) (Math.sqrt(3) / 2 * length);
        // left most point of triangle
        Point a = new Point(initialX, initialY);
        // right most point of triangle
        Point b = new Point(initialX + length, initialY);
        // top point of triangle
        // finds point c which is the point between point a & b using cos(pi/3)
        Point c = new Point(initialX + length / 2, initialY - height);

        // recursively draw all 3 sides
        ArrayList<Point> snowflake = new ArrayList<>();
        drawSnowflakeSide(g2, a, b, level, snowflake);
        drawSnowflakeSide(g2, b, c, level, snowflake);
        drawSnowflakeSide(g2, c, a, level, snowflake);

        System.out.println("All collected points:");
        for (Point p : snowflake) {
            System.out.println(p);
        }

        // compute and print total length
        double total = kochLength(level, length);
        System.out.printf("Total length: (level " + level + "): " + total);
    }

    /**
     * Recursively calculates the total length of the snowflake's edges.
     *
     * @param level recursion depth
     * @param length side length of triangle
     * @return total edge length of the snowflake
     */
    public double kochLength(int level, int length) {
       // base case: returns perimeter of level 0 snowflake
        if (level == 0) {
            return 3 * length;
        }
        //return perimeter's of snowflakes with levels > 0
        return 4.0 / 3.0 * kochLength(level - 1, length);
    }

    /**
     * Recursively draws a snowflake side between two points.
     *
     * @param g graphics context
     * @param a starting point
     * @param b ending point
     * @param level recursion depth
     * @param result list to store resulting points
     */
    private void drawSnowflakeSide(Graphics g, Point a, Point b, int level, ArrayList<Point> result) {
        if (level == 0) {
            g.drawLine(a.x, a.y, b.x, b.y);
            result.add(a);
        } else {
            Point p1 = linearInterpolation(a, b, 1.0 / 3);
            Point p2 = linearInterpolation(a, b, 2.0 / 3);
            Point peak = peakEdge(p1, p2);

            drawSnowflakeSide(g, a, p1, level - 1, result);
            drawSnowflakeSide(g, p1, peak, level - 1, result);
            drawSnowflakeSide(g, peak, p2, level - 1, result);
            drawSnowflakeSide(g, p2, b, level - 1, result);
        }
    }

    /**
     * Returns a point located between two specific points based on the level
     * that is currently affecting the snowflake.
     *
     * @param a first point
     * @param b second point
     * @param currentFraction fraction along the line from a to b (0.0 to 1.0)
     * @return the interpolated point between a and b
     */
    private Point linearInterpolation(Point a, Point b,
                                      double currentFraction) {
        int x = (int) (a.x + currentFraction * (b.x - a.x));
        int y = (int) (a.y + currentFraction * (b.y - a.y));
        return new Point(x, y);
    }

    /**
     * Builds the Point object for a peak point of an equilateral triangle
     * between the two points of the base a and b.
     *
     * @param a first point
     * @param b second point
     * @return the triangle's peak above segment a–b
     */
    private Point peakEdge(Point a, Point b) {
        // change in x; final x minus intial x coordinate
        double dx = b.x - a.x;
        // change in y; final y minus intial y coordinate
        double dy = b.y - a.y;
        // angle = 60 degrees
        double angle = Math.PI / 3;
        // new x coord for peak between base triangle's bottom points
        int px = (int) (dx * Math.cos(angle) - dy * Math.sin(angle));
        // new y coord for peak between base triangle's bottom points
        int py = (int) (dx * Math.sin(angle) + dy * Math.cos(angle));
        // create new Point object for peak edge of the triangle in snow flake
        return new Point(a.x + px, a.y + py);
    }

    /**
     * The Main function of the class that launches the specific level of
     * Koch Snow flake to be built. With manual tweaking of the parameters.
     *
     * @param args command-line arguments N/A
     */
    public static void main(String[] args) {
        // number of recursive levels
        int level = 3;
        // side length of triangle
        int length = 100;
        // starting x position
        int initialX = 100;
        // starting y position
        int initialY = 400;

        // create a window titled "Koch Snowflake"
        JFrame frame = new JFrame("Koch Snowflake");

        // program will exit/quit when window (specified above) is closed
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);

        // create a SnowFlake drawing panel
        SnowFlake panel = new SnowFlake(level, length, initialX, initialY);

        // window will display the snowflake computed
        frame.setContentPane(panel);

        // set the size of the window to equal constant PANEL_SIZE
        frame.setSize(PANEL_SIZE, PANEL_SIZE);

        // show the final drawn snowFlake
        frame.setVisible(true);
    }
}
