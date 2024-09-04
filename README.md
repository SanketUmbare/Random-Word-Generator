# Random Words Generator - Flutter App

## Overview

This Flutter project is a simple and interactive "Random Words Generator" app that allows users to generate random word pairs, add them to a list of favorites, and view the history of generated words. The app also features an animated history list and a favorites page.

## Features

- **Random Word Pair Generation**: Generates random word pairs using the `english_words` package.
- **Favorites Management**: Allows users to add or remove word pairs from their favorites list.
- **History Tracking**: Keeps track of all the word pairs generated in the current session.
- **Responsive UI**: Adapts to different screen sizes with a responsive layout using a `BottomNavigationBar` for mobile screens and a `NavigationRail` for wider screens.
- **Animated List**: The history list uses an animated list to add new items with a smooth transition effect.

## Getting Started

### Prerequisites

Ensure you have the following installed:

- Flutter SDK: [Flutter Installation Guide](https://flutter.dev/docs/get-started/install)
- Dart SDK (comes bundled with Flutter)
- An IDE such as Android Studio, IntelliJ, or Visual Studio Code with Flutter and Dart plugins

### Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/SanketUmbare/Random-Word-Generator.git
   cd random-words-generator
   ```

2. **Install Dependencies**:

   Run the following command to install the required dependencies:

   ```bash
   flutter pub get
   ```

3. **Run the App**:

   Start the app on an emulator or a physical device:

   ```bash
   flutter run
   ```

## Project Structure

The project follows the standard Flutter directory structure:

- `lib/`: Contains the main code for the app.
  - `main.dart`: The entry point of the app containing the main logic and UI components.

## How It Works

### Main Components

1. **MyApp**:
   - The root widget that initializes the app state using `ChangeNotifierProvider` and sets up the `MaterialApp` with a theme and home page.

2. **MyAppState**:
   - Manages the state of the app, including the current random word pair, the list of generated words (history), and the favorites list. It also handles the logic for generating new words, adding/removing favorites, and notifying listeners of state changes.

3. **MyHomePage**:
   - The main UI of the app that switches between the `GeneratorPage` and `FavoritesPage` based on the user's selection in the navigation.

4. **GeneratorPage**:
   - Displays the current random word pair with options to like (favorite) the word or generate a new one. It also shows the history of previously generated words.

5. **FavoritesPage**:
   - Displays a grid of the user's favorite word pairs with an option to remove them from the favorites list.

6. **HistoryListView**:
   - A custom widget that displays the history of generated word pairs with a fade effect at the top, using an animated list to show new items.

### Responsive Layout

The app is designed to be responsive, switching between a `BottomNavigationBar` for narrow screens and a `NavigationRail` for wider screens. This ensures a consistent user experience across different devices.

## Customization

- **Theme**: The app uses Material 3 with a deep orange color scheme, which can be customized in the `ThemeData`.
- **Word Generation**: The `WordPair` generation logic can be modified or extended to include more complex word combinations or filters.

## Dependencies

- `flutter`: The Flutter framework for building cross-platform apps.
- `provider`: A state management library for managing app state.
- `english_words`: A package for generating random English word pairs.

## Contributions

Contributions are welcome! Feel free to fork this repository, make improvements, and submit a pull request.

## License

You are free to use, modify, and distribute this code as you see fit.

---

Enjoy exploring and building with this Flutter app!
