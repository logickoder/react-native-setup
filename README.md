## ZynoPay

**Mobile App Project Structure Guide**

Welcome to your new React Native project! This guide will help you understand the recommended project structure and best
practices for organizing your codebase. Let's get started:

**Table of Contents**

-
    1. Project Structure

    - 1.1. Components Directory
    - 1.2. Slices (Redux Reducers)
    - 1.3. Navigation
    - 1.4. Features
    - 1.5. Utils and Helpers
-
    2. Redux Setup
-
    3. Styling
-
    4. Testing
-
    5. Environment Variables

**1. Project Structure**

**1.1. Components Directory**

* The `components` folder is used to store reusable UI components.
* Organize components based on their functionality (e.g., buttons, cards, forms).
* Each component should have its own folder containing the component file, styles, and tests.

**1.2. Slices (Redux Reducers)**

* We are using Redux Toolkit to manage state.
* Create a `slice` file in your feature folder to store individual slice files.
* For global slices, create a `slices` folder in the root directory.
* Each slice represents a piece of state (e.g., user, counter).
* Define initial state, reducers, and actions in each slice.

**1.3. Navigation**

* We are using React Navigation.
* Navigation related files can be found in the `src/navigation` directory.
* Define your feature's navigation structure there.

**1.4. Features**

* Each feature should have its own folder (under `src/features`) containing the screen component, styles, and navigation
  configuration.

**1.5. Utils and Helpers**

* Use the `utils` folder for utility functions, API calls, and other shared logic.
* Keep your code DRY by centralizing common functionality.

**2. Redux Setup**

* We are using Redux Toolkit (@reduxjs/toolkit).
* Our redux store is at `src/store.ts`.
* Combine all your slices (reducers) in the store.

**3. Styling**

* We are using Stylesheet from React Native for styling.
* Define reusable styles and themes (colors, fonts) in a separate file.

**4. Testing**

* Place test files (unit tests, integration tests) alongside your components.
* We use Jest for testing.

**5. Environment Variables**

* Manage environment-specific configuration (e.g., API keys) using react-native-config.

