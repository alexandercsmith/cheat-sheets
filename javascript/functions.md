# JavaScript Arrays

> JavaScript Array Functions & Methods

* `Array.from()` : Array Chunking
* `Intl.PluralRules` : Ordinal Numbers

---

### `Array.from()` : Array Chunking

> Large Array of 76 Items to Group by 10

```javascript
const hugeArray = Array.from({ length: 76 }, (_, i) => i);

function chunkify(array, chunkSize = 10) {
  { length: Math.ceil(array.length / chunkSize) },
  (_, i) => {
    const start = chunkSize * i;
    return array.slice(start, start + chunkSize);
  };
  return chunks;
}

console.log(chunkify(hugeArray));

/*
[
  [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
  [10, 11, 12, 13, 14, 15, 16, 17, 18, 19],
  [20, 21, 22, 23, 24, 25, 26, 27, 28, 29],
  [30, 31, 32, 33, 34, 35, 36, 37, 38, 39],
  [40, 41, 42, 43, 44, 45, 46, 47, 48, 49],
  [50, 51, 52, 53, 54, 55, 56, 57, 58, 59],
  [60, 61, 62, 63, 64, 65, 66, 67, 68, 69],
  [70, 71, 72, 73, 74, 75, 76]
]
*/
```

---

### `Intl.PluralRules` : Ordinal Numbers

> Find the Ordinal for Numbers

```javascript
function stndrdth(number) {
  const pr = new Intl.PluralRules('en-US', { type: 'ordinal' });
  const ordinals = {
    one: 'st',
    two: 'nd',
    few: 'rd',
    many: 'th',
    zero: 'th',
    other: 'th'
  };
  return `${number}${ordinals[pr.select(number)]}`;
}

stndrdth(1); // 1st
stndrdth(2); // 2nd
stndrdth(3); // 3rd
stndrdth(4); // 4th
```
