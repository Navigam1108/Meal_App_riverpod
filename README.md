# Meal App

A cross-platform Flutter application for browsing, filtering, and favoriting meals. This app demonstrates best practices in state management, modular architecture, and responsive UI design.

## Features

- **State Management with Provider**: Utilizes the Provider package for managing favorites, filters, and meal data across the app.
- **Dynamic Filtering**: Users can filter meals based on dietary preferences (gluten-free, lactose-free, vegetarian, vegan).
- **Favorites System**: Mark and unmark meals as favorites, with persistent state across navigation.
- **Modular & Reusable Widgets**: Clean separation of UI components for maintainability and scalability.
- **Navigation & Routing**: Multi-screen navigation with named routes and custom transitions.
- **Responsive UI**: Optimized layouts for both Android and web platforms.
- **Theming**: Custom themes for a consistent and visually appealing user experience.

## State Management

The app uses the Provider package for efficient and scalable state management. There are three main providers:

- `MealsProvider`: Manages the list of available meals and applies filters.
- `FiltersProvider`: Stores and updates the user's dietary filter preferences.
- `FavouriteProvider`: Handles the logic for adding/removing favorite meals and checking favorite status.

Providers are set up at the root of the widget tree, ensuring all screens and widgets have access to the necessary state.

## Folder Structure

```
lib/
  main.dart                # App entry point and provider setup
  data/dummy_data.dart     # Static meal and category data
  models/                  # Data models (Meal, Category)
  providers/               # State management (Provider classes)
  screens/                 # App screens (Categories, Meals, Filters, etc.)
  widgets/                 # Reusable UI components
```

## Getting Started

1. **Clone the repository:**
   ```sh
   git clone <repo-url>
   cd meal_App
   ```
2. **Install dependencies:**
   ```sh
   flutter pub get
   ```
3. **Run the app:**
   ```sh
   flutter run
   ```

## Customization

- To add new meals or categories, update `lib/data/dummy_data.dart`.
- To modify filters or favorites logic, edit the relevant provider in `lib/providers/`.
- UI changes can be made in the `lib/widgets/` and `lib/screens/` directories.

