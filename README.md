# Experiment 20 - Searching Techniques (Linear, Sequential, and Binary Search)

- **Name:** Harshil Nagori
- **Class:** ENTC A2
- **PRN:** 24070123046  
- **Title:** Implementation of Linear, Sequential, and Binary Search in C++  

---

## Aim
To implement and compare **Linear Search, Sequential Search, and Binary Search** techniques using C++ and analyze their efficiency.

---

## Objectives
1. To study and understand different searching techniques.  
2. To implement **Sequential Search** (basic linear approach).  
3. To implement **Linear Search** (unsorted array search).  
4. To implement **Binary Search** (sorted array search using divide and conquer).  
5. To compare the performance of all three searching techniques.  
6. To develop clarity on the choice of searching algorithm based on dataset type and size.  

---

## Theory

### Searching
Searching is the process of finding whether an element (key) exists in a dataset and, if so, determining its position. Efficient searching is vital in databases, operating systems, and real-time applications.

---

### 1. Sequential Search
- Simplest searching method.  
- Scans each element one by one from the beginning until the key is found or the array ends.  
- Works on both sorted and unsorted data.  
- **Time Complexity:**  
  - Best Case: O(1)  
  - Worst Case: O(n)  
- **Space Complexity:** O(1)  

---

### 2. Linear Search
- A practical form of **sequential search**.  
- Iterates over the array linearly and checks each element.  
- Commonly used when the dataset is **unsorted**.  
- **Time Complexity:**  
  - Best Case: O(1)  
  - Worst Case: O(n)  
- **Space Complexity:** O(1)  

---

### 3. Binary Search
- Works only on **sorted arrays**.  
- Uses **divide and conquer** approach.  
- Reduces the search interval by half each time.  
- Very efficient compared to linear and sequential search for large datasets.  
- **Time Complexity:**  
  - Best Case: O(1)  
  - Worst Case: O(log n)  
- **Space Complexity:** O(1)  

---

## Comparison Table

| Feature              | Sequential Search             | Linear Search                | Binary Search                |
|----------------------|--------------------------------|------------------------------|------------------------------|
| Data Requirement     | Sorted/Unsorted               | Sorted/Unsorted              | Sorted only                  |
| Technique            | Element-by-element scan       | Element-by-element scan      | Divide and Conquer           |
| Time Complexity      | O(n)                          | O(n)                         | O(log n)                     |
| Best Case            | O(1)                          | O(1)                         | O(1)                         |
| Worst Case           | O(n)                          | O(n)                         | O(log n)                     |
| Efficiency           | Poor for large datasets       | Poor for large datasets      | Highly efficient             |
| Use Case             | Small datasets                | Unsorted data search         | Large sorted datasets        |

---

## Concepts Used
- **Arrays:** To store input elements.  
- **Searching Algorithms:** Sequential, Linear, and Binary.  
- **Functions:** Binary search implemented with a separate function.  
- **Control Structures:** Loops (`for`, `while`) and decision-making (`if-else`).  
- **Complexity Analysis:** Understanding time/space efficiency of algorithms.  

---

## Algorithms
### 1.
### Sequential Search Program
- Takes `n` elements as input.  
- Uses a **basic loop** to check each element.  
- Returns index/position if found, else displays not found.
- 
### Algorithm for Sequential Search
1. Input the number of elements `n`.  
2. Input `n` elements into the array.  
3. Input the search key.  
4. For `i = 0` to `n-1`:  
   - If `arr[i] == key`, return position and exit.  
5. If end of array reached → element not found.  

---
### 2.

### Linear Search Program
- Similar to sequential but implemented more structurally.  
- Works on **unsorted data**.  
- Stops after finding the **first occurrence** of the key.
- 
### Algorithm for Linear Search
1. Input the number of elements `n`.  
2. Input `n` elements into the array.  
3. Input the search key.  
4. Traverse the array one by one.  
5. If element matches → return index and position.  
6. If no match found → print "Element not found".  

---
### 3.
### Binary Search Program
- Works on **sorted data only**.  
- Repeatedly divides the array in half.  
- Much faster for large datasets.
- 
### Algorithm for Binary Search
1. Input the number of elements `n`.  
2. Input `n` sorted elements into the array.  
3. Input the search key.  
4. Initialize `low = 0`, `high = n-1`.  
5. Repeat until `low <= high`:  
   - Compute `mid = (low + high) / 2`.  
   - If `arr[mid] == key` → return position.  
   - Else if `arr[mid] < key` → set `low = mid + 1`.  
   - Else → set `high = mid - 1`.  
6. If not found → print "Element not found".  

---

## Conclusion
- Sequential and Linear search are **simple but inefficient** for large datasets.  
- Binary search is **much faster** but requires the array to be **sorted**.  
- All three techniques were successfully implemented in C++.  
- The experiment provided clarity on the **trade-offs** between simplicity and efficiency in searching algorithms.  
- Practical takeaway: Use **Linear/Sequential search** for small/unsorted data and **Binary search** for large, sorted datasets.  

---
