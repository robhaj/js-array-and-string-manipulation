# Array, String, Object, and Number Methods in JavaScript

## Manipulating Arrays
### Arrays
- JavaScript arrays are used to store multiple values in a single variable

- An array can hold many values under a single name, and you can access the values by referring to an index number.

- Array indexes start at 0, the first element in the array is index position 0.

### Some Array Methods

- [.pop()](https://github.com/robhaj/js-array-and-string-manipulation#pop)
- [.push()](https://github.com/robhaj/js-array-and-string-manipulation#push)
- [.shift()](https://github.com/robhaj/js-array-and-string-manipulation#shift)
- [.unshift()](https://github.com/robhaj/js-array-and-string-manipulation#unshift)
- [.splice()](https://github.com/robhaj/js-array-and-string-manipulation#splicestart-deletecount-item1-item2-)
- [.slice()](https://github.com/robhaj/js-array-and-string-manipulation#slicebegin-end)
- [.sort()](https://github.com/robhaj/js-array-and-string-manipulation#sortcomparefunction)
- [.concat()](https://github.com/robhaj/js-array-and-string-manipulation#concatvalue1-value2--valuen)
- [.join()](https://github.com/robhaj/js-array-and-string-manipulation#joinseperator)


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
#### .splice(start, deleteCount[, item1[, item2[, ...]]])

Adds and/or removes elements from an array.

Arguments
- start - Index at which to start changing the array. If greater than the length of the array, actual starting index will be set to the length of the array. If negative, will begin that many elements from the end.
- deleteCount - An integer indicating the number of old array elements to remove. If deleteCount is 0, no elements are removed. In this case, you should specify at least one new element. If deleteCount is greater than the number of elements left in the array starting at start, then all of the elements through the end of the array will be deleted. If deleteCount is omitted, deleteCount will be equal to (arr.length - start).
- itemN - The element to add to the array. If you don't specify any elements, splice() will only remove elements from the array.

###### Syntax
```js
var arr = ['Robby', 'Bradley', 'Wes', 'Michael', 'Zach'];

arr.splice(1, 1)
> ['Bradley']

console.log(arr)
> ['Robby', 'Wes', 'Michael', 'Zach']

arr.splice(2, 3)
> ['Michael','Zach']

console.log(arr)
> ['Robby', 'Wes']

arr.splice(1)
> ['Wes']

console.log(arr)
> ['Robby']
```
#### .slice(begin, end)
Extracts a section of an array and returns a new array. This is not destructive as the original array remains unchanged.

 Arguments
- begin - Index at which to begin extraction. If begin is omitted || === null, slice begins from index 0.

- end -  Index at which to end extraction. Slice extracts up to but not including end. If end is omitted, slice extracts to the end of the sequence (arr.length).

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

#### .sort(compareFunction)
Sorts the elements of an array in place and returns the array. It has an optional argument which is a function to define the sort order. If no compare function is passed as an argument it is sorted according to each character's Unicode code point value, according to the string conversion of each element. This is why just calling .sort() will not order numbers logically but rather their Unicode value.

Arguments
- compareFunction (Optional) Specifies a function that defines the sort order. If omitted, the array is sorted according to each character's Unicode code point value, according to the string conversion of each element.

###### Syntax
```js
var arr = ['Robby', 'Bradley', 'Wes', 'Michael', 'Zach'];

arr.sort()
> ['Bradley', 'Michael', 'Robby', 'Wes', 'Zach']

console.log(arr)
> ['Bradley', 'Michael', 'Robby', 'Wes', 'Zach']

arr = [5, 2, 3, 4 ,1]

arr.sort()
> [1, 2, 3, 4, 5]

arr = [15, 7, 22, 5, 91]

arr.sort()
> [15, 22, 5, 7, 91]
```
#### .concat(value1[, value2[, ...[, valueN]]])
Returns a new array comprised of this array joined with other array(s) and/or value(s).

Parameters
- valueN - Arrays and/or values to concatenate into a new array. See the description below for details.

###### Syntax
```js
var arr1 = ['Mercury', 'Venus', 'Earth', 'Mars'];
var arr2 = ['Jupiter','Saturn','Uranus','Neptune'];
var str = 'Pluto';

var arr3 = arr1.concat(arr2)
console.log(arr3)
> ['Mercury','Venus','Earth','Mars','Jupiter','Saturn','Uranus','Neptune']

arr3.concat(str)
> ['Mercury','Venus','Earth','Mars','Jupiter','Saturn','Uranus','Neptune','Pluto']

```
#### .join(seperator)
Joins all elements of an array into a string. Takes an optional argument to specify a string to seperate each element.

Arguments
- separator (optional)
Specifies a string to separate each element of the array. The separator is converted to a string if necessary. If omitted, the array elements are separated with a comma. If separator is an empty string, all elements are joined without any characters in between them.

###### Syntax

```js
var arr = ['The','quick','brown','fox','jumped','over','the','lazy','dog'];

arr.join(' ')
> 'The quick brown fox jumped over the lazy dog'

arr.join()
> 'The,quick,brown,fox,jumped,over,the,lazy,dog'

arr.join('')
> 'Thequickbrownfoxjumpedoverthelazydog'
```

#### .indexOf(item,start)

The indexOf() method searches the array for the specified item, and returns its position.

The search will start at the specified position, or at the beginning if no start position is specified, and end the search at the end of the array.

Returns -1 if the item is not found.

If the item is present more than once, the indexOf method returns the position of the first occurrence.

Parameters
- item - The item to search for.
- start (optional) - Where to start the search. Negative values will start at the given position counting from the end, and search to the end.

###### Syntax

```js
var fruits = ["Banana", "Orange", "Apple", "Mango"];

console.log(fruits.indexOf("Apple"))
> 2

var fruits = ["Banana", "Orange", "Apple", "Mango", "Banana", "Orange", "Apple"];

console.log(fruits.indexOf("Apple", 4))
> 6
```
<hr>

## Manipulating Strings
### Strings
- A JavaScript string stores a series of characters like "John Doe".

- String indexes are zero-based: The first character is in position 0, the second in 1, and so on.

### Some String Methods

- [.concat()](https://github.com/robhaj/js-array-and-string-manipulation#concatstring2stringn)
- [.toUpperCase()](https://github.com/robhaj/js-array-and-string-manipulation#touppercase)
- [.toLowerCase()](https://github.com/robhaj/js-array-and-string-manipulation#tolowercase)
- [.charAt()](https://github.com/robhaj/js-array-and-string-manipulation#charatindex)
- [.slice()](https://github.com/robhaj/js-array-and-string-manipulation#slicebeginslice-endslice)
- [.split()](https://github.com/robhaj/js-array-and-string-manipulation#splitseperator-limit)
- [.trim()](https://github.com/robhaj/js-array-and-string-manipulation#trim)
- [.replace()](https://github.com/robhaj/js-array-and-string-manipulation#replaceregexpsubstr-newsubstrfunction-flags)

#### .concat(string2...stringN)
Joins two or more strings, and returns a new joined strings. Alternatively you can use the arithmetic operator, +.

Parameters
- Strings to concatenate to this string.

###### Syntax
```js
var str1 = "Hello ";
var str2 = "world!";
var str3 = " Have a nice day!";

str1.concat(str2,str3)
> 'Hello world! Have a nice day!'

console.log(str1 + str2 + str3)
> 'Hello world! Have a nice day!'
```
#### .toUpperCase()
Converts a string to uppercase letters

###### Syntax
```js
var str = 'lol';

str.toUpperCase()
> 'LOL'
```
#### .toLowerCase()
Converts a string to lowercase letters

###### Syntax
```js
var str = 'HELLO WORLD!';

str.toLowerCase()
> 'hello world!'
```
#### .charAt(index)
Returns the character at the specified index. Takes an index as a parameter.

Parameters
- Index

###### Syntax
```js
var str = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ';

str.charAt()
> 'A'
str.charAt(0)
> 'A'
str.charAt(25)
> 'Z'
```
#### .slice(beginSlice, endSlice)
Extracts a part of a string and returns a new string. Takes two parameters: the index at which to begin slicing and optionally an index at which to end slicing.

Parameters
- beginSlice - The zero-based index at which to begin extraction. If negative, it is treated as sourceLength + beginSlice where sourceLength is the length of the string (for example, if beginSlice is -3 it is treated as sourceLength - 3).
- endSlice (Optional) - The zero-based index at which to end extraction. If omitted, slice() extracts to the end of the string. If negative, it is treated as sourceLength + endSlice where sourceLength is the length of the string (for example, if endSlice is -3 it is treated as sourceLength - 3).


###### Syntax

```js
var str = 'Slice the fruits - Banana, Orange, Apple'

str.slice(19)
> 'Banana, Orange, Apple'

str.slice(19, 25)
> 'Banana'

str.slice(27, 33)
> 'Orange'

str.slice(35, 40)
> 'Apple'
```

#### .split(seperator, limit)
Splits a string into an array of substrings. Takes two optional parameters to set the seperator and/or limit of splits.

Parameters

- Seperator (optional) Specifies the character(s) to use for separating the string. The separator is treated as a string or a regular expression. If separator is omitted, the array returned contains one element consisting of the entire string. If separator is an empty string, str is converted to an array of characters.
- Limit (optional) Integer specifying a limit on the number of splits to be found. The split() method still splits on every match of separator, but it truncates the returned array to at most limit elements.

###### Syntax
```js
var str = '1062 Delaware St. Denver CO, 80204';

str.split('.')
> ['1062 Delaware St', ' Denver CO, 80204']
```
#### .trim()
Removes whitespace from both ends of a string

###### Syntax
```js
var str = ' 1-800-867-5309   ';

str.trim()
> '1-800-867-5309'
```

#### .replace(regexp|substr, newSubStr|function[, flags])

Parameters

- regexp (pattern) - A RegExp object. The match is replaced by the return value of parameter #2.
- substr (pattern) - A String that is to be replaced by newSubStr. It is treated as a verbatim string and is not interpreted as a regular expression.
- newSubStr (replacement) - The String that replaces the substring received from parameter #1.
- function (replacement) - A function to be invoked to create the new substring (to put in place of the substring received from parameter #1)


###### Syntax
```js
var str = "Michael Herman!";
var res = str.replace("Michael", "DonutsMcCookie");

console.log(res)
> "DonutsMcCookie Herman"
```

## Manipulating numbers

### Numbers

- JavaScript has only one type of number.
- Unlike many other programming languages, JavaScript does not define different types of numbers, like integers, short, long, floating-point etc.
- JavaScript numbers can be written with, or without decimals:
- NaN is a JavaScript reserved word indicating that a value is not a number.


#### parseInt()

Parses its argument and returns an integer

###### Syntax

```js
var str = '5.66';
var num = parseInt(str);

console.log(num)
> 5

console.log(typeof num)
> 'number'

```

#### parseFloat()

Parses its argument and returns a floating point number


###### Syntax

```js
var str = '5.666667';
var num = parseFloat(str);

console.log(num)
> 5.666667

console.log(typeof num)
> 'number'

console.log(+str)
> 5.666667
```

## Manipulating Objects

### Objects

In JavaScript, almost "everything" is an object.

- Booleans can be objects (or primitive data treated as objects)
- Numbers can be objects (or primitive data treated as objects)
- Strings can be objects (or primitive data treated as objects)
- Dates are always objects
- Maths are always objects
- Regular expressions are always objects
- Arrays are always objects
- Functions are always objects
- Objects are objects
Basically, in Javascript, all values except primitive values are objects.

#### for...in loop
- Iterates over the properties of an object and can be used to return either one of the key value pairs at that point in the object.
- You should only use a ```for...in``` loop when iterating over an object, although it can be used for arrays as well, you should use a ```for``` loop with a numeric index

###### Syntax
```js
var obj = { a:'alpha', b:'beta', c:'gamma' };

for (var prop in obj) {
  console.log("obj." + prop + " = " + obj[prop]);
}

// Output:
// "obj.a = alpha"
// "obj.b = beta"
// "obj.c = gamma"
```
