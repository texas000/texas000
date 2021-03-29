# LeetCode #4 - Median of Two Sorted Arrays

Hello folks, this problem is marked as "Hard"

## Problem Statement

Given two sorted arrays nums1 and nums2 of size m and n respectively, return **the median** of the two sorted arrays.

## Examples

**Example 1**

```
Input: nums1 = [1, 3] nums = [2]
Output: 2
```

**Example 2**

```
Input: nums1 = [1, 2] nums = [3, 4]
Output: 2.5
```

**Example 3**

```
Input: nums1 = [0, 0] nums = [0, 0]
Output: 0
```

**Example 1**

```
Input: nums1 = [] nums = [1]
Output: 1
```

**Example 1**

```
Input: nums1 = [2] nums = []
Output: 2
```

## Approch

1. Merge arrays
2. Sort merged array
3. return the median value

## Steps

Following are the steps that we will follow:

1. Define the `unsorted` varaible and store the concat of nums1 and nums2
2. Define the `sorted` variable and store the sorted array
3. Check if the `sorted` array has even or odd number of elements
4. If `sorted` has even number of elements, then add two values in the middle and return the average
5. If `sorted` has odd number of elements, then return the middle element

## Javascript Code

```javascript
var findMeidanSortedArrays = function(num1, num2) {
    var unsorted = nums1.conact(nums2)
    var sorted = unsorted.sort((a,b)=> return a-b)
    if(sorted.length%2===0) {
        //Even number of elements
        var first = (sorted.length/2)-1
        var second = (sorted.length/2)
        return (sorted[first]+sorted[second])/2
    } else {
        //Odd number of elements
        var middle = (sorted.length-1)/2
        return sorted[middle]
    }
}
```
