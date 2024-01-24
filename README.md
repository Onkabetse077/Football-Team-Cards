One common aspect of building web applications: processing datasets, and then outputting information to the screen.
In this sports team cards project, you'll learn how to work with DOM manipulation, object destructuring, event handling,
and data filtering.

This project will cover concepts like switch statements, default parameters, Object.freeze(), the map() method, and more.

//Step 1
In this project, you will build a set of football team cards and learn about nested objects, object destructuring,
default parameters, event listeners, and switch statements.
All of the HTML and CSS for this project has been provided for you.

Start by accessing the id called team from the HTML document and storing it in a const variable called teamName.

Remember, you can use the getElementById method for this.

//Step 2
Next, access the id called sport from the HTML document and store it in a const variable called typeOfSport.
Below that variable, assign the id of year to a const variable called worldCupYear.

//Step 3
Next, access the id called head-coach from the HTML document and store it in a const variable called headCoach.
Below that variable, assign the id of player-cards to a const variable called playerCards.

//Step 4
Create one more const variable called playersDropdownList and assign it the id of players using the getElementById method.

//Step 5
Now it is time to build out the data structure that will hold all of the information for your football team.

Below the variables you just created, create a new const variable called myFavoriteFootballTeam and assign it an empty object.

//Step 6
Inside the myFavoriteFootballTeam object, add a new property with a key named team and a string value of Argentina.

//Step 7
Below the team property, add a new property with a key named sport and a string value of Football.

//Step 8
Below the sport property, add a new property with a key named year and a number value of 1986.

//Step 9
Below the year property, add a new property with a key named isWorldCupWinner and a boolean value set to true.

//Step 10
Below the isWorldCupWinner property, add a new key called headCoach with a value of an empty object.
Inside that object, add a property with a key of coachName and a string value of Carlos Bilardo.
Below that property, add another key called matches with a number value of 7.

//Step 11
Below the headCoach property, create a new property with a key named players with the value of an empty array.

//Step 12
Inside that players array, create a new object with the following properties:

name: "Sergio Almirón"
position: "forward"
number: 1
isCaptain: false
nickname: null

//Step 13
Below that object, create a new object with the following properties:

name: "Sergio Batista"
position: "midfielder"
number: 2
isCaptain: false
nickname: null

//Step 14
The rest of the data for the myFavoriteFootballTeam.players array has been filled out for you.

The next step is to ensure that you can't modify this object by adding or removing any properties.
We are going to use a method called Object.freeze(obj) which will freeze this object and prevent any changes being made to it.

Use the Object.freeze() method to freeze the myFavoriteFootballTeam object.

//Step 15
To check if the Object.freeze() method is working, you can try to assign a new value to one of the existing properties.

Below the Object.freeze(myFavoriteFootballTeam), assign the USA string to myFavoriteFootballTeam.team.
Below that, add a console.log for myFavoriteFootballTeam.team.

When you open up the console, you will see an Uncaught TypeError message.
This error appears because the Object.freeze() method does not allow you to overwrite that value.

//Step 16
Now that you have tested the Object.freeze() method, you can delete those two lines of code from the last lesson.

The next step is to access the key called sport from the myFavoriteFootballTeam object and assign it to a new const variable called sport.

Remember you can use dot notation for this.

//Step 17
Below the sport variable, access the key called team from the myFavoriteFootballTeam object and assign it to a new const variable called team.

//Step 18
In the last two steps, you have been accessing properties from the myFavoriteFootballTeam object using dot notation and assigning them to new const variables.
But in JavaScript, there is an easier way to accomplish the same goal.

The object destructuring syntax allows you to unpack values from arrays and objects:

const developerObj = {
name: "Jessica Wilkins",
isDeveloper: true
};

// Object destructuring
const { name, isDeveloper } = developerObj;
Rewrite the two lines of code below using the new destructuring syntax. Your answer should be one line of code.

//Step 19
Next, add the year and players to your destructuring assignment.

//Step 20
Now you need to access the coachName value from the myFavoriteFootballTeam.headCoach object using the destructuring syntax.

//Step 21
Now you need to start displaying the team's information on the screen.

Below your destructuring assignments, assign the sport variable to typeOfSport.textContent.

Once you complete that task, you should see the result in the preview window.

//Step 22
Next, assign the team variable to teamName.textContent.

//Step 23
Assign the year variable to worldCupYear.textContent.

Below that, assign the coachName variable to headCoach.textContent.

You should now see all of that information displayed on the screen below Team stats.

//Step 24
Now you will start building out the function that will show player cards based on the selections made by the user in the Filter Teammates dropdown menu.

Start by creating an empty arrow function called setPlayerCards. You do not need to add a parameter because that will be taken care of in the next step.

//Step 25
Function parameters can be initialized with default values.
If a function is called without an argument, then the default value will be used:

const greeting = (name = "Anonymous") => {
return "Hello " + name;
}

console.log(greeting("John")); // Hello John
console.log(greeting()); // Hello Anonymous
Add a new parameter to your setPlayerCards function called arr and assign it a default value of players.

//Step 26
The next step is to create a new array that will be responsible for adding the player card information to the page.

Inside the setPlayerCards function, start by adding the map method to arr that will take in an empty callback function.
Then, use the addition assignment += operator to assign the new array to playerCards.innerHTML.

Remember that the innerHTML property gets, or in this case, sets the HTML markup for the playerCards element.

//Step 27
arr contains a series of objects that each contains a name, position, number, isCaptain and nickname property.
In order to access each of those properties inside the callback function, you will need to use object destructuring to unpack them into variables.

Here is an example:

function myExampleFunction({ name, age, job, city }) {

}
Inside the parameter list in the callback function for the map method, unpack all 5 object properties from objects in arr using object destructuring.

//Step 27
arr contains a series of objects that each contains a name, position, number, isCaptain and nickname property. In order to access each of those properties inside the callback function, you will need to use object destructuring to unpack them into variables.

Here is an example:

function myExampleFunction({ name, age, job, city }) {

}
Inside the parameter list in the callback function for the map method, unpack all 5 object properties from objects in arr using object destructuring.

//