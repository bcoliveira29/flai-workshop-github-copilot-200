# 📘 Assignment: Games in Python

## 🎯 Objective

Build the classic Hangman word-guessing game using Python strings, loops, and user input.

## 📝 Tasks

### 🛠️ Set Up the Game

#### Description
Create the initial game state by selecting a random secret word and setting up variables to track guesses and remaining attempts.

#### Requirements
Completed program should:

- Import the `random` module
- Define a list of at least 5 possible words
- Randomly select one word as the secret word
- Initialise variables for guessed letters and incorrect guess count

### 🛠️ Build the Game Loop

#### Description
Write the main game loop that shows the player their progress, accepts letter guesses, and updates the game state after each guess.

#### Requirements
Completed program should:

- Display the current word progress using `_` for unguessed letters (e.g. `_ _ t h o n`)
- Accept a single-letter guess from the player using `input()`
- Track correct and incorrect guesses separately
- End the loop when the word is fully guessed or the player runs out of attempts

### 🛠️ Display the Result

#### Description
Show the player a win or lose message when the game ends.

#### Requirements
Completed program should:

- Display a congratulations message if the player guesses the word
- Display a game over message revealing the secret word if the player runs out of attempts
