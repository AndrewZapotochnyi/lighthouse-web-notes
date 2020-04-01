### Looping over objects

```javascript
const person = {
  firstName: "Martin",
  lastName: "Laws",
  heightInCm: 188
};

// for (const key in person) {
//   console.log(`${key}: ${person[key]}`);
// }

const keys = Object.keys(person);
console.log(keys);

for (const key of keys) {
  console.log(person[key]);
}

// const values = Object.values(person);
// console.log(values);


```