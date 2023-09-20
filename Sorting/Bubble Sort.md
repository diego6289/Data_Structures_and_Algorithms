```c++
bool swapped = true;
for (int i = 0; i < n - 1; i++) {
    swapped = false;
    for (int j = 0; j < n - i - 1; j++) {
        if (nums[j] > nums[j + 1]) {
            swapped = true;
            swap(nums[j], nums[j + 1]);
        }
    }
    if (!swapped) break;
}
```

- Works by repeatedly swapping adjacent elements if they are in the wrong order.
- Stable Algorathim (Maintains the relative order of the items with equal sort keys)

## Time Complexity

Best Case: $O(n)

Average Case: $O(n^2)

Worst Case: $O(n^2)
