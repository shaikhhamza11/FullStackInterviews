## [[⬆]](../README.md) Data Structure Using JavaScript

#### Q1: Find first pair in an array who sum is zero ⭐
```js
#input
const numbers = [-5, -4, -3, -2, -1, 0, 2, 4, 6, 8]
#output 
```
**Soultion 1:**

```js
const numbers = [-5, -4, -3, -2, -1, 0, 2, 4, 6, 8]

const getSumOfZero = (numbers) => {
  for (let i = 0; i < numbers.length; i++) {
    for (let j = 1; j < numbers.length; j++) {
      if (numbers[i] + numbers[j] === 0) {
        return [numbers[i], numbers[j]]
      }
    }
  }
}
console.log(getSumOfZero(numbers))

#output
[-4, 4]
#Time complexity
o(n^2) quadractic time complexity
```

**Soulution 2:**
```js
const numbers = [-5, -4, -3, -2, -1, 0, 2, 4, 6, 8]

const getSumOfZero = (numbers) => {
  let left = 0;
  let right = numbers.length - 1;
  while (left < right) {
    const sum = numbers[left] + numbers[right]
    if (sum === 0) {
      return [numbers[left], numbers[right]]
    } else if (sum > 0) {
      right--
    } else {
      left++
    }
  }
}
console.log(getSumOfZero(numbers))

#output
[-4, 4]
#Time complexity
o(n) linear time complexity
```
###### Note: This logic will work only for sorted array