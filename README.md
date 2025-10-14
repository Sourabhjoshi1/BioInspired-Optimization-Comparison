# Comparative Study of Bio-Inspired Optimization Algorithm

## 🚀 Project Overview

This project conducts a comprehensive comparative analysis of three fundamental metaheuristic optimization algorithms—**Genetic Algorithm (GA)**, **Differential Evolution (DE)**, and **Simulated Annealing (SA)**—on a set of standard mathematical benchmark functions. The analysis evaluates each algorithm's performance, robustness, and efficiency in finding the global minimum for both unimodal and multimodal search spaces.

The entire comparison is implemented in a single Python script designed for easy execution in a Google Colaboratory environment.

---

## 🛠️ Algorithms and Inspiration

| Algorithm | Type | Core Inspiration | Key Optimization Process |
| :--- | :--- | :--- | :--- |
| **Genetic Algorithm (GA)** | Evolutionary | Natural Selection and Genetics | Selection, Crossover, and Mutation. |
| **Differential Evolution (DE)** | Evolutionary | Genetic Variation and Population-based Search | Mutation via vector difference, Crossover, and Selection. |
| **Simulated Annealing (SA)** | Metaheuristic | Annealing in Metallurgy | Probabilistic acceptance of worse solutions to escape local optima. |

---

## 📐 Benchmark Functions

The algorithms are tested on two classic continuous optimization problems to assess their behavior in different search space topologies:

| Function | Type | Characteristics | Key Test |
| :--- | :--- | :--- | :--- |
| **Sphere Function** | **Unimodal** | Simple, smooth, convex, with a single global minimum at $f(x)=0$. | **Exploitation Ability** (Convergence speed and precision). |
| **Rastrigin Function** | **Multimodal** | Highly complex, many regularly distributed local minima surrounding the global minimum at $f(x)=0$. | **Exploration Ability** (Capacity to avoid local traps). |

---

## 💻 How to Run the Project

### Prerequisites

The script requires the `deap` library, which is installed automatically within the Colab environment.

### Execution Steps

1.  **Create a New Colab Notebook:** Open Google Colaboratory and create a new Python notebook.
2.  **Paste the Code:** Copy and paste the entire Python script into the first code cell.
3.  **Run:** Execute the cell (Shift + Enter).

The script will automatically install dependencies, run the experiments, calculate the statistics over multiple runs, and generate performance charts.

### Experiment Configuration

The core comparison uses the following parameters:

| Parameter | Value | Metric |
| :--- | :--- | :--- |
| **Dimensionality ($D$)** | 10 | Number of variables (search space size). |
| **Max Iterations** | 100 | Maximum generations/steps. |
| **Population Size**| 20 | Number of search agents per algorithm. |
| **Number of Runs** | 10 | Independent repetitions to ensure statistically robust averages. |

---

## 📊 Results Analysis

The comparative performance is judged using the following key metrics, summarized in the output table and charts:

| Metric | Goal | Interpretation |
| :--- | :--- | :--- |
| **Avg. Final Value** | **Minimize** (closer to 0.0) | The average quality of the solution found. |
| **Std. Final Value** | **Minimize** | Measures the **Robustness** and consistency of the algorithm across multiple runs. |
| **Avg. Runtime (s)** | Minimize | Wall-clock time taken for execution. |
| **Avg. NFEV** | Minimize | **Number of Function Evaluations** (computational cost). |

The generated plots visually compare the algorithms' performance (Avg. Final Value on a log scale) and efficiency (Avg. Runtime) for both benchmark functions.




📧 Contact
Sourabh Joshi
Project Link: https://github.com/sourabhjoshi01/BioInspired-Optimization-Comparison

python run_comparison.py
