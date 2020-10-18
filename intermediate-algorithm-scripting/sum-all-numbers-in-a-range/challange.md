# Intermediate Algorithm Scripting: `Sum All Numbers in a Range`

We'll pass you an array of two numbers. Return the sum of those two numbers plus the sum of all the numbers between them. The lowest number will not always come first.

For example, `sumAll([4,1])` should return **10** because **sum of all the numbers between 1 and 4** (both inclusive) is **10**.

## :point_right: Result

- `sumAll([1, 4]) should return a number.`
- `sumAll([1, 4]) should return 10.`
- `sumAll([4, 1]) should return 10.`
- `sumAll([5, 10]) should return 45.`
- `sumAll([10, 5]) should return 45.`

## Answers

```javascript
function sumAll(arr) {
  const min = Math.min(...arr);
  const max = Math.max(...arr);
  let result;

  for (let i = min; i <= max; i++) {
    result += i;
  }

  return result;
}

const result = sumAll([1, 4]);

console.log(result);
```
