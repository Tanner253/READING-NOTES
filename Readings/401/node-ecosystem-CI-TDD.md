# TDD AND CI 

- Describe (in plain English) what Array.map() does

  - Array.map will return a new array by default or an array with the values mutated with a callback function.

- Describe (in plain English) what Array.reduce() does

  - Array.Reduce will use a "container" to keep track of a value effected by iterating through the array with a selected callback function EX: SumElements

- Provide code snippets showing how to use superagent() to fetch data from a URL and log the result

  ```js
  console.log(superagent.get(url))
  ```

- With normal Promise .then() syntax

```js
  let MakeGetReq = (url, callback) => {
  return new Promise((resolve, reject) => {
    let res = superagent.get(url) ? "true" : "false"
    if(res) resolve(callback(res));
    else reject(callback(res));
})
}
```

- Again with async / await syntax

```js
  async function () {
    let res = await superagent.get(url);
    .then( res => {
      console.log(res);
    })
  }

```

- Explain promises as though you were mentoring a Code 301 level student

  - Promises are, promises! The promise is a object implemented from the promise class, which says "function please do work .THEN()  give me the data and ill handle it" The advantage to doing this is we keep track of promises in the event loop, which allows our front end to keep doing its thing while the process is happening, once the callstack is clear the event loop pushes the promise back to the stack and finished the response ect... Promise . then allows us to specify the sync behavior.

- Are all callback functions considered to be Asynchronous? Why or Why Not?

  - Callbacks are not asynchronous by nature, but can be used for asynchronous purposes. This is because of higher order functions which we learned about in 301. weather or not the callback function is async is dependant on the definition of the callback function itself. if we need to wait for data to do stuff then the callback should be async.