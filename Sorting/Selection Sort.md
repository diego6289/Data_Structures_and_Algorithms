# Selection Sort



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

- Works by repeatedly selecting the smallest (or largest) element from the unsorted position of the list and moving it to the sorted position of the list.
- Unstable.
- In-place.
- Best for small datasets.

## Time Complexity

Best Case: $O(n^2)$

Average Case: $O(n^2)$

Worst Case: $O(n^2)$

## Space Complexity
$O(1)$
