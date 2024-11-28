# Sorting in Python

This repository contains examples and explanations of various sorting algorithms and techniques in Python.  Python offers efficient built-in methods as well as the possibility of implementing custom algorithms. This README provides an overview and links to specific examples.


## Contents

* **Built-in Sorting:**  Demonstrates the use of `sorted()` and `list.sort()`, including examples of customized sorting using `key` functions.
* **Custom Algorithms:**  Includes implementations of common sorting algorithms like:
    * Bubble Sort
    * Insertion Sort
    * Selection Sort
    * Merge Sort
    * Quick Sort
* **Performance Comparisons:**  (Future addition)  A comparison of the runtime performance of different algorithms with varying data sizes.
* **Use Cases:** (Future addition) Examples showcasing practical applications of different sorting methods.


## Built-in Sorting (`sorted()` and `list.sort()`)

Python's built-in `sorted()` function and `list.sort()` method are highly optimized and generally the preferred approach for most sorting tasks. `sorted()` returns a new sorted list, while `list.sort()` sorts the list in-place.  Both accept a `key` argument for customized sorting:


```python
# Example using sorted()
my_list = [3, 1, 4, 1, 5, 9, 2, 6]
sorted_list = sorted(my_list)
print(f"Original: {my_list}, Sorted: {sorted_list}")

# Example using list.sort() (in-place sorting)
my_list.sort()
print(f"In-place sorted: {my_list}")

# Example with custom key (sorting strings by length)
strings = ["apple", "banana", "kiwi"]
sorted_strings = sorted(strings, key=len)
print(f"Sorted by length: {sorted_strings}")
