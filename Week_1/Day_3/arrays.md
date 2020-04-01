### Looping over arrays best practice

```javascript
const friendsArray = ["Martin", "Scott", "Craig", "Mira"];

// Option 1:
function friendCallback(name) {
   console.log(name)
 }

 friendsArray.forEach(friendCallback)

 // Option 2:
 friendsArray.forEach(function(name) {
   console.log(name)
 })

 // Option 3 (most modern, much nice):
 friendsArray.forEach(name => console.log(name))

for (const friendName of friendsArray) {
  console.log(friendName);
}

for (const friendIndex in friendsArray) {
  console.log(friendIndex);
  console.log(friendsArray[friendIndex]);
}

 for (const [index, value] of friendsArray.entries()) {
   console.log(index, value);
 }

```