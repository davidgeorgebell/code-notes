# FizzBuzz

Create a function that takes in a number. 

**If** the number is divisible by 3 return 'Fizz'
**If** the number is divisible by 5 return 'Buzz'
**If** the number is divisible by both 3 and 5 return 'FizzBuzz'
**If** the number is divisible by neither 3 or 5 return the number

```javascript
const fizzBuzz = (number) => {
  let output = []
  
  for (let i = 1; i <= number; i++) {
    if(i % 3 === 0 && i % 5 === 0) {
      output.push('FizzBuzz')
    }
    else if (i % 3 === 0) {
      output.push('Fizz')
    }
    else if (i % 5 === 0) {
      output.push('Buzz')
    }
    else {
      output.push(i.toString())
    }
  }
    return output
}
/* [
  '1',        '2',
  'Fizz',     '4',
  'Buzz',     'Fizz',
  '7',        '8',
  'Fizz',     'Buzz',
  '11',       'Fizz',
  '13',       '14',
  'FizzBuzz'
] */
```