1. Describe in plain English what `Array.map()` does

- the `map()` method allows us to create an array using the contents of a pre-existing array, except the contents are changed in some way.
- the way that the array is changed depends on the function that we provide `map()`
- EXAMPLE:

```javascript
const my_array = [1, 2, 3, 4];

const new_array = my_array.map((x) => x * 3);

console.log(map1);
// Output: Array [3, 6, 9, 12]
```

2.

- the `reduce()` function, like `map()` uses a pre-defined array as input. the reducer returns a value a called the _accumulator_. For each element in an array, the reducer functions will perform a method the accumulator, usually this involves changing the accumliator in some way based on each element.
- EXAMPLE:

```javascript
const my_array = [1, 2, 3, 4];

const my_reducer = (accumulator, element) => accumulator + element;

console.log(my_array.reduce(my_reducer, 5));
// 5 + 1 + 2 + 3 + 4
// Output: 15
```
