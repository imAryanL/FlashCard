# Flashcard App

## Description
This lab focuses on building a simple flashcard app using **SwiftUI**. The app allows users to view flashcards, swipe through them, and create new flashcards. It includes basic animations and gesture handling to create a smooth user experience.

## Demo

![Flashcard App Demo](https://github.com/user-attachments/assets/602a288a-89ce-4659-a0e7-2d68567919db)

## Feature List
### Core Features:
1. **View Flashcards**: Tap to toggle between question and answer.
2. **Swipe Cards**: 
   - Swipe left (red): Marks card as needing more practice.  
   - Swipe right (green): Marks card as memorized.
3. **Deck Navigation**: Swipe through the deck of flashcards with smooth animations.
4. **Reset Deck**: Reset the deck with all cards or only the ones marked for practice.
5. **Create New Flashcards**: Add new flashcards via a modal form.

## Code Overview
### 1. `ContentView.swift`
- **Main Deck View**: The `ZStack` creates a layered deck of flashcards.
- **Swipe Functionality**: Users can swipe left or right, and cards are removed from the deck.
- **Reset Deck**: The deck can be reset with all cards or just those marked for practice.
- **Modal for New Cards**: A button in the top-right corner allows users to add new flashcards via a modal view.

### 2. `CardView.swift`
- **Custom Card View**: Displays the flashcard, showing either the question or answer based on user interaction.
- **Gesture Handling**: Supports tapping to toggle between question and answer, and swiping left/right to categorize cards.
- **Animation**: Uses `rotationEffect` and `opacity` modifiers to animate card swipes and fades.

### 3. `CreateFlashcardView.swift`
- **Input View for New Cards**: Modal form with input fields for users to create new flashcards.
- **Validation**: The Save button is disabled if either the question or answer fields are empty.
- **On Save**: The newly created flashcard is passed back to the main deck.

### 4. `Card.swift`
- **Card Model**: Defines the `Card` struct with `question` and `answer` properties.
- **Mock Data**: A static list of five hardcoded flashcards to start the deck.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/imAryanL/Flashcard.git
   ```
2. Open the project in Xcode.
3. Run the app on a simulator or a physical device.

## License
Copyright [2024] [Aryan Lakhani]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

