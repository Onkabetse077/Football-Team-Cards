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
