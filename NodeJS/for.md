<h1> For </h1>

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
