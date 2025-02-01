# Daily-Leetcode-problem-solution5
PROBLEM

An array is considered special if every pair of its adjacent elements contains two numbers with different parity.
You are given an array of integers nums. Return true if nums is a special array, otherwise, return false.

Intuition

To determine if the array is special, check whether each pair of adjacent elements has different parity (one is odd and the other is even).

Approach

We iterate through the array from index 0 to n-2 (because we check pairs of adjacent elements).
For each pair nums[i] and nums[i+1], we check if both elements have the same parity using the modulo operation.
(nums[i] % 2) will return 0 for even numbers and 1 for odd numbers.
If both elements have the same result from this operation, it means they have the same parity.
If we find such a pair, we return false. If no such pair is found after checking all the adjacent pairs, we return true.

Complexity

Time complexity:
O(n)

Space complexity:
O(1)
