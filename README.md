2048 Game

This is a JavaScript implementation of the classic 2048 game. The game logic is encapsulated in a Game class and interacts with a simple HTML/CSS UI. The player can move tiles using keyboard arrows, merge identical numbers, and aim to reach the 2048 tile.

Features:

- 4×4 game board

- Tiles can contain numbers: 2, 4, 8 … 2^n

- Tiles slide and merge according to standard 2048 rules

- Merged tiles increase the score

- Random new tile (2 or 4) appears after each move (4 has 10% probability)

- Start, restart, win, and game over messages handled dynamically

- Arrow key controls

- Optional animations for tile movements

- Blocked double merges during a single move

- Restart button resets the game to its initial state

Technologies:

- HTML5

- CSS3

- JavaScript (ES6)

- Module-based project structure

Project Structure:
```
src/
├─ modules/
│  └─ Game.class.js   # Game logic encapsulated in Game class
├─ index.html         # UI for the game
├─ scripts/
│  └─ main.js         # UI logic using Game class instance
└─ styles/
   └─ main.css        # Game styles
```

Required Game Class Methods:

- constructor(initialState?) – initializes the board; initialState is optional

- getState() – returns the current board state

- getScore() – returns the current score

- getStatus() – returns game status

- moveLeft() / moveRight() / moveUp() / moveDown() – move tiles in the specified direction

- start() – starts the game

- restart() – resets the game to the initial state

How to Run Locally:

Clone the repository:
```
git clone <repository_URL>
```

Navigate to the project folder:
```
cd 2048-game
```

Install dependencies (if using npm for testing):
```
npm install
```

Open index.html in a browser to play the game.

- [DEMO LINK](https://melarkkkk.github.io/js_2048/)
