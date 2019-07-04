> start (and try to finish) the [conditional tasks](https://javascript.info/ifelse) from javascript.info and paste each of your solutions into this file.  
> things that might help: [javascript.inf - comparisons](https://javascript.info/comparison), [interactive coercion table](https://janke-learning.org/equalities-coercion/), [equalities table](https://dorey.github.io/JavaScript-Equality-Table/)

## 1.if (a string with zero)
```js
if ("0") {
  alert( 'Hello' );
}
```
>Yes, it will be shown. Because "0" is a string and it gives "True" value.

## 2.The name of JavaScript
```js
let question = prompt("What is the official name of JavaScript?");

if (question == "ECMAScript"){
  alert ("Right!");
  }else{
    alert("Didn’t know? ECMAScript");
    }
```
## 3.Show the sign
```js
let number = prompt("Please, enter a number:");

if(number > 0 ){
  alert (1); 
}else if(number < 0){
  alert(-1);
 }else{
   alert(0);
   }
```
## 4.Rewrite 'if' into '?'
```js
if (a + b < 4) {
  result = 'Below';
} else {
  result = 'Over';
}
// Rewrite using the ternary operator '?'
let a , b ;
let result = (a + b < 4) ? "below" : "over";
```
## 5.Rewrite 'if..else' into '?'
```js
let message;

if (login ==   ) {
  message = 'Hello';
} else if (login == 'Director') {
  message = 'Greetings';
} else if (login == '') {
  message = 'No login';
} else {
  message = '';
}

// Rewrite using the ternary operator '?'
let login;
let message = (login == "Employee") ? "Hello" :
(login == "Director") ? "Greetings" :
(login == "") ? "No login" :
 "" ;
```
