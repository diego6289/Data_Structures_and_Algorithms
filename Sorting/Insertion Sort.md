# Insertion Sort


```c++
for (int i = 0; i < n - 1; i++) {
    int idx = i;
    for (int j = i + 1; j < n; j++) {
        if (nums[j] < nums[idx]) {
            idx = j;
        }
    }
    if (idx != i) {
        swap(nums[i], nums[idx]);
    }
}
```

- Works similar to the way you sort playing cards in your hand. The array is virtually split into a sorted and an unsorted part. Values from the unsorted part are picked and placed at the correct position in the sorted part.
- Stable.
- In-place.
- Best for small datasets or datasets that are already partially sorted.

## Time Complexity

Best Case: $O(n)$

Average Case: $O(n^2)$

Worst Case: $O(n^2)$

## Space Complexity
$O(1)$

