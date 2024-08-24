# Casino Game in C++

## Project Overview
This project is a simple text-based casino game written in C++. The game allows a player to deposit an initial amount of money, place bets, and guess a random number to win. If the player correctly guesses the number, they win a multiple of their betting amount; if not, they lose their bet. The game continues until the player decides to quit or runs out of money.

## Features
- Players can start with an initial deposit amount.
- A random number guessing game where players bet on their guesses.
- Players win 10 times their bet amount if they guess correctly.
- The game continues as long as the player has money.
- Error handling for invalid bets and guesses.

## Requirements
- A C++ compiler (e.g., GCC).
- Basic knowledge of C++ and how to compile and run a C++ program.

## How to Run the Game
1. **Clone or Download the Project:**
   Download the source code and save it in a file named `casino_game.cpp`.

2. **Compile the Code:**
   Open a terminal and navigate to the directory containing `casino_game.cpp`. Use the following command to compile the program:
   ```bash
   g++ -o casino_game casino_game.cpp
   ```

3. **Run the Executable:**
   After compilation, run the executable file:
   ```bash
   ./casino_game
   ```

4. **Gameplay Instructions:**
   - Enter a deposit amount to start the game.
   - Place a bet amount for each round.
   - Guess a number between 1 and 10.
   - If you guess the number correctly, you win 10 times the bet amount.
   - If you guess incorrectly, you lose your bet amount.
   - The game will continue until your balance reaches zero or you decide to exit.

## Example Gameplay

1. **Start the Game:**
   ```
   Enter Deposit amount to play game : $100
   ```

2. **Place a Bet:**
   ```
   Enter betting amount: 20
   ```

3. **Make a Guess:**
   ```
   Guess a number (1-10): 7
   ```

4. **Game Outcome:**
   - If you guessed correctly: `winner. Your balance now is $300`
   - If you guessed incorrectly: `loser. Your balance now is $80`

5. The game will loop, allowing you to keep playing as long as you have a balance greater than zero.

## Code Explanation

- **Headers and Libraries:** The program uses standard libraries such as `iostream`, `vector`, `algorithm`, `string`, and others for input/output and random number generation.
- **Random Number Generator:** The `rand_num()` function generates a random number between 1 and 10.
- **Main Loop:** The `main()` function handles the game flow, including taking user input, placing bets, generating random numbers, and updating the player's balance.

## Important Notes
- The program uses the `rand()` function, which generates a pseudo-random number. To make the random numbers more unpredictable, you may want to seed the random number generator using `srand(time(0));` at the start of the `main()` function.
- The game will end if the player's balance reaches zero.

## Future Enhancements
- Add more casino games (e.g., blackjack, roulette).
- Implement a graphical user interface (GUI) for a better user experience.
- Introduce a login system for multiple players.
- Add features for saving and loading game progress.

## License
This project is open-source and free to use. No license restrictions apply.

---

Feel free to modify and improve the code as per your requirements. Happy coding! 🎲
