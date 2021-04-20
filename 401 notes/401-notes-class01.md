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

2. Describe in plain English what `Array.reduce()` does

- the `reduce()` function, like `map()` uses a pre-defined array as input. the reducer returns a value a called the _accumulator_. For each element in an array, the reducer functions will perform a method the accumulator, usually this involves changing the accumliator in some way based on each element.
- EXAMPLE:

```javascript
const my_array = [1, 2, 3, 4];

const my_reducer = (accumulator, element) => accumulator + element;

console.log(my_array.reduce(my_reducer, 5));
// 5 + 1 + 2 + 3 + 4
// Output: 15
```

3. Provide code snippets showing how to use `superagent()` to fetch data from a URL and og the result

- With Promise `.then()` syntax

```javascript
superagent.get(`https://swapi.dev/api/`)then

let getCharacters = () =>{
  superagent.get(`https://swapi.dev/api/people`).then(data => {

   data.body.results.forEach(item => {
     console.log({key: item.name, url: item.url});
    })
  });

  getCharacters()
}
```

- Again with `async` / `await` syntax

```javascript
async function getACity(city) {
  let results = await superagent.get(`https://geocode.xyz/${city}?json=1`);
  console.log(results.body);
}
getACity("Seattle");
```

4. Explain promises as though you were mentoring a Code 301 level student

- A promise is a javascipt object that represents an asyncronous operation - and that operation's results - that has not yet been triggered, regardless whether or not the opertaion successed or fails.

5. Are all callback functions considered to be Asynchronous? Why or Why Not?

- Not all callbacks are asyncronus.
- A callback involes a parent function, and a child function. the child function is the one being used by the parent as a parameter. If the parent has to wait on the child function to return before it returns, then it is syncronous. otherwise, it is asyncronous.
