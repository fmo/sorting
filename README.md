# Bubble Sort

```
func BubbleSort(arr []int) {
	n := len(arr)
	for i := 0; i < n; i++ {
		// Flag to detect if any swapping occurs
		swapped := false
		for j := 0; j < n-i-1; j++ {
			// Compare adjacent elements and swap if needed
			if arr[j] > arr[j+1] {
				arr[j], arr[j+1] = arr[j+1], arr[j]
				swapped = true
			}
		}
		// If no swapping occurred, the slice is already sorted
		if !swapped {
			break
		}
	}
}
```
