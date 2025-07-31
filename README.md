# BMI Tracker App

A simple Flutter application to calculate and classify your Body Mass Index (BMI) based on your age, weight, and height inputs. The app then displays your BMI score and a health classification.

## 🚀 Features

- Input your **age**, **weight (kg)**, and **height (feet & inches)**.
- Calculate BMI using standard formula:

  \[
  BMI = \frac{\text{weight (kg)}}{(\text{height (m)})^2}
  \]

- Get your BMI result with health classification:
  - Underweight
  - Normal weight
  - Overweight
  - Obese
- Smooth UI with responsive layout and alert dialogs for validation.
- Navigate to a results screen with styled output and color-coded results.

## 📦 Project Structure

```
lib/
│
├── main.dart                 # Entry point
├── screens/
│   ├── home.dart             # MyHomePage widget (input screen)
│   └── result.dart           # ResultScreen widget (shows BMI result)
├── assets/
│   ├── images/
│       ├── hero.jpg          # Hero image shown on home screen
│       ├── logo.png          # Logo image in AppBar
```

## 📱 How It Works

### Input Screen (`MyHomePage`)

- Takes input for:
  - Age
  - Weight (in kg)
  - Height (feet + inches)
- Validates all fields before calculation.
- Calculates BMI using:
  ```dart
  double bmi = weight / (heightInMeters * heightInMeters);
  ```
- Navigates to `ResultScreen` on success.

### Result Screen (`ResultScreen`)

- Displays:
  - Calculated BMI (to 2 decimal places)
  - Health classification based on BMI
  - Age, weight, and height summary
- Color-coded status:
  - Blue: Underweight
  - Green: Normal
  - Orange: Overweight
  - Red: Obese

## ✅ Validation

- All fields are required.
- Only numeric input allowed.
- Error dialog shown if any input is missing.

## 📋 Requirements

- Flutter SDK
- Dart SDK
- Assets (images): `assets/images/logo.png`, `assets/images/hero.jpg`

### Packages Used

- `flutter/material.dart`
- `flutter/services.dart`

## 🔧 Setup

1. Clone the repo:

   ```bash
   git clone https://github.com/your-username/bmi-tracker.git
   cd bmi-tracker
   ```

2. Get packages:

   ```bash
   flutter pub get
   ```

3. Run the app:
   ```bash
   flutter run
   ```

## 📘 License

This project is open source and available under the [MIT License](LICENSE).

---

Made with ❤️ by Malaika Mustafa.

Made with ❤️ by Malaika.
