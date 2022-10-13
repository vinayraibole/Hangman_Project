# Hangman_Project
The objective of our project is to implement the hangman game using Python.

# About Hangman
Going back to our old school days, some of the pen-paper games were always a top for our leisure time. Hangman was one, other than some chit games, to guess words according to the guesses determined and as soon as they lost all their wrong guesses, they were hanged (not really, but on paper 😉). That is an old way, now to play Hangman. The new advancement in technologies allows us to play hangman using our own computer also without any other player.

# Project Prerequisites
This project requires good knowledge of Python which includes defining functions and managing for/while loops. The functions that we use here contain arguments that are defined in a global scope which can be further used in other functions to improve game quality. It can also be used to provide different steps when required to execute upon conditions by the for and while loops.

# Code Explanation

## Import random
This is used to randomly choose an item from a list [] or basically a sequence.

## Import time
This module is used to import the actual time from your pc to use in the program.

## Time.sleep()
This is used to halt the execution of the program for a few seconds. It is a fun way to put the user of the game in short suspense.

We define the main function that initializes the arguments: global count, global display, global word, global already_guessed, global length and global play_game. They can be used further in other functions too depending on how we want to call them.

## Words_to_guess
Contains all the Hangman words we want the user to guess in the game.

## Word
We use the random module in this variable to randomly choose the word from words_to_guess in the game.

## Length 
len() helps us to get the length of the string.

## Count 
Initialized to zero and would increment in the further code.

## Display 
This draws a line for us according to the length of the word to guess.

## Already_guessed
This would contain the string indices of the correctly guessed words.

## Play_loop 
This function deterrmines whether or not the user will play another game after a game is finished.

## Play_game
We use this variable to either continue the game after it is played once or end it according to what the user suggests.

## While loop
Used to execute the play_game argument. It takes the parameter, y=yes and n=no. If the user gives an input of something else other than y/n, it asks the question again for the appropriate answer. If the user inputs “y”, the game restarts, otherwise the game ends.

We call all the variables again under the hangman() function.

## Limit
It is the maximum guesses we provide to the user to guess a particular word.

## Guess
Takes the input from the user for the guessed letter. Guess.strip() removes the trailing and leading whitespaces from the given word.

## If loop 
Checks that if no input is given, or two letters are given at once, it tells the user about the invalid input and executes hangman again.

If the letter is correctly guessed, index searches for that letter in the word.

Display adds that letter in the given space according to its index or where it belongs in the given word.

If we have already guessed the correct letter before and we guess it again, It tells the user to try again and does not lessen any chances.

If the user guessed the wrong letter, the hangman starts to appear which also tells us how many guesses are left. Count was initialized to zero and so with every wrong guess its value increases with one.

Limit is set to 5 and so (limit- count) is the guesses left for the user with every wrong input. If it reaches the limit, the game ends, showing the right guesses (if any) and the word that was supposed to be guessed.

If the word is guessed correctly, matching the length of the display argument, the user has won the game.

Play_loop asks the user to play the game again or exit.

Main() and hangman() would start again if the play_loop executes to yes.

Use the function new_game() to start a new game.


# Summary
With this project in Python, we have successfully developed the Hangman game. We used the popular time and random modules to render our program. Executing different functions and using loops helped us with a better understanding of python basics.