
# 📘 Assignment: Hangman Game

## 🎯 Objective

Build a command-line Hangman game that lets a player guess a hidden word. Practice using strings, loops, conditionals, lists, and user input.

## 📝 Tasks

### 🛠️ Build the Hangman game

#### Description
Write a Python program that chooses a word and gives the player a limited number of incorrect guesses to uncover it.

#### Requirements
Completed program should:

- Choose one word at random from a predefined list of at least five words.
- Show each unguessed letter as an underscore and reveal letters when guessed correctly.
- Accept one letter per guess and track incorrect guesses, starting with six allowed mistakes.
- Continue until the player reveals the whole word or uses all six incorrect guesses.
- Display the word and a clear win or loss message when the game ends.

### 🛠️ Test and refine the game

#### Description
Run your game with different guesses and fix issues so the player receives clear feedback throughout play.

#### Requirements
Completed program should:

- Tell the player whether each new guess is correct or incorrect.
- Reject input that is not a single letter without reducing the remaining guesses.
- Detect repeated guesses and tell the player without counting them again.
- Show the remaining incorrect guesses after each valid guess.
