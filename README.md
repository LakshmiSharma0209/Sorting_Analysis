# Sorting Algorithm Performance Analysis

This repository contains a Python script that analyzes and compares the performance of several common sorting algorithms: **Insertion Sort**, **Merge Sort**, **Bubble Sort**, and Python's built-in **Timsort**. The goal is to provide a practical demonstration of the difference between **O(n²)** and **O(n log n)** time complexity, a fundamental concept in algorithm analysis.

The script generates random arrays of increasing sizes, measures the time each algorithm takes to sort them, and visualizes the results. This helps to illustrate how the choice of algorithm can dramatically impact performance as the input size grows.

## Features

- **Implementation of Sorting Algorithms**:
  - `insertion_sort` (O(n²))
  - `merge_sort` (O(n log n))
  - `bubble_sort` (O(n²))
  - `python_timsort` (Python's built-in `sorted()`, O(n log n))
- **Performance Measurement**: The `measure_sorting_time` function accurately records the execution time for each algorithm on various array sizes.
- **Data Generation**: The `generate_random_array` function creates test data for the experiment.
- **Data Analysis**: A pandas DataFrame is used to store and analyze the average execution times from multiple trials.
- **Visualizations**: Matplotlib is used to generate plots that visually compare the performance of the algorithms on different scales (linear and log-log).
- **Detailed Report**: The script prints a summary table and a detailed analysis of the results, including key observations and insights into algorithmic complexity.
- **CSV Output**: The experimental results are saved to a CSV file (`sorting_algorithm_results.csv`) for further analysis.

## Time Complexity Explained

- **O(n²)** (e.g., Insertion Sort, Bubble Sort): These algorithms have a quadratic relationship with the input size. If you double the number of elements, the execution time will increase by a factor of roughly four. This makes them inefficient for large datasets.
- **O(n log n)** (e.g., Merge Sort, Timsort): These algorithms have a much more efficient growth rate. As the input size increases, their performance scales much better, making them suitable for large-scale data processing.

## Usage

### Prerequisites

- Python 3.x
- `pandas` library (`pip install pandas`)
- `matplotlib` library (`pip install matplotlib`)
- `numpy` library (`pip install numpy`)

### Running the Script

1. Clone or download this repository.
2. Navigate to the directory containing the script.
3. Run the script from your terminal:

   ```bash
   python sorting_analyzer.py
