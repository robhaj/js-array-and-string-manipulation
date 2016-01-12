###Section 1

For the first set of questions, use the given methods to modify the top array so that it reads the same as the one underneath. console log the array to make sure it has been changed.

Using ```.pop()``` :

```js
  var nums = ['one', 'two', 'three', 'four', 'ten']

  ans => ['one', 'two', 'three', 'four']
```

Using ```.push()``` :

```js
  var letters = ['a', 'b', 'c', 'd']

  ans => ['a', 'b', 'c', 'd', 'e']
```

Using ```.shift()``` :

```js
  var vehicles = ['lollipop', 'car', 'truck', 'tank']

  ans => ['car', 'truck', 'tank']
```

Using ```.unshift()``` :

 ```js
  var sports = ['football', 'baseball', 'hockey']

  ans => ['rugby', 'football', 'baseball', 'hockey']
```

Using ```.splice()``` :

```js
  var years = [1990, 2015, 1066, 43, 90, 1607]

  ans => [1990, 2015, 1607]

  var movies = ['The Great Escape', 'Love Actually', 'Blade Runner', 'Indiana Jones and the Last Crusade']

  ans => ['The Great Escape', 'Blade Runner', 'Indiana Jones and the Last Crusade']
```

Using ```.sort()``` :

```js
  var greekLetters = ['beta', 'gamma', 'alpha', 'epsilon', 'delta']

  ans => ['alpha', 'beta', 'delta', 'epsilon', 'gamma']
```

###Section 2

For the next set of questions, simply return the answer. The original array/arrays should not be modified.

Using ```.slice()```

```js
  var animals = ['dog', 'cat', 'eagle', 'cow']

  ans => ['cat']

  var names = ['jeff', 'tony', 'tabitha', 'annie', 'edward', 'james']

  ans => ['annie', 'edward', 'james']
```

Using ```.concat()``` :

```js
  var firstNums = [1, 2, 3]

  var secondNums = [4, 5, 6]

  ans => [1, 2, 3, 4, 5, 6]
```

Using ```.join()``` :

```js
  var arr = ['Bradley', 'is', 'super', 'amazing']

  ans => 'Bradley is super amazing'
```

###Section 3

Next, use the string methods given to return the ans underneath

Using ```.concat()``` :

```js
  var str1 = 'Javascript is really '

  var str2 = 'really really great!'

  ans => 'Javascript is really really really great'
```

Using ```.toUpperCase()```


```js
  var talk = 'Now I\'m Shouting'

  ans => 'NOW I\'M SHOUTING'
```

Using ```.toLowerCase()``` :

```js
  var shout = 'EVERYONE BE QUIET'

  ans => 'everyone be quiet'
```

Using ```.charAt()``` :

```js
  var string = 'Super Amazing Stuff'

  ans => 'z'
```

Using ```.slice()``` :

```js
  var fullTitle = 'Lord Edward Swivington the 3rd'

  ans => 'Edward Swivington'
```

Using ```.split()``` :

```js
  var year = '1990'

  ans => ['1', '9', '9', '0']

  var quote = 'Why did it have to be snakes?'

  ans => ['Why', 'did', 'it', 'have', 'to', 'be', 'snakes?']
```

Using ```.trim()``` :

```js
  var lyric = '    Here I am. ROCK you like a hurricane.      '

  ans => 'Here I am. ROCK you like a hurricane.'
```

###Section 4

1. Write a function that will find the index of all the "o"s in "Oy! I am a normal string!" regardless of case.

1. Write a function which accepts a number as input and inserts dashes (-) between every two numbers. For example if you accept 025468 the output should be 02-54-68

1. Write a function to remove every item in an array that is not a number.

1. Write a JavaScript function to get a random item from an array.

1. Write a function that will take in a string and returns that same string in reverse.

1. Write a JavaScript function that reverse a number e.g.
```js
Example x = 32243;
Expected Output : 34223
```

1. Write a JavaScript function that takes in a string and returns it with letters in alphabetical order

1. Write a JavaScript function that accepts a string as a parameter and find the longest word within the string.
```js
Example string = 'Web Development Tutorial'
Expected Output => 'Development'
```

1. Write a function to add up all the numbers in any given year. The year will be given as a string, the output should be a number. For example the input ```'1470'``` should give ```12```

1. Write a function that will take in an array of full names, and only return the first name of each person. For example ```['Bradley Bouley', 'Robert Hajek']``` should return ```['Bradley', 'Robert']```

1. Write a JavaScript program which accepts a string as input and swap the case of each character. For example if you input ```'The Quick Brown Fox'``` the output should be ```'tHE qUICK bROWN fOX'```.

1. Write a JavaScript function to merge two arrays and removes all duplicates elements. e.g.
```js
var array1 = [1, 2, 3];
var array2 = [2, 30, 1];
console.log(merge_array(array1, array2));
[3, 2, 30, 1]
```
