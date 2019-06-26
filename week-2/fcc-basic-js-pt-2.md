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
## 13.

```js
```
## 14.

```js
```
## 15.

```js
```
## 16.

```js
```
## 17.

```js
```
## 18.

```js
```
## 19.

```js
```
## 20.

```js
```
## 21.

```js
```
## 22.

```js
```
