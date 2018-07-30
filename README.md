# Exercises for Day 3 Lecture 2
## Introduction to JavaScript, Part 2 (Web Pages)

## 0 &ensp; Getting Started
1. **Fork** the repository `https://github.com/meet-projects/y2s18-intro-js-2`.
2. **Clone** the repository `y2s18-intro-js-2` into a local directory, replacing `<username>` with your Github username in the following command:
    - `$ git clone https://github.com/<username>/y2s18-intro-js-2`.

## 1 &ensp; Labs

### 1.1 &ensp; Object literals and JSON (`./object-literals`)
0. For this lab, you'll be working in the `object-literals` directory. Make sure you are in the right directory. Make sure that you are adding your HTML and JavaScript to the correct files - don't add HTML to your `.js` file!
1. Create an object literal called `me` in `object-literals.js` that represents yourself. The object should contain the following properties:
    1. `firstName` (type: String) Your first name
    2. `lastName` (type: String): your last name
    3. `favoriteFoods` (type: Array): An array of your favorite foods
    4. `age` (type: Number): Your age
    5. `picture` (type: String): A URL to a picture you like.
2. Convert your object literal `me` into a JSON String that can be shared on different computers, and display it on the HTML page using `document.write`.
3. Go to https://api.meet.sh/json/ and submit your JSON string from step 2. If everything works, you just successfully transmitted data from your computer (the client) to `https://api.meet.sh` (the server), without needing to do much work.
4. Raise your hand and get a checkoff from a TA or Instructor. Nice work!

### 1.2 &ensp; Events (`./html-events`)
0. For this lab, you'll be working in the `html-events` directory. Make sure you are in the right directory. Make sure that you are adding your HTML and JavaScript to the correct files - don't add HTML to your `.js` file!
1. Create a button that creates an `alert` with whatever message you like when the button is clicked.
2. Create a button that, when clicked, cycles the background color of the entire web page in the following order: red, yellow, green, blue, purple.
3. Let's create a counter. Display the value 0 in a `<h1>` tag.
4. Create a button that, when clicked, changes increments the value inside the `<h1>` tag.
5. Create a final button that, when clicked, resets the value inside the `<h1>` tag back to 0.
6. Raise your hand and get a checkoff from a TA or Instructor. Nice work!

### 1.3 &ensp; Event Listeners (`./event-listeners`)
0. For this lab, you'll be working in the `event-listeners` directory. Make sure you are in the right directory. Make sure that you are adding your HTML and JavaScript to the correct files - don't add HTML to your `.js` file!
1. We will be creating a simple slideshow in this lab! Go on Google and download 5 pictures that you like. If you need some help finding images, [Unsplash](https://unsplash.com/) has some pretty photos. Save them into the `./imgs` directory.
2. Create an image on the page with a `<img>` tag.
3. In `event-listeners.js`, create an array called `pictures` of the file names of the images that you downloaded. The array should look something like `['./imgs/dog.jpeg', './imgs/image2.jpg']`.
3. Attach a `click` event listener to the image you created in step 2. Have the image change its `src` attribute when the image is clicked. The value of the `src` attribute should cycle through `pictures`, the list of images you created in the previous step. 
4. Raise your hand and get a checkoff from a TA or Instructor. Nice work!

### 1.4 &ensp; Forms (`./form-validation`)
0. For this lab, you'll be working in the `form-validation` directory. Make sure you are in the right directory. Make sure that you are adding your HTML and JavaScript to the correct files - don't add HTML to your `.js` file!
1. Change the `rating` input field in the rating form (`ratingForm`) so that it only allows users to enter numbers.
2. Add a `onsubmit` event listener, and have it check `validateForm()` in order to make sure the form has valid values in both the `username` and `rating` input fields. 
3. Finish the function `validateForm()` so that ratings cannot be less than 0 or greater than 5. Make sure that usernames have length greater than 0 as well.
4. Raise your hand and get a checkoff from a TA or Instructor. Nice work!

## 2 &ensp; Challenges

### 2.1 &ensp; Object Constructors (`./object-constructors`)
0. For this extra lab, you'll be working in the `object-constructors` directory. Make sure you are in the right directory. Make sure that you are adding your HTML and JavaScript to the correct files - don't add HTML to your `.js` file!
1. Write an object constructor an item a restaurant would sell, called a **MenuItem**. The object should have the following properties:
    1. `name` (type: String): The name of the **MenuItem**.
    2. `price` (type: Number): The price of the **MenuItem**.
    3. `restaurant` (type: String): The name of the restaurant that sells this **MenuItem**.
    4. `getInfo()` (type: Function): Calling this function should return **a sentence** containing the name of the **MenuItem**, its price, and the name of the restaurant where it can be purchased.
2. Create at least three different **MenuItem**'s from restaurants that you've seen before.
3. Display, using `document.write`, the `getInfo()` sentence of each **MenuItem**.

### 2.2 &ensp; Forms (`./form-validation`)
1. Demonstrate that client-side form validation isn't enough by giving a user a rating that's greater than 5 (or less than 0).

### 2.X &ensp; Culminating Challenge
Take the [Tic-Tac-Toe](https://en.wikipedia.org/wiki/Tic-tac-toe) game logic from the previous culminating challenge and build a frontend user interface. Don't prompt the players to type in their move anymore. Instead, the players should be able to click on the screen to make their move.

## 3 &ensp; References
1. JavaScript Events: https://www.w3schools.com/js/js_events.asp
2. List of JavaScript Events: https://www.w3schools.com/jsref/dom_obj_event.asp
3. JavaScript `addEventListener()`: https://www.w3schools.com/js/js_htmldom_eventlistener.asp
4. DOM Visualizer: http://bioub.github.io/d3.DOMVisualizer/