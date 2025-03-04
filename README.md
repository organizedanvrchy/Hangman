# Hangman (CLI)

## Summary
This Python script is a text-based implementation of the classic word-guessing game, Hangman. The program randomly selects a word from a predefined list, and the player must guess the word by suggesting letters one at a time. The player has a limited number of attempts (6) to guess the word correctly. The game provides visual feedback using ASCII art to represent the hangman's progress and displays the current state of the word with blanks and correctly guessed letters. The game ends when the player either guesses the word correctly or runs out of attempts.

## Features
- **Random Word Selection**: The program uses the `random` module to select a random word from a predefined list (`word_list`).
- **Word Blanks**: The selected word is initially displayed as a series of underscores (`_`), with each underscore representing a letter in the word.
- **Letter Guessing**: The player guesses one letter at a time. If the letter is in the word, the corresponding blanks are replaced with the letter. If the letter is not in the word, the player loses an attempt.
- **ASCII Art**: The program uses ASCII art (`HANGMANPICS`) to visually represent the hangman's progress as the player makes incorrect guesses.
- **Attempt Tracking**: The player has 6 attempts to guess the word. The number of remaining attempts is displayed after each guess.
- **Guessed Letters**: The program keeps track of all guessed letters and displays them to the player to avoid重复猜测.
- **Input Validation**: The program ensures that the player's input is a single alphabetical character and handles invalid inputs gracefully.
- **Screen Clearing**: The terminal screen is cleared after each guess to provide a clean interface for the next guess.
- **Win/Lose Conditions**: The game ends when the player either guesses the word correctly (win) or runs out of attempts (lose). The correct word is displayed at the end of the game.

## How to Play
1. Run the script in a Python environment.
2. Press `Enter` to start the game.
3. Guess one letter at a time by typing a single alphabetical character and pressing `Enter`.
4. If the guessed letter is in the word, the corresponding blanks will be replaced with the letter.
5. If the guessed letter is not in the word, the hangman's progress will be updated, and the number of remaining attempts will decrease.
6. The game ends when the player either guesses the word correctly or runs out of attempts.

## Requirements
- Python 3.x
- The `hangman_words` module (contains the list of words to guess).
- The `hangman_art` module (contains ASCII art for the hangman and the game logo).

## Running the Game
To run the game, simply execute the script in your Python environment:
```bash
python hangman.py
