# Tint Clothing POS

A modern, Flutter-based Point of Sale (POS) and Inventory Management system designed specifically for Tint Clothing. This application streamlines billing, stock tracking, and sales reporting.

## Features

- **Store Dashboard**: Get a quick overview of daily sales and quick actions.
- **Inventory Management**:
  - Add, update, and delete products easily.
  - Track stock levels in real-time.
  - Categorize items for better organization.
  - Manage pricing and GST details.
- **Point of Sale (Billing)**:
  - Intuitive cart system for quick checkout.
  - Automatic tax calculation.
  - Support for various payment methods.
  - Invoice generation (PDF) and printing support.
- **Sales Analytics**:
  - View detailed sales history.
  - Analyze performance with visual charts.
- **Secure Authentication**: Admin login to protect sensitive data and configuration.
- **Settings**: Configure application preferences.

## Tech Stack

- **Framework**: [Flutter](https://flutter.dev/) (Dart)
- **Backend**: [Firebase](https://firebase.google.com/)
  - **Authentication**: Secure user login.
  - **Firestore**: Real-time NoSQL database for inventory and sales data.
- **State Management**: [Provider](https://pub.dev/packages/provider)
- **Key Packages**:
  - `printing` & `pdf`: For generating professional invoices.
  - `fl_chart`: For visualizing sales data.
  - `google_fonts`: For consistent and modern typography.

## Getting Started

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install) installed.
- A Firebase project set up.

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/tint-clothing-pos.git
   cd tint_clothing
   ```

2. **Install dependencies**:
   ```bash
   flutter pub get
   ```

3. **Firebase Configuration**:
   - Create a project in the [Firebase Console](https://console.firebase.google.com/).
   - Enable **Authentication** (Email/Password & Google Sign-In).
   - Enable **Firestore Database**.
   - **Android**: Download `google-services.json` and place it in `android/app/`.
   - **iOS**: Download `GoogleService-Info.plist` and place it in `ios/Runner/`.

4. **Run the App**:
   ```bash
   flutter run
   ```

## Project Structure

```
lib/
├── main.dart           # Application entry point
├── app.dart            # Main app widget and theme setup
├── core/               # Core utilities (constants, themes)
├── models/             # Data models (Item, Sale, Admin)
├── screens/            # UI Screens
│   ├── auth/           # Login & Signup screens
│   ├── dashboard/      # Main dashboard with navigation
│   ├── inventory/      # Stock management screens
│   ├── pos/            # Billing & Cart screens
│   ├── sales/          # Sales history & analytics
│   └── settings/       # App settings
├── services/           # Business logic & API calls (Auth, Firestore, PDF)
└── widgets/            # Reusable UI components
```

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
