# Palindrome - Palindrome level

Palindrome is a word, phrase, or sequence that reads the same backward as forward e.g. "madam", "nurses run", "23499432". When palindrome sequence is splitted in half, the first sequence may be a palindrome too.

Palindrome Level is how many times a palindrome sequence can be splitted in half until the first sequence from splitted is not a palindrome or until the first sequence is just a character.

_Your task is to calculate palindrome level given a string._

## Example

- "nurses run"-> 1 level
- "451545154" -> 2 level
- "dam madam mad" -> 2 level

## Explanation

- "nurses run" :
  - "nursesrun" is a palindrome then can be splited (level 0)
  - "nurse" is not a palindrome, cant be splited anymore (level 1)
  - 1 level palindrome
- "451545154" :
  - "451545154" is a palindrome then can be splited (level 0)
  - "45154" is a palindrome then can be splited (level 1)
  - "451" is not a palindrome, cant be splited anymore (level 2)
  - 2 level of palindrome
- "dam madam mad"
  - "dammadammad" is a palindrome then can be splited (level 0)
  - "dammad" is a palindrome then can be splited (level 1)
  - "dam" is not a palindrome, cant be splited anymore (level 2)
  - 2 level of palindrome

## Constraint

- Characters are [0-9],[a-z],[A-Z], " ".
- 0 <= input length <= 262
- Space is ignored and case insensitive
- if the sequence length is odd number, then after split the sequence, take the middle character to the first sequence: "madam" -> "mad"
