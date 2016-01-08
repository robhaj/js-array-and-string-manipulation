# Array and String Methods in JavaScript

## Manipulating Arrays
### Arrays
- JavaScript arrays are used to store multiple values in a single variable

- An array can hold many values under a single name, and you can access the values by referring to an index number.

### Array Methods
#### .pop()
The pop() method removes the last element from an array and returns that element.

###### Syntax
```js
var arr = ['duck', 'duck', 'goose'];
arr.pop()

> 'goose'
```
#### .push()
The push() method adds one or more elements to the end of an array and returns the new length of the array.

###### Syntax
```js
var arr = ['spoon', 'fork', 'knife'];
arr.push('napkin')

> 4

console.log(arr)

> ['spoon', 'fork', 'knife', 'napkin']
```
#### .shift()
The shift() method removes the first element from an array and returns that element. This method changes the length of the array.

###### Syntax
```js
var arr = ['potato', 'blue', 'white', 'green']
arr.shift()

> 'potato'

console.log(arr)

> ['blue', 'white', 'green']
```

#### .unshift()
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
var arr = ['Robby', 'Bradley', 'Wes', 'Michael', 'Zach']
arr.splice(1, 1)

> ['Bradley']

arr.splice(2, 3)

> ['Wes','Michael','Zach']
```
#### .slice()
Extracts a section of an array and returns a new array.

 Arguments
- begin - Index at which to begin extraction. If begin is omitted, slice begins from index 0.
- end -  Index at which to end extraction. slice extracts up to but not including end. If end is omitted, slice extracts to the end of the sequence (arr.length).

###### Syntax
```js
var arr = ['Robby', 'Bradley', 'Wes', 'Michael', 'Zach']
arr.slice(4)

> ['Zach']

arr.slice(2, 4)

> ['Wes','Michael']
```

#### .sort()
Sorts the elements of an array in place and returns the array.

###### Syntax
.sort()

#### .concat()
Returns a new array comprised of this array joined with other array(s) and/or value(s).

###### Syntax
.concat()

#### .join()
Joins all elements of an array into a string.

###### Syntax
.join()




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
