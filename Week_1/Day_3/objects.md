### Objects

```javascript
const person = {
  firstName: "Martin",
  lastName: "Laws",
  fullName: function() {
    return `${this.firstName} ${this.lastName}`;
  },
  heightInCm: 188,
  heightInInches: function() {
    return Math.floor(this.heightInCm / 2.54);
  }
};

const dog = {
  firstName: "Maya",
  lastName: "Laws",
  fullName: function() {
    return `${this.firstName} ${this.lastName}`;
  }
};

console.log(person.fullName());
console.log(person.heightInInches());


```