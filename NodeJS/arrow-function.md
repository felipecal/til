<h1> Arrow Function </h1> <br>

Arrow function is one way more faster and short to write a function.

<h2>Normal function</h2><br>



```
function checkAge(ageToDrink) {
    if (age >= 18 ){
        ageToDrink -1 ;
        return console.log('Você pode beber 1 cervejas');
    }
    else {
        return console.log('Você não pode beber.');
    }
    
}
```

<h2>Arrow function</h2><br>



```
const checkBeer = beers => {
    if (age >= 18 ){
        beers -1 ;
        return console.log('Você pode beber 1 cervejas');
    }
    else {
        return console.log('Você não pode beber.');
    }
}
```

If in our function we have to pass more than 1 paramter we can do like this 



```
const checkBeer = (parametro, outroParametro) => {
    if (age >= 18 ){
        beers -1 ;
        return console.log('Você pode beber 1 cervejas');
    }
    else {
        return console.log('Você não pode beber.');
    }
}
```
