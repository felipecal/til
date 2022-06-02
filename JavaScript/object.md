An object in JS its like an object in the normal life, so an object has property ans types.<br>
Like an car, that has property like, color, age, name and others.

Example 1:
```
const person = { 
    name: "Felipe Caldas", 
    age: "20", 
    state: "Brasil" };// a little representation of objects - name, age, state

const test = ["name", "age", "state"]

console.log(`${person.name.substring(0,6)}'s`);
test.forEach(info => console.log(`${info}: ${person[info]}.`))
```

Other way to call an array with object

```
const person = { 
    name: "Felipe Caldas", 
    age: "20", 
    state: "Brasil" };// a little representation of objects - name, age, state

const test = ["name", "age", "state"]

console.log(person[test[0]]);

// or
test.forEach(object => console.log(person[object]));
```
Adding and Updating New Fields in an Object
```
const person = { 
    name: "Felipe Caldas", 
    age: "20", 
    state: "Brasil" };// a little representation of objects - name, age, state

//adding
person.email = "felipe@gmail.com";

console.log(person);
//updating
person.email = "f@gmail.com"

console.log(person);
```
