---
layout: project
type: project
image: img/KochSnowflake.png
title: "Optimization of Drawing Koch Snowflakes Using Trigonetry & Linear Algebra"
date: 04-02-2025
published: true
labels:
  - Java
  - Data Structure & Algorithms
  - Optimization & Mathematical Approch
summary: "This Java program uses recursion and Swing graphics to draw a Koch Snowflake fractal, collect and print its points, and compute the total perimeter length at a given recursion depth."
---

<img class="img-fluid" src="../img/cotton/cotton-header.png">


# Koch Snowflake Fractal in Java

This project implements a **Koch Snowflake fractal** in Java using recursion and the Swing graphics library. The program begins with an equilateral triangle and recursively subdivides each side, replacing the middle third with two new segments that form a peak, creating the classic snowflake shape. At each recursion level, the fractal becomes more detailed, and the program both draws the resulting figure and computes its total perimeter using a recursive formula. The implementation also prints all generated points for verification and visualization purposes.  

The program is structured for clarity and efficiency. Core functionality is divided into modular helper methods: `linearInterpolation` calculates intermediate points, `peakEdge` computes the triangular peaks with trigonometry, and `drawSnowflakeSide` applies the recursive subdivision logic. By separating these concerns, the recursion directly mirrors the mathematical definition of the Koch curve, making the code easy to read, debug, and extend. Additionally, the perimeter calculation leverages a direct recursive formula rather than summing individual segments, which greatly reduces computational overhead. The use of lightweight objects (`Point`) and efficient Java 2D graphics operations ensures smooth rendering.  

In terms of computational performance, the algorithm generates `3 × 4^n` line segments at recursion depth *n*, giving it a time complexity of **O(4^n)**. While exponential, this complexity is intrinsic to the fractal’s recursive definition, and the program is optimized to handle practical recursion depths (up to 6–7 levels) without performance issues. By combining mathematical elegance with efficient recursion and modular design, this project demonstrates both the power of fractals in computer graphics and effective recursive programming techniques in Java.  
