# Customer Management App

A cross-platform Flutter app for managing customer records: keep contact details in one place, find customers quickly, and keep their information up to date.

> **Status:** Early development. <!-- TODO: update as the project matures -->

## Features

<!-- TODO: keep only what is actually implemented; move the rest to Roadmap -->

- Add, view, edit and delete customers
- Search and filter the customer list
- Customer details: name, phone, email, address, notes
- Runs on Android, iOS, web, Windows, macOS and Linux

## Screenshots

<!-- TODO: add screenshots to assets/images and link them here -->
<!-- ![Customer list](assets/images/screenshot_list.png) -->

## Tech stack

- [Flutter](https://flutter.dev/) / Dart
- State management: <!-- TODO: Provider / Riverpod / Bloc / setState -->
- Data storage: <!-- TODO: SQLite / Hive / Firebase / Supabase / REST API -->

## Getting started

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install) (stable channel)
- An IDE such as Android Studio or VS Code with the Flutter plugin
- A device, emulator, or browser to run on

Check your setup with:

```bash
flutter doctor
```

### Installation

```bash
git clone https://github.com/rawther5-gif/customer-management.git
cd customer-management
flutter pub get
```

### Run the app

```bash
# List available devices
flutter devices

# Run on a connected device or emulator
flutter run

# Run in the browser
flutter run -d chrome
```

### Run the tests

```bash
flutter test
```

### Build

```bash
flutter build apk          # Android
flutter build ios          # iOS (requires macOS)
flutter build web          # Web
flutter build windows      # Windows
flutter build macos        # macOS
flutter build linux        # Linux
```

## Project structure

```
.
├── lib/            # Application source code
├── test/           # Unit and widget tests
├── assets/images/  # Images and other static assets
├── android/        # Android platform code
├── ios/            # iOS platform code
├── web/            # Web platform code
├── windows/        # Windows platform code
├── macos/          # macOS platform code
├── linux/          # Linux platform code
└── pubspec.yaml    # Dependencies and app metadata
```

<!-- TODO: add a short breakdown of lib/ (models, screens, services, widgets) once the structure settles -->

## Configuration

<!-- TODO: delete this section if the app needs no setup. Otherwise document API keys, Firebase config, .env files, etc. -->

## Roadmap

- [ ] Customer CRUD
- [ ] Search and filtering
- [ ] Import/export (CSV)
- [ ] Authentication
- [ ] Cloud sync

## Contributing

Contributions are welcome. To propose a change:

1. Fork the repository
2. Create a branch: `git checkout -b feature/your-feature`
3. Commit your changes and push the branch
4. Open a pull request

## License

<!-- TODO: choose a license (e.g. MIT) and add a LICENSE file -->
