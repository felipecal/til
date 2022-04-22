In JavaScript ES6, object destructuring has been released, which helps us extract values from an object.<br>

```
const person = {
    name: "Felipe",
    age: "20",
    state: "Brasil"
};

const {name, age, state} = person; //Here we get the values of all objects and create a variable to them  

console.log(name);
console.log(age);
console.log(state);

```

Getting only the state of the person object.

```
const person = {
    name: "Felipe",
    age: "20",
    state: "Brasil"
};

const { state } = person;

console.log(state);

```
