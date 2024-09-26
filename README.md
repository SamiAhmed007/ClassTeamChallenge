# Digital Pet App with State Management

## Overview

This Flutter project is a digital pet simulation app that allows users to interact with a virtual pet. The app showcases state management using Flutter's `StatefulWidget` and `State` classes. Users can feed or play with the pet, and the app will dynamically update the pet's happiness and hunger levels based on the interactions.

## Features

- **State Management**: Demonstrates the use of Flutter's `StatefulWidget` to manage the state of the digital pet.
- **Pet Interactions**: Users can play with or feed the pet to increase happiness or decrease hunger.
- **Dynamic UI**: The app displays the pet’s happiness and hunger levels in real-time.
- **To-Do Features** (for future implementation):
  - Pet's color changes based on happiness level.
  - Mood indicator with text and emoji.
  - Custom pet name input.
  - Timer-based hunger increase.
  - Win/loss conditions based on happiness and hunger.

## Getting Started

### Prerequisites

Make sure you have the following installed:

- [Flutter SDK](https://flutter.dev/docs/get-started/install)
- [Dart SDK](https://dart.dev/get-dart)
- Any IDE like Android Studio, VS Code, etc.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/SamiAhmed007/ClassTeamChallenge.git
   cd ClassTeamChallenge
   ```

2. Install the required dependencies:
   ```bash
   flutter pub get
   ```

3. Run the app:
   ```bash
   flutter run
   ```

### How to Use

1. When you run the app, a digital pet will appear with its initial happiness and hunger levels set to 50.
2. Use the buttons to either "Play with Your Pet" or "Feed Your Pet." This will increase happiness or decrease hunger levels.
3. The app will update the pet's state dynamically based on your interactions.

## Code Explanation

The core logic of the app is handled by the `State` class in Flutter.

- **State Variables**:  
  `petName`, `happinessLevel`, and `hungerLevel` represent the state of the digital pet.
  
- **Methods**:
  - `_playWithPet()`: Increases happiness and slightly increases hunger.
  - `_feedPet()`: Reduces hunger and updates happiness based on hunger level.
  - `_updateHappiness()` and `_updateHunger()`: Helper methods to modify happiness and hunger.
  
- **UI**: The app displays the pet's name, happiness level, and hunger level, with buttons for interaction.

## To-Do Features (Future Enhancements)

1. **Pet Color Change**:  
   The pet's color will change based on its happiness level:
   - Green for Happy (Happiness > 70)
   - Yellow for Neutral (30 ≤ Happiness ≤ 70)
   - Red for Unhappy (Happiness < 30)

2. **Pet Mood Indicator**:  
   A text-based mood indicator (Happy, Neutral, Unhappy) will be added, with corresponding emojis or mood icons.

3. **Custom Pet Name**:  
   Allow users to customize the pet’s name with a text input field.

4. **Automatic Hunger Increase**:  
   The pet's hunger will increase every 30 seconds using a timer, simulating real-time behavior.

5. **Win/Loss Conditions**:  
   - **Win**: Happiness level stays above 80 for 3 minutes.
   - **Loss**: Hunger level reaches 100, and happiness drops below 10, triggering a "Game Over" message.

## Contribution

Feel free to fork the project and submit pull requests for new features or improvements!
```
https://github.com/SamiAhmed007/ClassTeamChallenge
