# 2MP3 Assignment 2 - Sorting Algorithms in C

**Author:** Garret Langlois  
**Date:** October 2024

## Introduction

This repository contains the implementation of five different sorting algorithms in C for Assignment 2 of the MECHTRON 2MP3 course at McMaster University. Sorting algorithms are essential in many computing systems, and this assignment focuses on their implementation and performance analysis. The five algorithms implemented are:

- **Bubble Sort**
- **Insertion Sort**
- **Merge Sort**
- **Heap Sort**
- **Counting Sort**

### File Structure

- **`main.c`**: Contains test arrays and function calls for all sorting algorithms.
- **`mySort.h`**: Header file with function prototypes.
- **`mySort.c`**: Contains the implementation of the sorting algorithms.
- **`timing_script.py`**: Python script for timing the sorting algorithms and comparing them with Python’s built-in sorting methods.

## Problem Statement

You are required to implement the following sorting algorithms from scratch in C:
- **Bubble Sort** (already provided)
- **Insertion Sort**
- **Merge Sort**
- **Heap Sort**
- **Counting Sort**

The main goal is to ensure the correct implementation and analyze the performance of each algorithm by measuring time and space complexity.

## Solution Overview

Each algorithm has been implemented in the `mySort.c` file. Below is a brief description of each:

1. **Bubble Sort**: A simple sorting algorithm that repeatedly steps through the list, compares adjacent elements, and swaps them if they are in the wrong order.
2. **Insertion Sort**: Builds the final sorted array one item at a time, placing each unsorted item in its correct position.
3. **Merge Sort**: A divide-and-conquer algorithm that recursively splits the array into smaller subarrays and merges them back together in a sorted order.
4. **Heap Sort**: Utilizes a binary heap structure to sort the array by repeatedly removing the largest element from the heap and rebuilding it.
5. **Counting Sort**: An integer-based algorithm that counts occurrences of each value to determine the position of each element in the sorted output.

## Performance Case Study

A Python script is included to measure the performance (in CPU time) of each sorting algorithm, using a large array of random numbers. The script also compares the implemented algorithms with Python's built-in sorting methods. Below is a summary of the performance:

| Sort Method       | Time Complexity | Space Complexity | CPU Time (Seconds) |
|-------------------|-----------------|------------------|--------------------|
| Bubble Sort       | O(n²)           | O(1)             | 645.14             |
| Insertion Sort    | O(n²)           | O(1)             | 85.07              |
| Merge Sort        | O(n log n)      | O(n)             | 0.11               |
| Heap Sort         | O(n log n)      | O(1)             | 0.11               |
| Counting Sort     | O(n + k)        | O(k)             | 0.014              |
| Python `sorted()` | O(n log n)      | O(n)             | 0.21               |
| NumPy `sort()`    | O(n log n)      | O(n)             | 0.0029             |

## Instructions for Running the Code

### C Implementation
1. Compile the code by running the following command:
   ```bash
   gcc -o sorting_program main.c mySort.c
