# JavaScript specific concepts

## Find elements in the DOM:

- determine the URL - `document.location`
- page dimensions - `window.innerWidth` / `window.innerHeight`
- select element by ID - `getElementById()`
- select items by class - `getElementsByClassName()`
- select elements based on HTML tag - `getElementsByTagName()`
- select elements as in CSS - `querySelector()` / `querySelectorAll()`
- CSS in javascript _(eg. background-color in CSS, backgroundColor JS)_
- CSS class list - `classList` - `add`, `remove`, `toggle`, `list`
- get data of form inputs
- events - _click, key up, focus, blur_
- scrolling

### Exercises

1. create a text field in which you can enter a hex color code. And a button that - when pressed - sets the page's background color to this color
2. create a text field, and if you type in it, log out which character was entered
3. create a web page with some random long content and add button at the bottom that scrolls back to the top of the page (if possible, nicely animated, but it doesn't have to be the first time)
4. create a form with 3 text fields (name, email, password) and one button. The button should be inactive unless all three fields have values.

## Cookies, local storage, session storage:

- check what are the differences, learn how to modify them, delete them, where you can see it in the browser

### Exercises

1. ask the name of the user, and if you refresh the page, if it already exists, write it out on the screen
2. display a cookie banner at the bottom of a webpage (GDPR) and once it's accepted by the user, do not display it again

## Math functions:

- `min()`, `max()`
- `round()`, `floor()`, `ceil()`
- `random()`

**Numbers (not math):**

- `toFixed()`
- `parseInt()`, `parseFloat()`

### Exercises

```
const people = [
    {
        age: 32,
        name: 'Anne',
        date_of_birth: '1988-03-15'
    },
    {
        age: 22,
        name: 'Betty',
        date_of_birth: '1998-01-20'
    },
    {
        age: 15,
        name: 'Cyntia',
        date_of_birth: '2004-11-10'
    },
    {
        age: 21,
        name: 'David',
        date_of_birth: '1999-10-20'
    },
    {
        age: 25,
        name: 'Emil',
        date_of_birth: '1995-06-02'
    },
    {
        age: 49,
        name: 'Ferenc',
        date_of_birth: '1971-04-03'
    },
];
```

Create buttons for the following tasks:

1. print out a random number between 1 and 10
2. log out a random person from the array
3. find the youngest and oldest person from the list
4. calculate the average age
5. create a function that generates a random hex color code
   (hex color codes are like this: 0..255 red; 0..255 green, 0..255 blue), in hexadecimal numeric system)

## Timing

- `setTimeout()`
- `setInterval()`

### Exercises

1. create a button, which - 4 seconds after clicking on it - changes the background color to a random color.
   You should be able to cancel it by clicking on another button.
2. create a button which - when clicked - changes the background-color to a random color every 2 seconds.
   You should be able to cancel it by clicking on another button.

## Dates

- create a new date
- `getMonth`, `getDay`, `getHour` ...
- very useful library: **moment.js**
- learn about moment.js
- new date, from text, transforming

### Exercises

1. create a function that returns with the date of the first day of the current month
2. create a function that takes a number (eg 32) and prints out what day it will be in as many hours (eg Tuesday)
3. create a function that takes a date (in this format: 2020-04-12) and checks whether it is before or after today
4. make a real clock that plots the current time (regular clock with 3 hands).
   you can use setInterval to keep track of the time.
5. create a function that takes a date, and returns the people (from the _people_ array above) who were born before that date.
