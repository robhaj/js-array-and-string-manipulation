# Array and String Methods in JavaScript

## Manipulating Arrays
### Arrays
- JavaScript arrays are used to store multiple values in a single variable

- An array can hold many values under a single name, and you can access the values by referring to an index number.

- Array indexes start at 0, the first element in the array is index position 0.

### Array Methods
#### .pop()
The pop() method removes the last element from an array and returns that element. This method is destructive and modifies the array. If you call pop() on an empty array, it returns an undefined value.

###### Syntax
```js
var arr = ['duck', 'duck', 'goose'];

arr.pop()
> 'goose'

console.log(arr)
> ['duck', 'duck']

arr = [];

arr.pop()
> undefined
```
#### .push()
The push() method adds one or more elements to the end of an array and returns the new length of the array. This is also destructive and alters the array on which the method was called.

###### Syntax
```js
var arr = ['spoon', 'fork', 'knife'];

arr.push('napkin')
> 4

console.log(arr)
> ['spoon', 'fork', 'knife', 'napkin']

arr.push('plate','bowl')
> 6

console.log(arr)
> ['spoon', 'fork', 'knife', 'napkin', 'plate', 'bowl']
```
#### .shift()
The shift() method is like the pop() method, only it works at the beginning of the array. It removes the first element from an array and returns that element. This method is destructive and changes the length of the array.

###### Syntax
```js
var arr = ['potato', 'blue', 'white', 'green'];

arr.shift()
> 'potato'

console.log(arr)
> ['blue', 'white', 'green']
```

#### .unshift()
The unshift() method is like the push() method, only it works at the beginning of the array.
Adds one or more elements to the front of an array and returns the new length of the array.

###### Syntax
```js
var arr = ['Wes', 'Michael', 'Zach'];

arr.unshift('Robby', 'Bradley')
> 5

console.log(arr)
> ['Robby', 'Bradley', 'Wes', 'Michael', 'Zach']

```
#### .splice()
Adds and/or removes elements from an array.

Arguments
- start - Index at which to start changing the array.
- deleteCount - An integer indicating the number of old array elements to remove.

###### Syntax
```js
var arr = ['Robby', 'Bradley', 'Wes', 'Michael', 'Zach'];

arr.splice(1, 1)
> ['Bradley']

console.log(arr)
> ['Robby', 'Wes', 'Michael', 'Zach']

arr.splice(2, 3)
> ['Michael','Zach']

console.log(arr);
> ['Robby', 'Wes']

arr.splice(1)
> ['Wes']

console.log(arr);
> ['Robby']
```
#### .slice()
Extracts a section of an array and returns a new array. This is not destructive as the original array remains unchanged.

 Arguments
- begin - Index at which to begin extraction.

<!-- If begin is omitted, slice begins from index 0.
if begin === null, slice begins from 0 -->

- end -  Index at which to end extraction. slice extracts up to but not including end. If end is omitted, slice extracts to the end of the sequence (arr.length).

###### Syntax
```js
var arr = ['Robby', 'Bradley', 'Wes', 'Michael', 'Zach'];

arr.slice(4)
> ['Zach']

console.log(arr)
>['Robby', 'Bradley', 'Wes', 'Michael', 'Zach']

arr.slice(2, 4)
> ['Wes','Michael']

console.log(arr)
>['Robby', 'Bradley', 'Wes', 'Michael', 'Zach']
```

#### .sort()
Sorts the elements of an array in place and returns the array. If no compare function is passed as an argument it is sorted according to each character's Unicode code point value, according to the string conversion of each element. This is why just calling .sort() will not order numbers logically but rather their Unicode value.

###### Syntax
```js
var arr = ['Robby', 'Bradley', 'Wes', 'Michael', 'Zach'];

arr.sort()
> ['Bradley', 'Michael', 'Robby', 'Wes', 'Zach']

arr = [5,2,3,4,1]

> [1, 2, 3, 4, 5]

arr = [15,7,22,5,91]

arr.sort()
> [15, 22, 5, 7, 91]
```
#### .concat()
Returns a new array comprised of this array joined with other array(s) and/or value(s).

###### Syntax
```js
var arr1 = ['Mercury', 'Venus', 'Earth', 'Mars'];
var arr2 = ['Jupiter','Saturn','Uranus','Neptune'];

arr1.concat(arr2)
> ['Mercury','Venus','Earth','Mars','Jupiter','Saturn','Uranus','Neptune' ]
```
#### .join()
Joins all elements of an array into a string.

###### Syntax
```js
var arr = ['The','quick','brown','fox','jumped','over','the','lazy','dog'];

arr.join()
> 'The,quick,brown,fox,jumped,over,the,lazy,dog'
```

<hr>

## Manipulating Strings
### Strings
- A JavaScript string stores a series of characters like "John Doe".

- String indexes are zero-based: The first character is in position 0, the second in 1, and so on.

### String Methods

#### .concat()
Joins two or more strings, and returns a new joined strings

###### Syntax
.concat()

#### .toUpperCase()
Converts a string to uppercase letters

###### Syntax
.toUpperCase()

#### .toLowerCase()
Converts a string to lowercase letters

###### Syntax
.toLowerCase()

#### .charAt()
Returns the character at the specified index

#### .slice()
Extracts a part of a string and returns a new string

###### Syntax
.slice()

#### .split()
Splits a string into an array of substrings

###### Syntax
.split()

#### .trim()
Removes whitespace from both ends of a string

###### Syntax
.trim()
