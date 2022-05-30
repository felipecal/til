<h1> Array </h1>

<h2> Two-Dimensional Array </h2>

In the example below we have in the console.log 'concatenate[0][0]', the first 0 is which array I want the data, in this case we can choose with was 0 will be the list of friends, and if it is 1 it would be languages.<br>


```
const friends = ['Pedro', 'Daniel', 'Stequero', 'Andrezin'];

const languages = ['Python', 'JavaScript', 'Java', 'PHP'];
//          index 0 = friends[], index 1 = languages[]

let concatenacao = [friends,languages]

console.log(`${concatenacao[0][0]} your favorite language is ${concatenacao[1][1]}.`);

//Output

Pedro your favorite language is JavaScript
```



<h2> Concat of arrays </h2>

We can follow the code below to concat arrays

```
const friends = ['Pedro', 'Daniel', 'Stequero', 'Andrezin'];

const languages = ['Python', 'JavaScript', 'Java', 'PHP'];

const concatenacao = friends.concat(languages);

console.log(concatenacao);

//Output

[
  'Pedro',
  'Daniel',
  'Stequero',
  'Andrezin',
  'Python',
  'JavaScript',
  'Java',
  'PHP'
]
```
when we want to loop through a list in javascript we can use for.<br>
Mainly when we want to create a loop.<br>

Example:
```
const notas = [10,6.5,8,7.5];
let media = 0;


for (index = 0; index < notas.length; index++) {
    media += notas[index];
}
console.log(`A media das notas é ${media/notas.length}.`);
```

Example with Two-Dimensional Array:
```
const friends = ['Pedro', 'Daniel', 'Stequero', 'Andrezin'];

const languages = ['Python', 'JavaScript', 'Java', 'PHP'];

let concat = [friends,languages];
let secondList = 1;
//        start           end                 incremen
for ( let index =0; index < languages.length; index++ ) {
    console.log(`The favorite language of ${concat[0][index]} is ${concat[1][index]}`);
    secondList ++;
}
```

<h2> forEach </h2>
forEach is a newer method for looping an array.<br>
The difference between for and forEach is that forEach is a callback function

```
const notas = [10,6.5,8,7.5];

let calc = 0;

notas.forEach(nota => calc += nota);

console.log(`A média das notas é ${calc/notas.length}`);
```

forEach with a function that was declared outside.

```
const languages = ['Python', 'JavaScript', 'Java', 'PHP'];


languages.forEach(getLanguage)

function getLanguage(language) {
    console.log(language);
}
```

<h2> Map </h2>

Basically map is so similar to forEach, but the difference is that the map will get all the itens of the array and update/change this array to a new array.
Example of map with numbers:
```
const notas = [10,6.5,8,7.5];
//                                      operador ternário
const novasNotas = notas.map (nota => nota == 10 ? nota : ++nota)
console.log(novasNotas);

```

Example of map with string: 
```
const friends = ['Pedro', 'Daniel', 'Stequero', 'Andrezin'];

const newNames = friends.map (name => name.toLowerCase()) 

console.log(newNames);
```
