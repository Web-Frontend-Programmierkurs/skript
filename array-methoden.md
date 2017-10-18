# Array Methoden

Um gut auf Daten arbeiten zu können, sollte man ein paar nützliche Methoden von `Array` kennen.

#### Filter

[https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global\_Objects/Array/filter](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)

```js
[1, 2, 3].filter(e => e >= 2); // [2, 3]
```

#### Find

[https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global\_Objects/Array/find](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Array/find)

```js
var inventory = [
    {name: 'apples', quantity: 2},
    {name: 'bananas', quantity: 0},
    {name: 'cherries', quantity: 5}
];

function findCherries(fruit) { 
    return fruit.name === 'cherries';
}

console.log(inventory.find(findCherries)); // { name: 'cherries', quantity: 5 }
```

#### FindIndex

[https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global\_Objects/Array/findIndex](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Array/findIndex)

```js
[12, 5, 8, 130, 44].findIndex(e => e >=15); // 3
```

#### ForEach

[https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global\_Objects/Array/forEach](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)

```
var a = ['a', 'b', 'c'];

a.forEach(function(element) {
    console.log(element);
});

// a
// b
// c
```

#### Map

[https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global\_Objects/Array/map](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Array/map)

```js
[1, 2, 3].map(e => ({value: e})); // [{value: 1}, {value: 2}, {value: 3}]
```



