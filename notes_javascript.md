# Learning Javascript

### Contents

1. [Refer elements from HTML](#refer-elements-from-html)
2. [Difference between var, let and const](#difference-between-var-let-and-const)
3. [Local Storage vs Session Storage vs Cookies](#local-storage-vs-session-storage-vs-cookies)
4. [Strings in Javascript](#strings-in-javascript)
5. [Arrays in Javascript](#arrays-in-javascript)

---

### Refer elements from HTML

* Class Elements
```javascript
let elements = document.getElementsByClassName ('class');
```

* Id Element
```javascript
let element = document.getElementById ('id');
```

* HTML Tag
```javascript
let elements = document.getElementsByTagName ('tag');
```

* CSS Selector
```javascript
let elements = document.querySelectorAll ('css selector');

let element = document.querySelectorAll ('css selector')[i];

let element = document.querySelector ('css selector');
```

---

### Difference between var, let and const

> [Var, Let, and Const in Javascript](https://medium.com/nerd-for-tech/var-let-and-const-in-javascript-15e41cf90f01 "Var, Let, Const in Javascript")

> [Var, Let, and Const – What's the Difference?](https://www.freecodecamp.org/news/var-let-and-const-whats-the-difference "Var, Let, and Const – What's the Difference?")

|                    | Var                  | Let   | Const |
|--------------------|:--------------------:|:-----:|:-----:|
| __Scope__          | Global or Functional | Block | Block |
| __Re-declaration__ | __✓__                | X     | X     |
| __Updation__       | __✓__                | __✓__ | X     |
| __Initialization__ | default __undefined__| X     | X     |
| __Declaration__    | X                    | X     | must be __initialized__ |

---

### Local Storage vs Session Storage vs Cookies

> [Storages](https://stackoverflow.com/questions/19867599/what-is-the-difference-between-localstorage-sessionstorage-session-and-cookies "Difference between localStorage, sessionStorage, and cookies")

* Getting items from Local Storage
```javascript
let item = localStorage.getItem ("key");
```

* Converting string received from Local Storage to array
```javascript
let value = JSON.parse (item);
```

* Setting items to Local Storage
```javascript
localStorage.setItem ("key", item);
```
* Converting array to string for local storage
```javascript
let item = JSON.stringify (value);
```

---

### Strings in Javascript

* String length
```javascript
let str = "Some text here";

let len = str.length; // reutrns length of str
```

* Uppercase
```javascript
str.toUpperCase ();
```

* Lowercase
```javascript
str.toLowerCase ();
```

* Indexing
```javascript
str.indexOf ('t'); // returns 1st occurance of 't' else -1

str.lastIndexOf ('t'); // returns last occurance of 't' else -1

str.charAt (n); // returns char at nth index of 0-based index string
```

* Substring
```javascript
str.substring (m, n); // returns str from m to n-1 index
str.substring (n); // returns str from nth to last index

str.slice (m, n); // same as substring
str.slice (n); // if n is negative then returns last n char else same as substring
```

* Other
```javascript
str.endsWith (text); // checks if str ends with text

str.includes (text); // checks if str includes text

str.split (delimiter); // returns array for string splitted over delimiter
```

---

### Arrays in Javascript

* Push and Pop
```javascript
const arr = [23, 43, 64, 12, 93, 20];

arr.push (num); // push element at end of array

arr.pop (); // pop element from end of array
```

* Unshift and Shift
```javascript
arr.unshift (num); // push element at front of array

arr.shift (); // pop element from front of array
```

* Splice
```javascript
arr.splice (m, n); // removes n elements from index m (inclusive)
```

* Other
```javascript
arr.reverse () // reverse the array
```
