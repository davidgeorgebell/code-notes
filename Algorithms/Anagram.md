# Anagram

Pass two strings into a function. Check if either string is an anagram of the the other.

Using the frequency counter pattern. 

```javascript
function validAnagram(first, last){
  if(first.length !== last.length) return false

let output = {}

  for(let i = 0; i < first.length; i++) {
    let letter = first[i]
    output[letter] ? output[first] += 1 : output[letter] = 1
  }
  
  for(let i = 0; i < last.length; i++) {
    let letter = last[i]
    if(!output[letter]) {
      return false
    } else {
      return true
    }
  }
}

validAnagram('bat', 'tab')
```