<h1 align ="center"> Import and Export a function </h1>


When we want to use a code in other place, we can call it a module.<br>
So, when you have some code that can also be used in other parts of your code, files, call it a model

<h2 align ="center">Import and export</h2>
<h3> Export default e import </h2>
With export default we normally use to export and import just one thing, like variable, class and others. So we have to pay attention in the import, because we dont will use {}; 
<br>

Import
```
import  books  from '../../../index';
```

Export
```
const books = [
  {
    title: 'Clean Code',
    author: 'Robert Cecil Martin',
  },
  {
    title: 'The Clean Coder',
    author: 'Robert Cecil Martin',
  },
]

export default books;
```

<h2>Export and import</h2>
We can use  export to export multiple variable, class or functions
<br>
Import


```
import { books, authors } from '../../../index';
```
Export


```
const books = [
  {
    title: 'Clean Code',
    author: 'Robert Cecil Martin',
  },
  {
    title: 'The Clean Coder',
    author: 'Robert Cecil Martin',
  },
]

const authors = [
  {
    author: 'Robert Cecil Martin'
  },
  {
    author: 'Robert Cecil Martin',
  },
]

export {books,author};
```

<h2 align ="center"> Module.exports and require </h2>


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
