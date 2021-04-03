# LeetCode #5 - Longest Palindromic Substring

Given a string `s`, return the _longest palindromic substring_ in `s`.

> What is panlindromic
> a word, verse, or sentence or a number that reads the same backward or forward.

## Examples

**Example 1**

```javascript
Input = "babad";
Output = "bab" || "aba";
```

**Example 2**

```javascript
Input = "cbbd";
Output = "bb";
```

**Example 3**

```javascript
Input = "a";
Output = "a";
```

**Example 4**

```javascript
Input = "ac";
Output = "a";
```

**Constraints**

- `1<= s.length <=1000`
- s consist of only digits and Enlgish letters (lower case and upper case)

**Approach**

- Compare the first and last character.
- If the inner character is same, update the longest string.
- When there is a single character between the character, discard the character if the front and back letter are the same.

Unsolved yet...
