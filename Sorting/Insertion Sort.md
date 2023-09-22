# Insertion Sort


```c++
for (int i = 1; i < n; i++) {
    int j = i - 1;
    while (j >= 0 && nums[j] > nums[j + 1]) {
        swap(nums[j], nums[j + 1]);
        j--;
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

