> start (and try to finish) the [loop tasks](https://javascript.info/while-for) from javascript.info and paste each of your solutions into this file.  
> Don't be afraid of peeking at the solutions!  Just be sure you study them well

## 1.Last loop value
```js
let i = 3;

while (i) {
  alert( i-- );
}

The answer: 1 Because every loop iteration decreases i by 1. The check while(i) stops the loop when i = 0.
```
## 2.Which values does the while loop show?
```js
> The prefix form ++i:

let i = 0;
while (++i < 5) alert( i );                       
                                                      
alert( 1 ) 

The answer: 
alert( i )=1
           2
           3
           4
           
> The postfix form i++:

let i = 0;
while (i++ < 5) alert( i );

The answer:
alert( i )=1
           2
           3
           4
           5

```
 In this example postfix/prefix forms lead to different results.
## 3.Which values get shown by the "for" loop?

> Both loops alert same values.
```js
1. alert( i )=0
              1
              2
              3
              4
              
2. alert( i )=0
              1
              2
              3
              4             

```
## 4.Output even numbers in the loop
```js
for (let i=2; i<=10; i+=2)
console.log(i)
; 

```
## 5.Replace "for" with "while"
```js
let i = 0;
while (i < 3) {
  console.log( `number ${i}!` );
  i++;
}
```
## 6.Repeat until the input is correct
```js
let i;

do {
  i = prompt("please enter a number greater than 100");
} while (i <= 100);
```
## 7.Output prime numbers
```js
let n = 10;
for (let i = 2; i <= n; i++) { 

  for (let j = 2; j < i; j++) { 
    if (i % j == 0) ;  
  }

  alert( i ); 
}
```
