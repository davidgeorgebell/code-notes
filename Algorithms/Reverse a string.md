# Reverse a string

The way if the string is an array of strings.

Create a left and right variables. 

These need to cross over.

A temporary or hold variable is used to hole either left or rights value.

string index left needs to become string index right.

Then increment.

```javascript
const reverseString = (s) => {
  let left = 0
  let right = s.length - 1

  while (left < right) {
    let temp = s[left]
    s[left] = s[right]
    s[right] = temp

    left++
    right--
  }
  return s
}

reverseString(['h','e','l','l','o'])
// [ 'o', 'l', 'l', 'e', 'h' ]
```

When type is string.

Loop down through the `string` length.

Add the string index to your output `variable`

```javascript
const reverseString = (s) => {
  let output = ''
  for (let i = s.length - 1; i >= 0; i--) {
    output += s[i]
  }
  return output
}
reverseString('hello')
// olleh
```