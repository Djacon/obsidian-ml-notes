**Bubble Sort** is the simplest sorting [[Algorithms|algorithm]] that works by repeatedly swapping the adjacent elements if they are in the wrong order. This algorithm is not suitable for large [[data]] sets as its average and worst-case time complexity is quite high

![[Bubble_sort_image.gif]]


#### Python implementation:
```python
def bubbleSort(arr):
    for i in range(len(arr)):
        for j in range(len(arr)-1):
	        if arr[j] > arr[j+1]:
		        arr[j], arr[j+1] = arr[j+1], arr[j]
	return arr
```

#### Complexity

* Time Complexity: O$(n^2)$
* Auxiliary Space: O$(1)$