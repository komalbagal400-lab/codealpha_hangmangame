# Hangman Game (Python)

This is a basic **console-based Hangman game** written in Python.  
The player guesses letters to reveal a hidden word before running out of lives.

---

## Game Description

- A random word is selected from a list of words
- The player starts with **6 lives**
- Correct guesses reveal letters in the word
- Incorrect guesses reduce lives
- Hangman stages are displayed after each guess
- The game ends when:
  - All letters are guessed → **You Win**
  - Lives reach zero → **You Lose**

---

## Files Used

hangman_game
│
├── main.py # Main game logic
├── word_file.py # Contains the list of words
├── hangman_stages.py # Contains hangman ASCII stages
└── README.md # Project documentation

---

## Code Explanation (Overview)

- `random.choice()` selects a word from `word_file.words`
- A list called `display` stores `_` for unguessed letters
- A `while` loop runs until the game ends
- User inputs a letter and the program checks:
  - If the letter exists in the word
  - If the guess is wrong, a life is lost
- The hangman stage updates after each guess

  ---

  ## Example `word_file.py`

```python
words=[
"jenny",
"apple",
"beautiful",
"mango",
"jayanti",
"attitude",
"aeroplane"
]

---

Example hangman_stages.py
stages = ['''
  +---+
  |   |
  O   |
 /|\  |
 / \  |
      |
=========
''', '''
  +---+
  |   |
  O   |
 /|\  |
 /    |
      |
=========
''', '''
  +---+
  |   |
  O   |
 /|\  |
      |
      |
=========
''', '''
  +---+
  |   |
  O   |
 /|   |
      |
      |
=========''', '''
  +---+
  |   |
  O   |
 /    |
      |
      |
=========
''', '''
  +---+
  |   |
  O   |
      |
      |
      |
=========
''', '''
  +---+
  |   |
      |
      |
      |
      |
=========
''']

---

How to Run the Game
1.	Make sure all files are in the same folder
2.	Open a terminal in that folder
3.	Run the program:
Hangman game.py
4.	Guess letters until you win or lose

---

Features
•	Random word selection
•	Lives system
•	Visual hangman stages
•	Win and lose messages

---

Possible Improvements
•	Hide the chosen word (remove print(chosen_word))
•	Prevent repeated guesses
•	Add full-word guessing
•	Improve input validation

---

Author

📌 Komal Bagal

