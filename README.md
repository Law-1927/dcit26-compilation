  # DCIT 26 – Flutter Laboratory Compilation

**Course:** DCIT 26 – Application Development and Emerging Technologies
**School:** Cavite State University – Don Severino de las Alas Campus, Indang, Cavite

| | |
|---|---|
| **Name** | _Your Full Name_ |
| **Student Number** | _Your Student Number_ |
| **Course / Year / Section** | _e.g., BSCS 3-1_ |

## About this repository

This repository is a compilation of my DCIT 26 laboratory activities, written in
Dart using the Flutter framework. The repository root is **not** a Flutter app.
Each laboratory is its own independent Flutter project in a separate folder, with
its own `lib/main.dart`, `pubspec.yaml`, `pubspec.lock` and `.gitignore`.

## Laboratory activities

| Lab | Folder | Description |
|---|---|---|
| 1 | `lab1_hello_world/` | Displays a centered "Hello World!" message on a light-blue background. |
| 2 | `lab2_student_profile/` | Display-only student profile showing Name, Age, Course/Year/Section, About me, Achievements and Skills. |
| 3 | `lab3_input_list/` | A text field ("Enter Item") and ADD button that appends items to a list using `setState()`. Blank input is ignored. |
| 4 | `lab4_modal/` | A button opens a modal dialog with an image, scrollable long text and a CLOSE button. Modal lives in `lib/widgets/sample_modal.dart`. |
| 5 | `lab5_navigation/` | Navigation between Home, Profile and About screens, with a drawer. |
| 6 | `lab6_products/` | Product list; selecting an item passes the Product object to a detail screen. |
| 7 | `lab7_networking/` | Fetches a random user from an API using the `http` package, with loading, refresh and retry-on-error states. |
| 8 | _(repository root)_ | Git and GitHub: this repository itself. |

## Repository structure

```
dcit26-compilation/
├── README.md
├── lab1_hello_world/
├── lab2_student_profile/
├── lab3_input_list/
├── lab4_modal/
├── lab5_navigation/
├── lab6_products/
└── lab7_networking/
```

## Requirements

- Flutter SDK (verify with `flutter doctor`)
- Visual Studio Code with the Flutter and Dart extensions
- A run target such as Chrome (Flutter web) or an Android device/emulator
- Internet connection (needed for Lab 7)

## How to run a lab

Run all commands from **inside the lab folder**, not from the repository root.

```bash
cd lab1_hello_world
flutter pub get
flutter run -d chrome
```

Replace `lab1_hello_world` with the lab you want to run. Use `flutter devices`
to see available targets.

### Lab-specific notes

- **Lab 4:** the image must exist at `assets/images/sample_modal_image.png` and be
  registered in that project's `pubspec.yaml`.
- **Lab 7:** requires the `http` package. If dependencies are missing, run
  `flutter pub add http` inside `lab7_networking/`.

## Checks

Run inside a lab folder:

```bash
dart format lib
flutter analyze
flutter test
```

## Notes

- Each lab is a separate project so one activity never overwrites another's `lib/main.dart`.
- Generated folders such as `build/` and `.dart_tool/` are ignored by Git.
- The images in the lab handouts are illustrative mockups, not screenshots of the app.
