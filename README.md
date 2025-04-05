# INTEL-Unnati-2025
# Gen AI Interactive Learning Games

Welcome to Gen AI Interactive Learning Games, a terminal-based mini math game designed to make learning fun through color, interactivity, and soon—AI-powered features!

---

## Overview

This game helps users practice basic arithmetic operations through randomly generated problems. User progress is saved between sessions, allowing them to continue learning from where they left off. It's built using Python with a clean modular approach and uses fun terminal visuals for an engaging experience.

---

## Modules Used

### 1. `random`
- Generates random numbers and selects random arithmetic operations.
- Powers the dynamic math problem generation.

### 2. `json`
- Manages saving and loading user progress via a file named `progress.json`.
- Ensures user data is retained between sessions.

### 3. `colorama`
- Adds color to the terminal text for a more visually appealing interface.
- Enhances the fun and engagement level of the game.

---

## Game Features

### Load Progress
- On startup, the game attempts to load previous progress from `progress.json`.
- If the file doesn’t exist, an empty dictionary (`progress = {}`) is initialized.

### Save Progress
- After each correct answer, the progress is saved back to `progress.json`.
- Utilizes `json.dump(progress, file)` for writing the dictionary to file.

### Main Game Loop
- Loads user progress at launch.
- Prints a colorful welcome message using `colorama`.
- Enters an infinite loop (`while True`) to generate new problems continuously.
- Each iteration:
  - Presents a random arithmetic question.
  - Checks user input and validates correctness.
  - Updates and saves progress accordingly.

---

## Current Operations Supported

- Addition (`+`)
- Subtraction (`-`)
- Multiplication (`*`)
- Division (`/`)

---

## Future Scope

We're planning to integrate AI capabilities in future updates, including:
- Adaptive difficulty levels based on user performance.
- AI-generated custom problem sets.
- Personalized learning insights and feedback.
- Voice-based interaction and visual recognition features.

---
Happy Learning!
