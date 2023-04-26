# Add-Digits

Given an integer num, repeatedly add all its digits until the result has only one digit, and return it. 

## Example 1:

Input: num = 38

Output: 2

Explanation: The process is

38 --> 3 + 8 --> 11

11 --> 1 + 1 --> 2 

Since 2 has only one digit, return it.

## Example 2:

Input: num = 0

Output: 0
 

## Constraints:

0 <= num <= 231 - 1

# Solution 
The problem can be solved using a simple recursive function that calculates the sum of digits of the given number, and calls itself with the sum until the sum becomes a single digit.

- we first check if the given number is less than 10 , then we return the number as it is. 
- If the number is greater than or equal to 10, we calculate the sum of digits of the number by adding the remainder of the number divided by 10, and dividing the number by 10. 
- We then call the same function recursively with the sum of digits as the argument, until the sum becomes a single digit. Finally, we return the single digit.
## Time Cmplexity 
the time complexity of the recursive function is O(log n),

