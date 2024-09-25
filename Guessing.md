# Random Guessing Game Flowchart

```mermaid
flowchart TD
    Start([Start Game]) --> GenerateNumber[Generate Random Number]
    GenerateNumber --> GetGuess[Get User Guess]
    GetGuess --> CheckGuess{Is the Guess Correct?}
    CheckGuess -->|Too Low| FeedbackLow[Provide Feedback: Too Low] --> GetGuess
    CheckGuess -->|Too High| FeedbackHigh[Provide Feedback: Too High] --> GetGuess
    CheckGuess -->|Correct| End([End Game])


## Flowchart Description
1. **Start Game**: The game begins, and the computer generates a random number.
2. **Generate Random Number**: The computer randomly selects a number.
3. **Get User Guess**: The player enters a guess for the number.
4. **Check Guess**: The game checks if the guess is too high, too low, or correct.
5. **Provide Feedback**: Based on the guess, the game provides feedback ("too high" or "too low") and prompts the player to guess again if incorrect.
6. **End Game**: The game ends when the player guesses the number correctly.
