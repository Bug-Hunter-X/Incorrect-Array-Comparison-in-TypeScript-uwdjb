# Incorrect Array Comparison in TypeScript
This repository demonstrates a common bug in TypeScript related to comparing arrays of different lengths. The provided code attempts to compare two arrays for equality, but it fails to accurately handle cases where the arrays have unequal lengths.

## Bug Description
The `compareArrays` function is designed to determine if two number arrays are identical. However, it incorrectly returns `true` when comparing arrays of different lengths, rather than correctly returning `false`. This issue stems from the logic failing to consider the scenario of arrays with varying lengths before proceeding with element-wise comparison. 

## Solution
The solution corrects this by explicitly checking the lengths of the arrays before starting the element-wise comparison. If the lengths differ, the function correctly returns `false`, resolving the comparison inaccuracy.