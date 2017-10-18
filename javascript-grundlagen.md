# JavaScript Grundlagen

JavaScript ist eine schwach getypte Sprache. Die wichtgsten Datentypen sind `String`, `Number`, `Boolean`, `Object`, `Array` und `Date`.

Neue Variablen defininiert man mit dem Schlüsselwort `var` oder ab ES6 mit `const` oder `let`.

Verwirrend ist manchmal die Typisierung, da noch zwischen primitiven Werten \(`Strings` und `Numbers`\) und Objekten unterschieden wird. Besondere Werte sind `null` und `undefined`. Am besten man spielt mal ein bisschen mit `typeof` und `instanceof` herum.

```js
typeof 1 // "number"
typeof NaN // "number"
typeof Infinity // "number"
typeof -Infinity // "number"
typeof 'test' // "string"
typeof function(){} // "function"
typeof [] // "object"
typeof {} // "object"
typeof null // "object"
typeof undefined // "undefined"
typeof true // "boolean"
3 instanceof Object // "false"
3 instanceof Number // false
Number('3') instanceof Number // false
null instanceof Object // false
new Number('3') instanceof Number // true
[] instanceof Object // true
[] instanceof Array // true
function() {} instanceof Function // true
```

Folgende Kontrollstrukturen gibt es:

```js
while (i < 10) {
    // do something
}

do {
    // do something
}
while (i < 10);

if (a === b) {
  // do something
}

for (var c = 0; c < 10; c += 1) {
  // do something
}

for (element in object) {
  // do something
}

switch(i) {
  case 1:
    // do something
    break;
  case 2:
    // do something
    break;
  default:
     // do something
    break;
}

var c = (b === 5) ? 3 : 4;
```

Siehe hierfür auch [JavaScript/control structures](https://en.wikibooks.org/wiki/JavaScript/Control_structures).

