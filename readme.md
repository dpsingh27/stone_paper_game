Working of javascript code explaining all the functions abd concepts

Sure, let's go through the code line by line:

1. `let userScore = 0;` and `let compScore = 0;`: Initialize variables to keep track of user and computer scores.

2. `const choices = document.querySelectorAll(".choice");` and `const msg = document.querySelector("#msg");`: Select all elements with the class "choice" and the element with the id "msg" from the HTML document.

3. `const userScorePara = document.querySelector("#user-score");` and `const compScorePara = document.querySelector("#comp-score");`: Select elements with the ids "user-score" and "comp-score" to display and update the user and computer scores.

4. `const genCompChoice = () => {...}`: Define a function `genCompChoice` that generates a random choice ("rock", "paper", or "scissors") for the computer.

5. `const drawGame = () => {...}`: Define a function `drawGame` that displays a message indicating a draw.

6. `const showWinner = (userWin, userChoice, compChoice) => {...}`: Define a function `showWinner` that updates scores and displays a message based on whether the user wins or loses.

7. `const playGame = (userChoice) => {...}`: Define a function `playGame` that takes the user's choice, generates the computer's choice, and determines the winner by calling the `drawGame` or `showWinner` functions.

8. `choices.forEach((choice) => {...});`: Add a click event listener to each element with the class "choice." When a choice is clicked, get the user's choice and call the `playGame` function with that choice.

9. `const resetBtn = document.querySelector("#reset_score");`: Select the element with the id "reset_score" to create a button for resetting scores.

10. `resetBtn.addEventListener("click", () => {...});`: Add a click event listener to the reset button. When the button is clicked, reset the user and computer scores, update the score display elements, and reset the message and background color.

The code essentially creates a simple Rock, Paper, Scissors game with a UI. Users make a choice by clicking on one of the elements with the class "choice," and the computer randomly selects its choice. The game logic determines the winner, updates the scores, and displays messages accordingly. There's also a reset button to clear the scores and start a new game.