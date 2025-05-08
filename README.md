# TDA Comparison: Clustering vs. Persistent Homology vs. KeplerMapper

This repository contains a Python script (`tda_comparison.py`) that demonstrates and compares different data analysis techniques on a synthetically generated "noisy circle" dataset. The goal is to illustrate how Topological Data Analysis (TDA) methods can reveal underlying structural features that traditional methods might miss.

## Techniques Explored:

1.  **K-Means Clustering:** A standard partitioning clustering algorithm.
2.  **Persistent Homology (via `giotto-tda`):** Computes a persistence diagram to quantify topological features like connected components (H0) and loops/holes (H1).
3.  **KeplerMapper:** Constructs a graph-based (simplicial complex) representation of the data, providing a visual summary of its shape and connectivity.

## Features:

*   Generates a 2D noisy circle dataset.
*   Applies K-Means clustering and visualizes the results.
*   Computes and visualizes a persistence diagram.
*   Constructs and visualizes a KeplerMapper graph (outputs an interactive HTML file).
*   Provides clear Matplotlib visualizations and console output for interpretation.
*   Well-commented and structured Python code.

## How to Run:

1.  **Clone the repository:**
    ```bash
    git clone <your-repo-url>
    cd <your-repo-name>
    ```

2.  **Install dependencies:**
    Ensure you have Python 3 installed. Then, install the required libraries:
    ```bash
    pip install numpy matplotlib scikit-learn giotto-tda kmapper
    ```
    *(You might want to use a virtual environment for this.)*

3.  **Run the script:**
    ```bash
    python tda_comparison.py
    ```

4.  **View Outputs:**
    *   Console output will provide summaries and insights.
    *   Matplotlib plots will display K-Means results and the persistence diagram.
    *   An HTML file (default: `kepler_mapper_noisy_circle.html`) will be generated for the interactive KeplerMapper graph. This file will attempt to open in your default web browser.

## Expected Outcome:

The script aims to show:
*   How K-Means might segment the circle based on local density.
*   How the persistence diagram clearly identifies the single significant loop (H1 feature) of the circle.
*   How the KeplerMapper graph visually represents this circular structure as a looped graph.

This comparison highlights the strengths of TDA in capturing global topological characteristics of data.

---


