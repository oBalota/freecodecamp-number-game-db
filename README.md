# Number Guessing Game

This repository contains my solution for the **Number Guessing Game** project, which is the final milestone of the **Relational Database Certification** on freeCodeCamp.

The project features a dynamic interactive Bash script that generates a random secret number between 1 and 1000 and challenges the user to guess it. The script seamlessly connects to a PostgreSQL database to track user history, calculate total games played, and update their personal best score (fewest guesses).

---

## 🚀 Features

* **Relational Database Integration:** Tracks users and game statistics across two normalized tables (`users` and `games`) using Foreign Keys.
* **Smart User Recognition:** * Greets new users and initializes their profile in the database.
    * Welcomes returning users with personalized statistics: total games played and their all-time best game score.
* **Robust Input Validation:** Uses regular expressions to detect non-integer inputs and gracefully prompts the user to guess again without crashing.
* **Git Version Control:** Developed using strict conventional commit messages (`feat:`, `fix:`, `chore:`, `refactor:`) with a perfectly clean working tree.

---

## 🛠️ Tech Stack & Concepts

* **Database:** PostgreSQL (SQL)
* **Scripting:** Bash / Shell (Loops, Conditionals, User Input Handling)
* **Version Control:** Git
* **Concepts:** Database Normalization, Aggregate Functions (`MIN`, `COUNT`), Pattern Matching

---

## 💻 How to Run the Script

Ensure you have PostgreSQL running with the `number_guess` database imported from the provided `.sql` dump file.

1. Give execution permissions to the script:
   ``bash
   chmod +x number_guess.sh``

   ## Run the game:
    ``./number_guess.sh``

   ## Gameplay Flow Example:
   Enter your username:
   oBalota
   Welcome back, oBalota! You have played 3 games, and your best game took 12 guesses.
   Guess the secret number between 1 and 1000:
   500
   It's lower than that, guess again:
   250
   It's higher than that, guess again:
   340
   You guessed it in 3 tries. The secret number was 340. Nice job!
   
