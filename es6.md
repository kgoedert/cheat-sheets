### Const

A variable that can't be changed.

```javascript
const cake = true;
cake = false; //error
```

### Let

a scoped variable. The scope is protected.

```javascript
var topic = "Javascript";

if (topic) {
  let topic = "React";
  console.log(topic); //React
}
console.log(topic); //Javascript
```

### Template Strings

```javascript
const first = "Homer";
const last = "Simpson";

console.log(`${first} ${last}`); //Homer Simpson
```

### Functions Default Parameters

```javascript
function logUserActivity(name, activity = "play guitar") {
  console.log(`The user ${name} likes ${activity}.`);
}

logUserActivity("David"); //The user David likes to play guitar.
logUserActivity("John", "Running"); //The user John likes Running.
```

### Destructuring

```javascript
var movie = {
  title: "Star Wars",
  director: "George Lucas",
  characters: ["Chewbacca", "R2D2", "C3P0", "Yoda"]
};

const { title, director } = movie;

console.log(title, director); //Star Wars George Lucas
```

```javascript
var person = {
  firstname: "Bob",
  lastname: "Doe"
};

var placeOfBirth = ({ firstname }) => {
  console.log(`${firstname} of England.`);
};

placeOfBirth(person); //Bob of England
```

```javascript
var [firstCity] = ["London", "Paris", "New York"];

console.log(firstCity); //London

var [, , thirdCity] = ["London", "Paris", "New York"];

console.log(thirdCity); //New York
```
