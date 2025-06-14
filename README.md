# Day46-50-days-coding-challenge


## 🌟 Problem 1: Find Center of Star Graph

### Problem Statement:
Given a star graph represented by `n-1` edges, find the center node.

### Approach:
- In a valid star graph, the center appears in every edge.
- So, the node common to the first two edges is the center.

### Example:
Input: [[1,2],[2,3],[4,2]]  
Output: 2

---

## 🧮 Problem 2: Prime Number of Set Bits

### Problem Statement:
Given two integers `left` and `right`, count how many numbers in the range have a **prime** number of set bits (1s in their binary representation).

### Steps:
1. Loop through numbers from `left` to `right`.
2. Count set bits using `bin(num).count("1")`.
3. Check if the count is a prime number.

### Prime Numbers Considered:
Since `right <= 10^6`, max bits in binary is around 20. So primes ≤ 20 are:  
`[2, 3, 5, 7, 11, 13, 17, 19]`

### Example:
Input: left = 10, right = 15  
Binary:
- 10 → 1010 → 2 set bits ✅  
- 11 → 1011 → 3 set bits ✅  
- 12 → 1100 → 2 set bits ✅  
- 13 → 1101 → 3 set bits ✅  
- 14 → 1110 → 3 set bits ✅  
- 15 → 1111 → 4 set bits ❌  
Output: 5
