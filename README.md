# Slot Machine Game
<img width="747" alt="image" src="https://github.com/user-attachments/assets/f81e3e47-20af-4ea7-a65e-f522bc79df57">

## Introduction
This is a simple slot machine game that consists of a front-end and a back-end part.

- `core.php`: Back-end API file responsible for handling game logic and generating results.
- `index.html`: Front-end file, built using Vue.js and the Axios library for communicating with the back-end API and rendering animations.

## Installation

1. Place the `core.php` and `index.html` files in the same directory.
2. Ensure that PHP is installed in your environment.
3. Open `index.html` in a web browser to run the game.

## Game Rules

- The game features **5 reels**, with **4 different symbols** on each reel.
- Players can adjust their bet amount, ranging from **100 to 1000**.
- If three or more matching symbols appear on the reels, the player wins a corresponding reward.
- **Free Spin Mode** is triggered when 3 or more **Scatter symbols** appear:
  - **3 Scatter symbols**: 5 free spins
  - **4 Scatter symbols**: 10 free spins
  - **5 Scatter symbols**: 15 free spins
- During the free spin mode, the player's bet amount is **not deducted**, but rewards are still accumulated.

### Special Feature: Saving and Completing Free Spins
This slot machine game allows players to save and complete their free spins even if they close and reopen the game. The game state, including the remaining free spins and other relevant data, is stored and retrieved from the back-end API.

## Back-end API

`core.php` is written in PHP and provides the following functionalities:

- Receive game data from `POST` requests.
- Generate reel results and calculate rewards based on the configuration.
- Handle the logic for the free spin mode.
- Return the results in JSON format to the front-end.

## Front-end Interface

`index.html` is built using the Vue.js framework and offers the following features:

- Display the current balance, bet amount, and reward amount.
- Render the 5 reels with animation effects.
- Provide buttons to adjust the bet amount and start spinning.
- Send requests to the back-end API and display the results.
- Show the game rules.

## Notes

- Ensure that PHP is correctly installed in your environment.
- The game logic and configuration can be adjusted in `core.php`.
- The front-end interface styles and animation effects can be modified in `index.html`.

## Enjoy the Game!
