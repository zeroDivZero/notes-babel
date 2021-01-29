# transform-object-rest-spread

[website](https://www.npmjs.com/package/babel-plugin-transform-object-rest-spread)

Transforms rest properties for object destructuring assignment and spread properties for object literals.

## Setup

```zsh
npm install babel-plugin-transform-object-rest-spread
```

Edit `.babelrc`:

```json
{
  "presets": [
    "env"
  ],
  "plugins": [
    "transform-object-rest-spread"
  ]
}
```

## Rest Properties

```javascript
let { x, y, ...z } = { x: 1, y: 2, a: 3, b: 4 }
console.log(x) // 1
console.log(y) // 2
console.log(z) // { a: 3, b: 4 }
```

## Spread Properties

```javascript
let n = { x, y, ...z }
console.log(n) // { x: 1, y: 2, a: 3, b: 4 }
```
