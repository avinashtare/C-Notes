# Methods Of Array
* Array methods are functions that can be applied to arrays in C++. 
* They can perform calculations or changes to arrays.
* save time by avoiding the need to write common functions from scratch.

## List Of Inbuild Functions In C++
| Function                        | Description                                           |
| ------------------------------- | ----------------------------------------------------- |
| `begin(arr)`               | Returns an iterator pointing to the beginning of the array or container. |
| `end(arr)`                 | Returns an iterator pointing to the end of the array or container. |
| `size(arr)` or `sizeof(arr)/sizeof(arr[0])` | Returns the number of elements in the array. |
| `swap(arr1, arr2)`         | Swaps the contents of two arrays.                     |
| `copy(begin, end, dest)`   | Copies elements from the range `[begin, end)` to the destination array `dest`. |
| `fill(begin, end, value)`  | Sets all elements in the range `[begin, end)` to the specified value. |
| `reverse(begin, end)`      | Reverses the order of elements in the range `[begin, end)`. |
| `sort(begin, end)`         | Sorts the elements in the range `[begin, end)` in ascending order. |
| `binary_search(begin, end, value)` | Performs binary search in the sorted range `[begin, end)` for the specified value. |
| `find(begin, end, value)`  | Searches for the first occurrence of `value` in the range `[begin, end)`. |
| `accumulate(begin, end, init)` | Computes the sum of the elements in the range `[begin, end)` starting with the initial value `init`. |
| `min_element(begin, end)`  | Returns an iterator pointing to the minimum element in the range `[begin, end)`. |
| `max_element(begin, end)`  | Returns an iterator pointing to the maximum element in the range `[begin, end)`. |




| [Back: Operation Of Array](./operation.md) |
| ----------------------------- |