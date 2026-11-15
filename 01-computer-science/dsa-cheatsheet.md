# 💻 Data Structures & Algorithms (DSA) Quick Reference

> **Stream:** Computer Science & IT | **High-Yield Cheat Sheet**

---

## 📊 1. Common Data Structures & Time Complexities

| Data Structure | Access | Search | Insertion | Deletion | Best Used For |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Array** | O(1) | O(n) | O(n) | O(n) | Fast index lookup |
| **Linked List** | O(n) | O(n) | O(1) | O(1) | Frequent insertions/deletions |
| **Stack (LIFO)** | O(n) | O(n) | O(1) | O(1) | Undo operations, recursion |
| **Queue (FIFO)** | O(n) | O(n) | O(1) | O(1) | Task scheduling, breadth-first search |
| **Hash Table** | N/A | O(1) | O(1) | O(1) | Fast key-value lookups |

---

## 🔍 2. Essential Python Code Snippets

### Binary Search (O(log n))
```python
def binary_search(arr, target):
    left, right = 0, len(arr) - 1
    while left <= right:
        mid = (left + right) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    return -1
