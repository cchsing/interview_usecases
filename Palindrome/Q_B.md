# Palindrome - Sum of palindrome level

Palindrome is a word, phrase, or sequence that reads the same backward as forward e.g. "madam", "nurses run", "23499432". When palindrome sequence is splitted in half, the first sequence may be a palindrome too.

Sum of the Palindrome Level is calculated by adding palindrome level of all the string's prefixes. See Question 1 on how to calculate the palindrome level.

_Your task is to calculate sum of palindrome level given a string._

## Example

- "abacaba" -> 2
- "aaa" -> 3

## Explanation

- "abacaba" : 1 + 1 = 2 (sum of palindrome level)
  - a = 0 level of palindrome
  - ab = 0 level of palindrome
  - aba = 1 level of palindrome
  - abac = 0 level of palindrome
  - abaca = 0 level of palindrome
  - abacab = 0 level of palindrome
  - abacaba = 1 level of palindrome
- "aaa" : 1 + 2 = 3 (sum of palindrome level)
  - a = 0 level of palindrome
  - aa = 1 level of palindrome
  - aaa = 2 level of palindrome

## Constraint

- Characters are [0-9], [a-z], [A-Z], " ".
- 0 <= input length <= 262
- Space is ignored and case insensitive
- if the sequence length is odd number, then after split the sequence, take the middle character to the first sequence: "madam" -> "mad"
