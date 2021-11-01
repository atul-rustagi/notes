# Learning Javascript

### Contents

1. [Refer elements from HTML](#refer-elements-from-html)
2. [Difference between var, let and const](#difference-between-var-let-and-const)
3. [Local Storage vs Session Storage vs Cookies](#local-storage-vs-session-storage-vs-cookies)

---

### Refer elements from HTML

* Class Elements
```javascript
var elements = document.getElementsByClassName ('class');
```

* Id Element
```javascript
var element = document.getElementById ('id');
```

* HTML Tag
```javascript
var elements = document.getElementsByTagName ('tag');
```

* CSS Selector
```javascript
var elements = document.querySelectorAll ('css selector');

var element = document.querySelectorAll ('css selector')[i];

var element = document.querySelector ('css selector');
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
