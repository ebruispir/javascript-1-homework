> start (and try to finish) the [object tasks](https://javascript.info/object) from javascript.info and paste each of your solutions into this file.    
> Don't be afraid of peeking at the solutions!  Just be sure you study them well

## 1.Hello, object
```js
let user = {name :"John", surname :"Smith",} ;
user.name = "Pete";
delete user.name;
```
## 2.Check for emptiness
```js
let obj= {};
function isEmpty(obj) {
    for (let key in obj) {
      return false;
    }
    return true;
  }
  console.log(isEmpty(obj));
```
## 3.Constant objects?
```js
const user = {
  name: "John"
};
user.name = "Pete";
```
> Answer= Yes, it possible to change an object declared with const but if it is a variable declared with const then you can't change its value.

## 4.Sum object properties
```js
let salaries = {
  John: 100,
  Ann: 160,
  Pete: 130
}
var sum = 0;
for(let key in salaries){
  sum += salaries[key];
  }
  console.log(sum);
```
## 5.Multiply numeric properties by 2
```js
let obj = { speed:100, time:20, name:"toyota",}
function multiplyNumeric(obj){
  for(let key in obj){
    if(typeof obj[key] == "number"){
      obj[key] *= 2;
    }
  }
}

```
