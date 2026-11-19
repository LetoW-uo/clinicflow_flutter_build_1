# clinicflow_flutter_build_1

A new Flutter project.

## Project structure

Flutter uses the same Dart application source for web and mobile, so feature code
belongs in `lib/`, not in `web/`. The `web/` folder contains browser-specific
files such as the HTML entry point, manifest, and icons.

```text
lib/
  main.dart
  core/                         Shared app code used by multiple features
    models/
    navigation/
    theme/
    widgets/
  features/                     Keep each subsystem in its own folder
    authentication/
    appointments/
    patient_check_in/
    communication/
      notifications/
      messages/
    clinic_administration/
test/
  features/                     Tests organized to match lib/features
    authentication/
    appointments/
    patient_check_in/
    communication/
      notifications/
      messages/
    clinic_administration/
assets/                         Shared app assets (register used assets in pubspec.yaml)
  images/
  fonts/
web/                            Web entry point and static web files
```

For branch work, keep changes within the feature folder for the subsystem being
developed. Coordinate shared changes to `lib/core/` and `lib/main.dart` with the
team, and put tests in the matching `test/features/` folder. These folders are
placeholders only; no features have been implemented.

### Human summary
Basically, the subsystem folders are all in lib, not in web. 
Also, the code for the patient, staff and admin sides of each subsystem will be implemented and designed inside those subsystem files.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Learn Flutter](https://docs.flutter.dev/get-started/learn-flutter)
- [Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Flutter learning resources](https://docs.flutter.dev/reference/learning-resources)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## To Do before branching out the project (DO NOT SKIP!!!!!!!!!!!!!!)

First and foremost we need to figure out how the backend and frontend will communicate. That way each subsystem will be "speaking the same language". 

We will also need to determine how/if we will encrypt data for this prototype. For now I have not added anything to that effect.

Then we need to figure out who will work on what parts of the app