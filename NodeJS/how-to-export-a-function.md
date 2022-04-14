<h1 align ="center"> Import and Export a function </h1>

When we want to use a code in other place, we can call it a module.<br>
So, when you have some code that can also be used in other parts of your code, files, call it a model
```
const shoes = require('./shoesStore');
```

When we set a require inside our code its important to before use require see if exits some module.exports,<br> that will export the module and after this  we can use in others files

```
class shoesStore {
  constructor() {
    this._codigo = 99;
   }
  imprime(shoes) {
    shoes.forEach(shoes => {
        console.log(`${this._codigo}: ${shoes}`);
     });
   }
}
module.exports = shoesStore; 
```


exporting the class 'ShoesStore'
