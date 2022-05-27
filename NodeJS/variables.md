<h1>We have e types of variables that we can use in JS.</h1> <br>

<h2> Var </h2>
The first one is the var, the important thing about var is that we can start using var before declare it, so we can do like this <br>

```
var first = 'hello';
var second = 'world.';

phrase = first + ' ' + second;
console.log(phrase);
var phrase;
```
If we declare one var inside of a function we can use it in all code, the same didn't happened in others (let and const) <br>
But one big problem is that we can have more than 1 variable with the same name when we used var.

<h2> Let </h2>
The use of Let is little bit different than var.<br>
Different of Var, we just can use Let before we declare it.

```
let first = 'hello';
let second = 'world.';
let phrase;

phrase = first + ' ' + second;
console.log(phrase);
```

So we cant have more than one variable with the same name using let.

<h2> Const </h2>

We can't initialize without a value, so we have to set a value in the initialize of this variable.


```
const first = 'hello';
const second = 'world.';

let phrase = first + ' ' + second;
console.log(phrase);

```

One important thing about the const is that we cant change the value of the variable after the same was initialized. So in this case we still can use let.
