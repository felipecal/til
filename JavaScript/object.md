An object in JS its like an object in the normal life, so an object has property ans types.<br>
Like an car, that has property like, color, age, name and others.

Example 1:
```
const person = { 
    name: "Felipe Caldas", 
    age: 20, 
    state: "Brasil" };

const test = ["name", "age", "state"]

console.log(`${person.name.substring(0,6)}'s`);
test.forEach(info => console.log(`${info}: ${person[info]}.`))
```

Other way to call an array with object

```
const person = { 
    name: "Felipe Caldas", 
    age: 20, 
    state: "Brasil" };

const test = ["name", "age", "state"]

console.log(person[test[0]]);

// or
test.forEach(object => console.log(person[object]));
```
Adding and Updating New Fields in an Object
```
const person = { 
    name: "Felipe Caldas", 
    age: 20, 
    state: "Brasil" };

//adding
person.email = "felipe@gmail.com";

console.log(person);
//updating
person.email = "f@gmail.com"

console.log(person);
```

Inside of an object we can have array, numbers and other like the example below

```
const person = {
    name: "Felipe Caldas",
    age: 20,
    state: "Brasil",
    phone: ['12233213452', "12332255664"]
};

console.log(`The ${person.name}, has ${person.phone.length} number.\n`);

person.phone.forEach(phones =>console.log(phones));
```

<h2>Object in Obbject </h2>

```

const person = { 
    name: "Felipe Caldas", 
    age: 20, 
    state: "Brasil" ,
    dependent: [{
        name: "Caldas", 
        age: 21,
        state: "Brazil",
        languages: "trsd"
    }]
};

console.log(person.denpendent.languages);
```

other form to add an object in object

```
const person = { 
    name: "Felipe Caldas", 
    age: 20, 
    state: "Brasil" ,
    dependent: [{
        name: "Caldas", 
        age: 21,
        state: "Brazil",
        languages: "trsd"
    }]
};


person.dependent.push({
    name: "Carla", 
    age: 20,
    state: "Brazil"
});



console.log(person);
```
<h2> Object.keys() </h2>
The Object.keys('object') return an array whose elements are strings corresponding to the enumerable properties found directly upon an object, like the example below.

```
const person = { 
    name: "Felipe Caldas", 
    age: 20, 
    state: "Brasil" ,
    dependent: [{
        name: "Caldas", 
        age: 21,
        state: "Brazil",
        languages: "trsd"
    }]
};

console.log(Object.keys(person));
```

That will return the enumerable properties for us in console:

```
[ 'name', 'age', 'state', 'dependent' ]
```

<h2> Object.values() </h2>
The Object.values('object') return for us all the values that we have inside of the object, like the example below

```
const person = { 
    name: "Felipe Caldas", 
    age: 20, 
    state: "Brasil" ,
    dependent: [{
        name: "Caldas", 
        age: 21,
        state: "Brazil",
        languages: "trsd"
    }]
};

console.log(Object.keys(person));
```

That will return the enumerable properties for us in console:

```
[
  'Felipe Caldas',
  20,
  'Brasil',
  [ { name: 'Caldas', age: 21, state: 'Brazil', languages: 'trsd' } ]
]
```

<h2> Object with Function </h2>
Putting an function inside of an object

```
const person = { 
    name: "Felipe Caldas", 
    age: 20, 
    state: "Brasil" ,
    dependent: [{
        name: "Caldas", 
        age: 21,
        state: "Brazil",
        languages: [{
            backend: "Python",
            frontend: "html"
        }]
    },{
        name: "Carla", 
        age: 20,
        state: "Brazil",
        languages: "Python"
    }],
    changeState: function(newState){
        person.dependent.forEach(item => 
            item.name = newState
        )
        console.log("Deu bom!");
    }
};

console.log(person.dependent);

person.changeState("Fulano");

console.log(person.dependent);
```
