
<h2> Two-Dimensional Array </h2>

In the example below we have in the console.log 'concatenate[0][0]', the first 0 is which array I want the data, in this case we can choose with was 0 will be the list of friends, and if it is 1 it would be languages.<br>


```
const friends = ['Pedro', 'Daniel', 'Stequero', 'Andrezin'];

const languages = ['Python', 'JavaScript', 'Java', 'PHP'];
//          index 0 = friends[], index 1 = languages[]

let concatenacao = [friends,languages]

console.log(`${concatenacao[0][0]} your favorite language is ${concatenacao[1][1]}.`);
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
