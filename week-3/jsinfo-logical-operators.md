> start (and try to finish) the [loop tasks](https://javascript.info/logical-operators) from javascript.info and paste each of your solutions into this file.  
> things that might help: [truthiness](https://github.com/janke-learning/truthiness/blob/master/README.md)

## 1.What's the result of OR?
```js
alert( null || 2 || undefined );
```
> The answer is 2 .Because null is falsy value.
## 2.What's the result of OR'ed alerts?
```js
alert( alert(1) || 2 || alert(3) );
```
> The answer is 2 .The first OR || evaluates it’s left operand alert(1). That shows the first message with 1.
The alert returns undefined, so OR goes on to the second operand searching for a truthy value.

## 3.What is the result of AND?
```js
alert( 1 && null && 2 );
```
>The answer is "null".

## 4.What is the result of AND'ed alerts?
```js
alert( alert(1) && alert(2) );
```
> The answer is 1.Because alert(1) is undefined and it is a falsy value. 
## 5.The result of OR AND OR
```js
alert( null || 2 && 3 || 4 );
```
> The precedence of AND && operator is higher than OR ||.So the code 2 && 3 = 3.The result is the first truthy value: 3.

## 6.Check the range between
```js
 var age;
 if (age >= 14 && age <= 90){
 }
```
## 7.Check the range outside
```js
The first variant: if (!(age >= 14 && age <= 90))

The second variant: if (age < 14 || age > 90)
```
## 8.A question about "if"
```js
if (-1 || 0) alert( 'first' );  ----> The result of -1 || 0 = -1, truthy.

if (null || -1 && 1) alert( 'third' ); -------> The result of null || -1 && 1 = 1,truthy .
```
## 9.Check the login
```js
let userName = prompt("Who's there?", '');

if (userName == 'Admin') {

  let pass = prompt('Password?', '');

  if (pass == 'TheMaster') {
    alert( 'Welcome!' );
  } else if (pass == '' || pass == null) {
    alert( 'Canceled.' );
  } else {
    alert( 'Wrong password' );
  }

} else if (userName == '' || userName == null) {
  alert( 'Canceled' );
} else {
  alert( "I don't know you" );
}
```
