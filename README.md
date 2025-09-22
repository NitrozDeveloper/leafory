# Leafory - Book Discovery App

<p align="center">
    <img src="https://img.shields.io/badge/Flutter-3.35.4-027DFD?logo=flutter" alt="Flutter Version">
    <img src="https://img.shields.io/badge/Dart-3.9.2-0175C2?logo=dart" alt="Dart Version">
    <img src="https://img.shields.io/badge/Architecture-Clean%20%2B%20Feature--First-1E93AB" alt="Architecture">
    <img src="https://img.shields.io/badge/State%20Management-BLoC-00D3B9" alt="State Management">
    <img src="https://img.shields.io/badge/License-MIT-1F509A" alt="License">
</p>

## 📖 Project Description

**Leafory** is a cross-platform (iOS & Android) mobile application that allows users to explore, search, and save their favorite books from the [GutenDex API](https://gutendex.com/), a public API for Project Gutenberg.

This project was designed with a focus on a clean, scalable, and maintainable architecture, as if it were a long-term project to be worked on by a team.

## 🎨 Design

- **Design (Figma):** [Figma URL](https://www.figma.com/design/mteuznbIG6AaJQtwrfPHin/Leafory--Book-Discovery-App-Design?node-id=0-1&t=DW3VJNueDyDkBOCy-1)

## ✨ Key Features

- ✅ **Popular Books Display:** Shows a list of popular books with infinite scroll pagination.
- ✅ **Book Search Functionality:** Search functionality by title or author with debounce for efficiency.
- ✅ **Book Details Page:** Displays detailed information about a selected book.
- ✅ **Favorite/Liking System:** Users can like and unlike books, and their choices are persisted locally on the device.
- ✅ **Favorites Page:** A dedicated page that displays all liked books.
- ✅ **Clean & Scalable Architecture:** Implements Clean Architecture with a clear separation between the Presentation, Domain, and Data layers.
- ✅ **Modern State Management:** Utilizes BLoC for predictable and structured state management.
- ✅ **Declarative Routing:** Uses `go_router` for robust, route-based navigation.
- ✅ **Unit Testing:** Includes unit tests for the Repository and BLoCs to ensure code quality and reliability.

## 🚀 Tech Stack & Architecture

- **Framework:** Flutter
- **Language:** Dart
- **Architecture:** Clean Architecture (Data, Domain, Presentation) + Feature-First
- **State Management:** `flutter_bloc` / `bloc`
- **Navigation:** `go_router`
- **Networking:** `dio`
- **Local Storage:** `hive_ce`
- **Testing:** `mocktail`, `bloc_test`
- **Dependency Injection:** Service Locator Pattern (Manual)

## 📂 Folder Structure

The project follows a clean and scalable directory structure to facilitate easy navigation and development.

```
lib/
├── core/              # For shared logic, services, and utilities (Routing, Dependency Injection, Theme, Database Service, etc.)
├── features/          # For individual feature modules (e.g., book_discovery)
│   ├── data/
│   ├── domain/
│   └── presentation/
└── shared/            # For shared, reusable UI widgets
```

## ⚙️ Getting Started

Follow these steps to get the project up and running on your local environment.

### Prerequisites

- Ensure you have the latest stable version of the [Flutter SDK](https://docs.flutter.dev/get-started/install) installed.
- An emulator (Android/iOS) or a physical device.

### Installation & Running

1. **Clone this repository:**
> ```bash
> git clone https://github.com/deandrasatriyosetiawan/leafory.git
> ```

2. **Navigate to the project directory:**
> ```bash
> cd leafory
> ```

3. **Install all dependencies:**
> ```bash
> flutter pub get
> ```

4. **Run the code generator (important for Hive):**
> ```bash
> dart run build_runner build
> ```

5. **Run the application:**
> ```bash
> flutter run
> ```

### Running Unit Tests

To verify that the business logic in the Repository and BLoCs is working as expected, you can run the provided unit tests.

From the project's root directory, run the following command in your terminal:
> ```bash
> flutter test
> ```

You will see the output in the terminal indicating the status of all executed test cases.

## ⚖️ License

This project is licensed under the MIT License. See the [```LICENSE```](https://github.com/deandrasatriyosetiawan/leafory/blob/main/LICENSE) file for details.