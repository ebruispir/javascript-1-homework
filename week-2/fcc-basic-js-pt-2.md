> complete the rest of [basic JS exercises](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript) on FCC and paste each of your solutions into this file.  This will allow you to use your FCC exercises as a study reference later on  
> [completed example](https://github.com/AlfiYusrina/hyf-javascript1/blob/master/week1/freecode_camp_solutions.MD) 

>[My freeCodeCamp Portfolio](https://www.freecodecamp.org/ebruispir)

## 1.Counting Cards

```js
var count = 0;

function cc(card) {
  
   switch(card){
        case 2:
        case 3:
        case 4:
        case 5:
        case 6:
          count++;
          break;
        case 10:
        case "J":
        case "Q":
        case "K":
        case "A":
          count--;
          break;
      }
      if (count > 0){
        return count + " Bet";
      } else {
        return count + " Hold";
      }
  
  return "Change Me";

}
cc(2); cc(3); cc(7); cc('K'); cc('A');
```
## 2.Build JavaScript Objects

```js
var myDog = {
  "name":"Efe",
  "legs": 4,
  "tails":1,
  "friends":["cats","birds"]
};
```
## 3.Accessing Object Properties with Dot Notation

```js
var testObj = {
  "hat": "ballcap",
  "shirt": "jersey",
  "shoes": "cleats"
};

var hatValue = testObj.hat;     
var shirtValue = testObj.shirt;  
```
## 4.Accessing Object Properties with Bracket Notation

```js
var testObj = {
  "an entree": "hamburger",
  "my side": "veggies",
  "the drink": "water"
};

var entreeValue = testObj["an entree"]; 
var drinkValue = testObj["the drink"];  
```
## 5.Accessing Object Properties with Variables

```js
var testObj = {
  12: "Namath",
  16: "Montana",
  19: "Unitas"
};

var playerNumber=16;     
var player = testObj[playerNumber]; 
```
## 6.Updating Object Properties

```js
var myDog = {
  "name": "Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

myDog.name= "Happy Coder"

```
## 7.Add New Properties to a JavaScript Object

```js
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

myDog.bark= "woof";
```
## 8.Delete Properties from a JavaScript Object


```js
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};

delete myDog.tails;
```
## 9.Using Objects for Lookups

```js
function phoneticLookup(val) {
  var result = "";
    var lookup = {
    "alpha": "Adams",
    "bravo": "Boston",
    "charlie": "Chicago",
    "delta": "Denver",
    "echo": "Easy",
    "foxtrot": "Frank"
  };
 result = lookup[val];
 
 return result;
}
phoneticLookup("charlie");
```
## 10.Testing Objects for Properties

```js
var myObj = {
  gift: "pony",
  pet: "kitten",
  bed: "sleigh"
};

function checkObj(checkProp) {

  if (myObj.hasOwnProperty(checkProp) == true) {
    return myObj[checkProp];
  }
  else {
       return "Not Found"
  }
  return "Change Me!";
}

checkObj("gift");
```
## 11.Manipulating Complex Objects

```js
var myMusic = [
  {
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [ 
      "CD",
      "8T",
      "LP"
    ],
    "gold": true
  }
,{
   "artist": "Deep Purple",
   "title": "Smoke on the water",
   "release_year": 1976,
   "formats": [ 
     "CD",
     "8T",
     "LP"
   ],
 }
];
```
## 12.Accessing Nested Objects

```js
// Setup
var myStorage = {
  "car": {
    "inside": {
      "glove box": "maps",
      "passenger seat": "crumbs"
     },
    "outside": {
      "trunk": "jack"
    }
  }
};

var gloveBoxContents = myStorage.car.inside["glove box"];
```
## 13.Accessing Nested Arrays

```js
var myPlants = [
  { 
    type: "flowers",
    list: [
      "rose",
      "tulip",
      "dandelion"
    ]
  },
  {
    type: "trees",
    list: [
      "fir",
      "pine",
      "birch"
    ]
  }  
];

var secondTree = myPlants[1].list[1]; 
```
## 14.Record Collection

```js
var collection = {
    "2548": {
      "album": "Slippery When Wet",
      "artist": "Bon Jovi",
      "tracks": [ 
        "Let It Rock", 
        "You Give Love a Bad Name" 
      ]
    },
    "2468": {
      "album": "1999",
      "artist": "Prince",
      "tracks": [ 
        "1999", 
        "Little Red Corvette" 
      ]
    },
    "1245": {
      "artist": "Robert Palmer",
      "tracks": [ ]
    },
    "5439": {
      "album": "ABBA Gold"
    }
};
var collectionCopy = JSON.parse(JSON.stringify(collection))

function updateRecords(id, prop, value) {
  if (prop === "tracks" && value !== "") {
   if(collection[id][prop]) {
    collection[id][prop].push(value);
   }
   else {
    collection[id][prop]=[value];
   }
  } else if (value !== "") {
    collection[id][prop] = value;
  } else {
    delete collection[id][prop];
  }
  
  
  return collection;
}

updateRecords(5439, "artist", "ABBA");
```
## 15.Iterate with JavaScript While Loops

```js
var myArray = [];

var a = 0;
while(a<5){
myArray.push(a);
a++;
}
```
## 16. Iterate with JavaScript For Loops

```
var myArray = [];
for (var a = 1; a <= 5; a++){
    myArray.push(a);
}
```
## 17.Iterate Odd Numbers With a For Loop

```js
var myArray = [];

for(var a=1; a<=9; a +=2){
  myArray.push(a);
}

```
## 18.Count Backwards With a For Loop

```js
var myArray = [];

for(var a=9; a>0; a -= 2){
myArray.push(a);
}

```
## 19.Iterate Through an Array with a For Loop

```js
var myArr = [ 2, 3, 4, 5, 6];
var total = 0;
for (var a=0; a<myArr.length; a ++){
  total += myArr[a]
}
```
## 20.Nesting For Loops

```js
function multiplyAll(arr) {
  var product = 1;
 
  for(var i=0; i<arr.length; i ++ ){
      for( var j=0; j<arr[i].length; j ++){
      product = product*arr[i][j] ;
      }
  }

  return product;
}

multiplyAll([[1,2],[3,4],[5,6,7]]);
```
## 21.Iterate with JavaScript Do...While Loops

```js
var myArray = [];
var i = 10;
do  {
  myArray.push(i);
  i++;
}while (i < 5)
```
## 22.Profile Lookup

```js
var contacts = [
    {
        "firstName": "Akira",
        "lastName": "Laine",
        "number": "0543236543",
        "likes": ["Pizza", "Coding", "Brownie Points"]
    },
    {
        "firstName": "Harry",
        "lastName": "Potter",
        "number": "0994372684",
        "likes": ["Hogwarts", "Magic", "Hagrid"]
    },
    {
        "firstName": "Sherlock",
        "lastName": "Holmes",
        "number": "0487345643",
        "likes": ["Intriguing Cases", "Violin"]
    },
    {
        "firstName": "Kristian",
        "lastName": "Vos",
        "number": "unknown",
        "likes": ["JavaScript", "Gaming", "Foxes"]
    }
];


function lookUpProfile(name, prop){
// Only change code below this line
for (var x = 0; x < contacts.length; x++){
    if (contacts[x].firstName === name) {
        if (contacts[x].hasOwnProperty(prop)) {
            return contacts[x][prop];
        } else {
            return "No such property";
        }
    }
}
return "No such contact";

}
lookUpProfile("Akira", "likes");
```
## 23.Generate Random Fractions with JavaScript
```js
function randomFraction() {

  var result = 0;
  while (result === 0) {
    result = Math.random();
  }

  return result;  
 
}
```
## 24.Generate Random Whole Numbers with JavaScript
```js
var randomNumberBetween0and19 = Math.floor(Math.random() * 20);

function randomWholeNum() {

  return Math.floor(Math.random() * 10);
  }
```
## 25.Generate Random Whole Numbers within a Range
```js
function randomRange(myMin, myMax) {

  return Math.floor(Math.random() * (myMax - myMin + 1)) + myMin;;
}

var myRandom = randomRange(5, 15);
```
## 26.Use the parseInt Function
```js
function convertToInteger(str) {
  return parseInt(str);
}

convertToInteger("56");
```
## 27.Use the parseInt Function with a Radix
```js
function convertToInteger(str) {
return parseInt(str,2); 
}

convertToInteger("10011");
```
## 28.Use the Conditional (Ternary) Operator
```js
function checkEqual(a, b) {
  return a == b ? true : false ;
}

checkEqual(1, 2);
```
## 29.Use Multiple Conditional (Ternary) Operators
```js
function checkSign(num) {
return (num > 0) ? 'positive' : (num < 0) ? 'negative' : 'zero';
}

checkSign(10);
```
