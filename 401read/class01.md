# Class 01

## Array.map()

it's an array method throw it you can return a new value or array with some edits 

## Array.reduce()

Array method throw it you can return the accumulator value and it takes two parameters one for accumulator and the other one for current value the accumulator can be any data type you want.

## superagent codes

1. with `.then()` promises.
    ```
    superagent.get(url).then( x => {
        console.log('API data', x.body);
    });
    ```
1. with `async / await` fun.
    ```
    async function superAgent(){
        let result = await superagent.get(url);
        console.log('API data', result.body);
    };
    ```

## Promises
In 301 I thought promises is a built in code to do some certain things

## Are all callback functions considered to be Asynchronous? Why or Why Not?
Of course no because JavaScript is single threaded language but there's some operations make it multi threaded.