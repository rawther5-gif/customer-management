# Customer Management App

A cross-platform Flutter app for managing customer records: keep contact details in one place, find customers quickly, and keep their information up to date. The app talks to a backend over a REST API.

> **Status:** Early development (v1.0.0). <!-- TODO: update as the project matures -->

## Features

<!-- TODO: confirm each item against the code; add delete/search here if they already exist -->

- Home screen with the customer list
- Add new customers
- Edit existing customers
- Fetches and saves data through a REST API

## Screenshots

<!-- TODO: add screenshots to assets/images and link them here -->
<!-- ![Customer list](assets/images/screenshot_list.png) -->

## Tech stack

- [Flutter](https://flutter.dev/) with Dart SDK `^3.12.2`
- [`http`](https://pub.dev/packages/http) for API requests
- Material Design, with `cupertino_icons` for iOS-style icons
- No third-party state management package
- Backend: <!-- TODO: name your API/backend (e.g. Node/Express, Laravel, Django, Firebase) -->

## Getting started

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install) (stable channel) with Dart 3.12.2 or newer
- An IDE such as Android Studio or VS Code with the Flutter plugin
- A device, emulator, or browser to run on
- A running instance of the backend API (see [Configuration](#configuration))

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
```

Windows, macOS and Linux platform folders are included as well (`flutter build windows`, `flutter build macos`, `flutter build linux`).

## Configuration

The app needs the address of your backend API.

<!-- TODO: say where the base URL is set (e.g. a constant in lib/...) and what the API endpoints are -->

Notes for local development:

- **Android emulator:** use `http://10.0.2.2:<port>` to reach a server running on your computer. `localhost` points to the emulator itself.
- **iOS simulator / web:** `http://localhost:<port>` works.
- **Physical device:** use your computer's local network IP, and make sure both are on the same Wi-Fi.
- Plain `http://` URLs may need extra platform settings, and production should use `https://`.

## App icon

The launcher icon is generated from `assets/images/cm_logo.png` for Android (min SDK 21) and iOS. After changing the logo, regenerate the icons with:

```bash
dart run flutter_launcher_icons
```

## Project structure

```
.
├── lib/
│   ├── main.dart   # App entry point
│   ├── models/     # Data models
│   ├── screens/    # home_screen, add_customer_screen, edit_customer_screen
│   ├── services/   # API and business logic
│   ├── utils/      # Helpers and shared utilities
│   └── widgets/    # Reusable UI components
├── test/           # Unit and widget tests
├── assets/images/  # Images, including the app logo (cm_logo.png)
├── android/        # Android platform code
├── ios/            # iOS platform code
├── web/            # Web platform code
├── windows/        # Windows platform code
├── macos/          # macOS platform code
├── linux/          # Linux platform code
└── pubspec.yaml    # Dependencies and app metadata
```

## Roadmap

- [x] Customer list, add and edit screens
- [ ] Delete customers
- [ ] Search and filtering
- [ ] Import/export (CSV)
- [ ] Authentication
- [ ] Offline support

## Contributing

Contributions are welcome. To propose a change:

1. Fork the repository
2. Create a branch: `git checkout -b feature/your-feature`
3. Commit your changes and push the branch
4. Open a pull request

## License

<!-- TODO: choose a license (e.g. MIT) and add a LICENSE file -->
