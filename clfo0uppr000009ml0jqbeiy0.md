---
title: "Learn: Array Methods"
datePublished: Sat Mar 25 2023 13:43:22 GMT+0000 (Coordinated Universal Time)
cuid: clfo0uppr000009ml0jqbeiy0
slug: learn-array-methods
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1679732275048/0168980d-8bb4-4105-9235-347168830ed5.png
tags: javascript, ineuron, hiteshchoudharylco, hiteshchaudhary, anuragtiwarime

---

### Converting Array values to String

The JavaScript method `toString()` converts an array of values to Single String.

```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
console.log(fruits.toString());
//Output: Banana,Orange,Apple,Mango
```

The `join()` method also joins all array elements into a string.It behaves just like `toString()`, but in addition, you can specify the separator.`console.log(fruits.join("*"))` it will join the "\*" in between the elements of array.

### Popping and Pushing

In arrays, we have to do removing and add elements. The **pop** will remove the elements at the last of the array, the length will change. The **push** will add the elements at the last of the array, the length will change.

```javascript
// pop
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.pop();
console.log(fruits);// Banana, Orange, Apple
// push
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.push("Kiwi");
console.log(fruits);// Banana, Orange, Apple, Mango, Kiwi
```

### Shifting Elements

Shifting is like pop-ing but it works from starting of the array. The `shift()` method **removes** the first array element and "shifts" all other elements to a lower index.

The `unshift()` method adds a new element to an array at the beginning, and "unshifts" older elements. It returns the new array length.

```javascript
// Shift()
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.shift();
console.log(fruits);// Orange, Apple, Mango
//Unshift()
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.unshift("Lemon");
console.log(fruits);//Lemon,Banana, Orange, Apple, Mango
```

### JavaScript Array length

The `length` property provides an easy way to append a new element to an array. It is like push.

```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits[fruits.length] = "Kiwi";
```

> **Note:**
> 
> Array elements can be deleted using the JavaScript operator `delete`.
> 
> Using `delete` leaves `undefined` holes in the array.
> 
> Use **pop()** or **shift()** instead.

### Concatenating Arrays

The concatenating creates a new array by merging the two arrays.

**Note**: The `concat()` method does not change the existing arrays. It always returns a **new array**.

The `concat()` method can take **any number of array arguments.**

The `concat()` method can also take **strings as arguments**.

```javascript
const myGirls = ["Cecilie", "Lone"];
const myBoys = ["Emil", "Tobias", "Linus"];

const myChildren = myGirls.concat(myBoys);
console.log(myChildren); // Cecilie,Lone,Emil,Tobias,Linus

// More array arguments
const arr1 = ["Cecilie", "Lone"];
const arr2 = ["Emil", "Tobias", "Linus"];
const arr3 = ["Robin", "Morgan"];
const myChildren = arr1.concat(arr2, arr3);
console.log(myChildren); //Cecilie,Lone,Emil,Tobias,Linus, Robin, Morgan
```

### Flattening

Flattening an array is the process of reducing(1D) the dimensionality of an array.

### Array splice()

The `splice()` method can be used to add new items to an array with out removeing it or we can add elements by removeing some elements of the array.

```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.splice(2, 0, "Lemon", "Kiwi");
console.log(fruits); // Banana,Orange,Lemon,Kiwi,Apple,Mango
```

The first parameter (2) defines the position **where** new elements should be **added** (spliced in).

The second parameter (0) defines **how many** elements should be **removed**.

The rest of the parameters ("Lemon" , "Kiwi") define the new elements to be **added**.

The `splice()` method returns an array with the deleted items,

You can use `splice()` to **remove elements.**

```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.splice(0, 1); // 0th index will remove
console.log(fruits); // Orange, Apple, Mango

const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.splice(1, 1); // 1st index will remove
console.log(fruits); // Banana, Apple, Mango
```

### Array slice()

The `slice()` method slices out a piece of an array into a new array.

```javascript
const fruits = ["Banana", "Orange", "Lemon", "Apple", "Mango"];
const citrus = fruits.slice(1); // slice from 1st index
console.log(citrus); //Orange,Lemon,Apple,Mango
```

**Note:** The `slice()` method creates a new array.

The `slice()` method does not remove any elements from the source array.

The `slice()` method can take two arguments like `slice(1, 3)` 1 to 2 index. If the end argument is omitted, like in the first examples, the `slice()` method slices out the rest of the array.

### Sorting an Array

The `sort()` method sorts an array alphabetically **assending** order.

```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.sort();
console.log(fruits); //Apple,Banana,Mango,Orange
```

### Reversing an Array

By combining `sort()` and `reverse()` you can sort an array in **descending** order.

```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.sort();
fruits.reverse();
console.log(fruits); // Orange,Mango,Banana,Apple
```

### Numeric Sort

By default, the `sort()` function sorts values as **strings**.This works well for strings ("Apple" comes before "Banana").However, if numbers are sorted as strings, "25" is bigger than "100", because "2" is bigger than "1".Because of this, the `sort()` method will produce incorrect result when sorting numbers.

You can fix this by providing a **compare function**:

```javascript
const points = [40, 100, 1, 5, 25, 10];
points.sort(function(a, b){return a - b}); //Assending order
console.log(points); // 1,5,10,25,40,100

const points = [40, 100, 1, 5, 25, 10];
points.sort(function(a, b){return b - a}); // Dessending order
console.log(points); //100,40,25,10,5,1
```

**Working of Numeric sorting:**

When the `sort()` function compares two values, it sends the values to the compare function, and sorts the values according to the returned (negative, zero, positive) value.

If the result is **negative**, `a` is sorted before `b`.

If the result is **positive**, `b` is sorted before `a`.

If the result is 0, no changes are done with the sort order of the two values.

### Sorting an Array in Random Order

```javascript
const points = [40, 100, 1, 5, 25, 10];
points.sort(function(){return 0.5 - Math.random()});
```

### Find the Highest (or Lowest) Array Value

There are no built-in functions for finding the **max** or **min** value in an array. After you have sorted an array, you can use the 0th index to obtain the lowest value . If we want highist use `points[points.length-1]` .

### Math.max()

You can use `Math.max.apply` to find the highest number in an array.

```javascript
function myArrayMax(arr) {
  return Math.max.apply(null, arr);
}

// Tradisonal method
// function loops through an array comparing each value with the highest //value found.
function myArrayMax(arr) {
  let len = arr.length;
  let max = -Infinity;
  while (len--) {
    if (arr[len] > max) {
      max = arr[len];
    }
  }
  return max;
}
```

### Math.min()

```javascript
function myArrayMin(arr) {
  return Math.min.apply(null, arr);
}

// Tradisonal method
//function loops through an array comparing each value with the lowest value //found.
function myArrayMin(arr) {
  let len = arr.length;
  let min = Infinity;
  while (len--) {
    if (arr[len] < min) {
      min = arr[len];
    }
  }
  return min;
}
```

### Sorting Object Arrays

```javascript
const cars = [
  {type:"Volvo", year:2016},
  {type:"Saab", year:2001},
  {type:"BMW", year:2010}
];
```

Even if objects have properties of different data types, the `sort()` method can be used to sort the array.

```javascript
cars.sort(function(a, b){return a.year - b.year}); //object so we access values by using dot(.).
```

### Stable Array sort()

```javascript
const myArr = [
  {name:"X00",price:100 },
  {name:"X01",price:100 },
  {name:"X02",price:100 },
  {name:"X03",price:100 },
  {name:"X04",price:110 },
  {name:"X05",price:110 },
  {name:"X06",price:110 },
  {name:"X07",price:110 },
  {name:"X08",price:120 },
  {name:"X09",price:120 },
  {name:"X10",price:120 },
  {name:"X11",price:120 },
  {name:"X12",price:130 },
  {name:"X13",price:130 },
  {name:"X14",price:130 },
  {name:"X15",price:130 },
  {name:"X16",price:140 },
  {name:"X17",price:140 },
  {name:"X18",price:140 },
  {name:"X19",price:140 }
];

myArr.sort( (p1, p2) => {
  if (p1.price < p2.price) return -1; // if p1 is less than p2 we return -1.
  if (p1.price > p2.price) return 1;
  return 0;
});

let txt = "";
myArr.forEach(myFunction);

function myFunction(value) {
  txt += value.name + " " + value.price + "<br>"; 
}
document.getElementById("demo").innerHTML = txt;
```

### Array forEach()

The `forEach()` method calls a function (a callback function) once for each array element. Calls a function once for each array element.

```javascript
const numbers = [45, 4, 9, 16, 25];
let txt = "";
numbers.forEach(myFunction);

function myFunction(value, index, array) { // index and array are opctional
  txt += value + "<br>"; 
//45 4 9 16 25
}
```

### Array map()

The `map()` method creates a **new array** by performing a function **on each array element**. The `map()` method does **not change the original array**.The `map()` method does not execute the function for array elements without values.

```javascript
const numbers1 = [45, 4, 9, 16, 25];
const numbers2 = numbers1.map(myFunction);

function myFunction(value) {
  return value * 2;
}
```

### Array flatMap()

The `flatMap()` method first maps **all elements** of an array and then creates a new array by flattening the array.

```javascript
const myArr = [1, 2, 3, 4, 5,6];
const newArr = myArr.flatMap((x) => x * 2); //2,4,6,8,10,12
```

### Array filter()

`filter()` method creates a **new array** with array elements that pass a test.

```javascript
const numbers = [45, 4, 9, 16, 25];
const over18 = numbers.filter(myFunction);

document.getElementById("demo").innerHTML = over18;

function myFunction(value, index, array) {
  return value > 18; // 45 25
```

### Array reduce()

The `reduce()` method runs a function on each array element to produce (reduce it to) a single value(total).

```javascript
const numbers = [45, 4, 9, 16, 25];
let sum = numbers.reduce(myFunction);

function myFunction(total, value, index, array) {
  return total + value; //99 total
//The total (the initial value / previously returned value)
//The item value
//The item index
//The array itself
}

//The reduce() method can accept an initial value:
const numbers = [45, 4, 9, 16, 25];
let sum = numbers.reduceRight(myFunction, 100); // we can also use reduceRight()

function myFunction(total, value) {
  return total + value; // 199 total
}
```

### Array every()

It checks all the values are pass the test if pass returns True else False.

```javascript
const numbers = [45, 4, 9, 16, 25];
let allOver18 = numbers.every(myFunction);
                          //(opctional)
function myFunction(value, index, array) {
  return value > 18; //  False
}
```

### Array some()

Checks the some elements are pass the test.

```javascript
const numbers = [45, 4, 9, 16, 25];
let someOver18 = numbers.some(myFunction);

function myFunction(value, index, array) {
  return value > 18; //  True
}
```

### Array indexOf()

The `indexOf()` method searches a value in array and returns its position(index).

***Syntax:*** *array*.indexOf(*item*, *start*). `Array.indexOf()` returns -1 if the item is not found.

```javascript
const fruits = ["Apple", "Orange", "Apple", "Mango"];
let position = fruits.indexOf("Apple") + 1; // index is 0 , Position is 1
```

### Array lastIndexOf()

It is same as the `IndexOf()` but it returns last index.

### Array find()

The `find()` method returns the value of the first array element that passes a test function.

This example finds (returns the value of) the first element that is larger than 18.

```javascript
const numbers = [4, 9, 16, 25, 29];
let first = numbers.find(myFunction);

function myFunction(value, index, array) {
  return value > 18; // 25
}
```

### findIndex()

The `findIndex()` method returns the index of the first array element that passes a test function.

```javascript
const numbers = [4, 9, 16, 25, 29];
let first = numbers.findIndex(myFunction);

function myFunction(value, index, array) {
  return value > 18; // 3
}
```

### Array.from()

The `Array.from()` method returns an **Array object** from any object with a length property or any iterable object.

```javascript
const myArr = Array.from("ABCDEFG");
document.getElementById("demo").innerHTML = myArr; // A,B,C,D,E,F,G
```

### Array Keys()

The `Array.keys()` method returns an **Array Iterator object with the keys** of an array.

```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
const keys = fruits.keys();

let text = "";
for (let x of keys) {
  text += x + "<br>";
}

document.getElementById("demo").innerHTML = text;// 0 1 2 3
```

### Array entries()

The `entries()` method returns an **Array Iterator object** with **key/value pairs**.

```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
const f = fruits.entries();

for (let x of f) {
  document.getElementById("demo").innerHTML += x;
}
// [0, "Banana"]
//[1, "Orange"]
//[2, "Apple"]
//[3, "Mango"]
```

### Array includes()

This allows us to check if an element is present in an array.

```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];

fruits.includes("Mango"); // is true
```

### Const keyword

The keyword `const` is a little misleading.

It does **NOT define a constant array**. It defines a **constant reference** to an array.

Because of this, we can **still change the elements** of a constant array.

An array declared with `const` **must** be **initialized** when it is declared.

```javascript
const cars = ["Saab", "Volvo", "BMW"];
cars = ["Toyota", "Volvo", "Audi"];    // ERROR you cannot assign new reference to const.

// You can create a constant array:
const cars = ["Saab", "Volvo", "BMW"];
// You can change an element:
cars[0] = "Toyota";
// You can add an element:
cars.push("Audi");
```

### Const Block Scope

An array declared with `const` has **Block Scope**.

An array declared in a block is **not the same** as an array declared outside the block:

An array declared with `var` does not have block scope.

```javascript
const cars = ["Saab", "Volvo", "BMW"];
// Here cars[0] is "Saab"
{
  const cars = ["Toyota", "Volvo", "BMW"];
  // Here cars[0] is "Toyota"
}
// Here cars[0] is "Saab"
```

### Redeclaring Arrays

Redeclaring an array declared with `var` is allowed anywhere in a program.

```javascript
var cars = ["Volvo", "BMW"];   // Allowed
var cars = ["Toyota", "BMW"];  // Allowed
cars = ["Volvo", "Saab"];      // Allowed
```

Redeclaring or reassigning an array to `const`, in the same scope, or in the same block, is not allowed.

```javascript
var cars = ["Volvo", "BMW"];     // Allowed
const cars = ["Volvo", "BMW"];   // Not allowed
{
  var cars = ["Volvo", "BMW"];   // Allowed
  const cars = ["Volvo", "BMW"]; // Not allowed
}

//Redeclaring or reassigning an existing const array, in the same scope, or in the same block, is not allowed
const cars = ["Volvo", "BMW"];   // Allowed
const cars = ["Volvo", "BMW"];   // Not allowed
var cars = ["Volvo", "BMW"];     // Not allowed
cars = ["Volvo", "BMW"];         // Not allowed

{
  const cars = ["Volvo", "BMW"]; // Allowed
  const cars = ["Volvo", "BMW"]; // Not allowed
  var cars = ["Volvo", "BMW"];   // Not allowed
  cars = ["Volvo", "BMW"];       // Not allowed
}

//Redeclaring an array with const, in another scope, or in another block, is allowed:
const cars = ["Volvo", "BMW"];   // Allowed
{
  const cars = ["Volvo", "BMW"]; // Allowed
}
{
  const cars = ["Volvo", "BMW"]; // Allowed
}
```