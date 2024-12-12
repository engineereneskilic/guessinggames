# Guessing Games Project

## Table of Contents
- [Introduction](#introduction)
- [Technologies Used](#technologies-used)
- [Features](#features)
- [Project Structure](#project-structure)
- [Usage Instructions](#usage-instructions)
- [Development Details](#development-details)
  - [Core Classes](#core-classes)
  - [Game Flow](#game-flow)
- [Future Enhancements](#future-enhancements)
- [Project Outcomes & Achievements](#project-outcomes--achievements)
- [License](#license)

## Introduction
The **Guessing Games** project is a console-based application written in **C++**, offering an interactive and engaging experience through various guessing game modes. The primary game mode, **"GuessMovie"**, challenges players to guess movie names by providing partially hidden titles based on difficulty levels. This project demonstrates core object-oriented programming principles, including inheritance, encapsulation, and polymorphism, while being extensible for additional game modes in the future.

## Technologies Used
- **Programming Language**: C++
- **Development Environment**: C++ Console Application

## Features
1. **Dynamic Difficulty Levels**:
   - Easy, Medium, and Hard modes adjust the number of hidden letters in the movie title.
2. **Progressive Gameplay**:
   - Players can choose to guess the full movie title or request additional letters for hints.
3. **Score Tracking**:
   - Keeps track of player scores based on correct guesses and requests for hints.
4. **Randomized Challenges**:
   - Movie titles are randomly selected from a pre-defined list to ensure replayability.
5. **Extensible Design**:
   - Built with scalability in mind, enabling easy addition of new game modes and features.

## Project Structure
The project is organized into the following core components:

1. **Base Class (`GuessGame`)**:
   - Manages shared functionalities such as score tracking, random movie selection, and player interaction.
2. **Derived Class (`GuessMovie`)**:
   - Implements the specific logic for the "GuessMovie" game mode, including letter hiding and hint mechanisms.
3. **Player Class**:
   - Tracks player details, including scores and attempts.

## Usage Instructions
To play the **Guessing Games**:

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/guessing-games.git
   ```
2. Navigate to the project directory:
   ```bash
   cd guessing-games
   ```
3. Compile the C++ files using a compiler like `g++`:
   ```bash
   g++ -o GuessingGames main.cpp GuessGame.cpp GuessMovie.cpp Player.cpp
   ```
4. Run the compiled executable:
   ```bash
   ./GuessingGames
   ```
5. Follow the on-screen instructions to select a game mode and difficulty level.

## Development Details
### Core Classes
1. **GuessGame Class**:
   - Base class providing foundational game functionalities.
   - Handles player input and random movie selection.
2. **GuessMovie Class**:
   - Derived class implementing movie-specific guessing mechanics.
   - Dynamically hides letters in titles based on the selected difficulty.
3. **Player Class**:
   - Tracks player scores and game statistics.
   - Offers methods for updating scores and validating inputs.

### Game Flow
1. **Start**:
   - Players choose a difficulty level.
2. **Gameplay**:
   - A movie title is selected randomly.
   - The title is displayed with hidden letters based on the difficulty.
   - Players can:
     - Guess the full title.
     - Request hints (revealing letters reduces the score).
3. **End**:
   - Scores are calculated and displayed.
   - Players can choose to play again or exit.

## Future Enhancements
- **Additional Game Modes**:
  - Expand the game with other guessing challenges, such as guessing song lyrics or historical events.
- **Multiplayer Support**:
  - Add functionality for multiple players to compete in real-time.
- **Leaderboard System**:
  - Implement a persistent leaderboard to track high scores.
- **Graphical Interface**:
  - Upgrade the console application to a GUI for enhanced user experience.

## Project Outcomes & Achievements
- **Functional Gameplay**:
  - Developed a fully operational guessing game with dynamic difficulty levels.
- **Modular Design**:
  - Ensured the application is easily extensible for future updates.
- **Engaging User Experience**:
  - Designed intuitive game mechanics for smooth gameplay.
- **Technical Proficiency**:
  - Demonstrated expertise in C++ object-oriented programming principles.

## License
This project is open-source and available under the [MIT License](LICENSE).

---

Feel free to explore, contribute, or adapt the **Guessing Games** project for your own applications!
