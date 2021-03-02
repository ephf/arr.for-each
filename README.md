# Array.prototype.setEach

### download:

```bash
npm install arr.set-each --save
```

### use:

```javascript
require('arr.set-each');

var array = [1, 2, 3, 4, 5];

array.setEach((a) => { a += 3; });

console.log(array);
```

*output*

```javascript
[ 4, 5, 6, 7, 8 ]
```

### why?

`Array.prototype.forEach` does not change any values:

```javascript
var array = [1, 2, 3, 4, 5];

array.forEach((a) => { a += 3; });

console.log(array);
```

*output*

```javascript
[ 1, 2, 3, 4, 5 ]
```