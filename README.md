# Number Guessing Game

**Note:** The use of AALang for this application is overkill. The simple number guessing game could be implemented with just a few lines of code in any programming language, but it serves as a demonstration of AALang's capabilities for defining agent architectures and behaviors.

## Description

This is an interactive number guessing game implemented using AALang (Agent Architecture Language). The game is defined as a JSON-LD specification that describes an agent system with modes, actors, and personas.

### How It Works

The game follows a simple premise:
- The agent (game master) generates a random number between 1 and 100
- The player attempts to guess the number
- The game provides feedback: "too high", "too low", or "correct"
- The game tracks the number of guesses
- After a correct guess, the player can choose to play again

### Technical Implementation

The game is implemented using AALang, which uses JSON-LD to define:
- **Modes**: The game mode that handles gameplay
- **Actors**: Two actors (Senior and Junior) that operate in the game mode
- **Personas**: Personas that define the behavior and responsibilities of each actor
- **Isolated State**: Game state that tracks the random number, guess count, and game status
- **Message Interface**: Communication between personas and the user

The random number generation uses contextual information from the chat state and temporal context, ensuring variety across different game sessions.

### Running the Game

To play the game, load the `number-guessing-game.jsonld` file in an AALang-compatible agent system. The game will start immediately upon loading.

### Game Features

- Random number generation (1-100)
- Input validation
- Guess tracking
- Feedback on each guess
- Play-again functionality
- Ability to quit at any time

