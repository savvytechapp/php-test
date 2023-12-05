Problem: Given a sorted array that can contain duplicates, find the first and last position of a given target value. If the target is not found, return [-1, -1].


Example :

```
$search_array = [1, 2, 3, 4, 4, 4, 5, 5, 6, 6, 7, 7, 8, 8, 8, 8, 8, 8, 8, 8, 8, 8, 8, 8, 8, 8, 8, 9];
$target = 4;
print_r(findRange($search_array , $target));
```

Should output [2,4] because 4 first appears at index 2 and last appears at index 4.

The reason why we want to use a binary search in this problem is that a linear scan is too slow (O(n) complexity), while a binary search can find elements in log(n) time.
