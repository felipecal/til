An object in JS its like an object in the normal life, so an object has property ans types.<br>
Like an car, that has property like, color, age, name and others.

Example 1:
```
const datas = ["11122231234", "11222244232", "66544386543"]; // just a simple list

const people = ["name","Felipe","age", "20","state", "Brasil"] // old form without objects

const  person = {name: "Felipe", age: "20", state: "Brasil"};// a little representation of objects - name, age, state


console.log(person.name);
```

Example 2:
Different form to call an object

```
const  person = {name: "Felipe", age: "20", state: "Brasil"};// a little representation of objects - name, age, state

const test = ["name", "age", "state"]

test.forEach(info => console.log(person[info]))
```
