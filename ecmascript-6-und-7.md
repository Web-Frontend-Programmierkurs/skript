EcmaScript 6 oder auch EcmaScript 2015 ist die 6. Version der Standardisierung von JavaScript vom Juni 2015. Sie enthält viele Neuerungen, die deutlich schöneren code ermöglichen. Aufgelistet findet man diese [hier](http://es6-features.org/#Constants).

Die wichtigsten sind folgende:

## Arrow Functions

```js
const myFunc = () => {
    console.log('Hello World');
};
// equals
var myFunc = function() {
   console.log('Hello World');
};
```

Nützlich ist dies vorallem bei Callbacks:

```js
const myArray = [1, 2, 3, 4, 5];
myArray.findIndex(e => e === 4); // 3
```

Außerdem sind Arrow Functions automatisch zu `this` gebunden.

## Klassen

```js
class Greeter {
    constructor(text) {
        this.text = text || 'Hallo Welt!';
    }

    set (text, newText) {
        // do some validation
        this.text = newText;
    }

    get (text) {
        // do something else
        return this.text;
    }

    greet() {
        console.log(this.text);
    }
}

const myGreeter = new Greeter();
myGreeter.greet();
```

## const / let

```js
const myConst = 5; // won't change

for (let i = 0; i < a.length; i++) {
    let x = a[i] // i is valid just in this scope
}
```

## Destructuring

```
const myObj = {
    a = 5,
    b = 42
};

const {a, b} = myObj;
```



