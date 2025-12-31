# 🎲 Mouse race

A simple, interactive dice game for two players built with Vanilla JavaScript. The goal is to be the first player to reach 100 points.

## 🎮 How to Play
1. **Roll the Dice:** Click "Roll Dice" to accumulate points in your "Current" score.
2. **Avoid Rolling a 1:** If you roll a 1, your current score is lost, and it becomes the next player's turn.
3. **Hold Your Points:** Click "Hold" to add your current score to your total score. The turn then passes to the other player.
4. **Winning:** The first player to reach a total score of **100 points** wins the game!

## ✨ Features
* **Dual Player Modes:** Supports two players with active player highlighting.
* **Dynamic UI:** Uses DOM manipulation to update scores and dice images in real-time.
* **Game State Management:** Includes a "New Game" functionality to reset all scores and states without refreshing the page.
* **Visual Feedback:** Uses CSS class toggling (`player--winner`, `player--active`) to indicate game status and the winner.

## 🛠️ Tech Stack
* **HTML5:** Structure of the game board.
* **CSS3:** Styling and layout (including winner and active player states).
* **JavaScript (ES6+):** Game logic, event listeners, and state management.

## 🚀 Installation & Setup
1.  **Clone the repository**
    ```bash
    git clone [https://github.com/yourusername/pig-game.git](https://github.com/yourusername/pig-game.git)
    ```
2.  **Open the project**
    Simply open the `index.html` file in any modern web browser.

3.  **Assets Required**
    Ensure you have the dice images (`dice-1.png` through `dice-6.png`) in the project folder for the dice display to work correctly.

## 📂 Code Logic Highlights
* **`init()` function:** Resets the game state (scores to 0, player 1 as active, playing status to true).
* **`switchPlayer()`:** A reusable function that resets the current score and toggles the active player UI using `classList.toggle`.
* **Dice Logic:** Uses `Math.random()` and `Math.trunc()` to generate a random number between 1 and 6.
* **Winner State:** Disables the game buttons once a player hits the 100-point threshold to prevent further moves.

## 📄 License
This project was created for educational purposes as part of a JavaScript Course by Jonas Schemdtmann

