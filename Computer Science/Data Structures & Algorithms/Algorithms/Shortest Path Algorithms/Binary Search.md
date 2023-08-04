**Binary Search** is defined as a searching [[algorithms|algorithm]] used in a sorted [[array]] by repeatedly dividing the search interval in half. The idea of binary search is to use the information that the array is sorted and reduce the time complexity to $O(logN)$

#### Python implementation:

```python
def binarySearch(arr, target):
	left, right = 0, len(arr) - 1
    while left <= right:
        mid = left + (right - left) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    return -1
```