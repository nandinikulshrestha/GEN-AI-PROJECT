
# 5M Stress Relief (Flutter + Firebase) — Prototype

A hackathon-ready prototype for your **5M framework**:
- **Mood**: Emoji-based mood + AI-styled chat
- **Match**: Tinder-like swipe to find peers with similar mood
- **Material**: Roadmap/timeline to reduce stress
- **Maps**: Nearby doctors, yoga teachers, psychologists
- **Mission**: Mini tasks (yoga, walk, diet) with progress

> ⚠️ This ZIP ships without the heavy `android/` and `ios/` folders.
> Generate them once with Flutter:

```bash
flutter create .
flutter pub get
flutter run
```

## Firebase Setup (quick)
1. Create a Firebase project.
2. Enable **Authentication** (Email/Password + Anonymous).
3. Enable **Cloud Firestore** (test mode for demo).
4. Download `google-services.json` → place at `android/app/`.
5. Download `GoogleService-Info.plist` → place at `ios/Runner/`.
6. Update your `applicationId`/`bundleId` in the Firebase console if needed.

This app **will still run without Firebase** in *mock mode*. When Firebase init fails, it uses local in-memory data for demo.

## Maps
- Add an Android Maps API key in `AndroidManifest.xml` after running `flutter create .`.
- iOS requires adding the key in `AppDelegate` Info.plist.
 ![WhatsApp Image 2026-01-04 at 8 44 04 PM (2)](https://github.com/user-attachments/assets/9c2bab55-a68e-4d54-9f04-ee1039710800)

## Mission
![WhatsApp Image 2026-01-04 at 8 44 04 PM (1)](https://github.com/user-attachments/assets/f6395f1d-eadc-4bb1-923c-7c611492df0f)

## Material
![WhatsApp Image 2026-01-04 at 8 44 04 PM](https://github.com/user-attachments/assets/b6e2615f-8e5c-4978-8591-0af34cdd619a)
![WhatsApp Image 2026-01-04 at 8 44 03 PM (1)](https://github.com/user-attachments/assets/cc9517fb-2432-4c65-b976-e12e742a15ab)


## Match
![WhatsApp Image 2026-01-04 at 8 44 03 PM (3)](https://github.com/user-attachments/assets/40e200ee-3532-4db7-b308-144d87da4eb5)
![WhatsApp Image 2026-01-04 at 8 44 03 PM (2)](https://github.com/user-attachments/assets/5ec92731-1df9-41d5-826c-8ff567672d17)
![WhatsApp Image 2026-01-04 at 8 44 03 PM](https://github.com/user-attachments/assets/c2a900b3-b5b0-444c-b42d-19b30d8ed8d4)

## Login page
![WhatsApp Image 2026-01-04 at 8 44 02 PM (2)](https://github.com/user-attachments/assets/fd103588-0e3c-4f12-93d9-c40188f0f1a4)
![WhatsApp Image 2026-01-04 at 8 44 02 PM](https://github.com/user-attachments/assets/c1849343-80d5-4ad5-b235-b8459b3ec254)


## Mood
![WhatsApp Image 2026-01-04 at 8 44 02 PM (1)](https://github.com/user-attachments/assets/66ad34c8-58b1-4e85-bdf0-082ee5948cb8)
![WhatsApp Image 2026-01-04 at 8 44 01 PM (1)](https://github.com/user-attachments/assets/c8f1ca3c-0eb5-4147-9a51-59786c5441fe)






  


## Structure
```
lib/
  main.dart
  theme.dart
  services/
    firebase_service.dart
  screens/
    login_screen.dart
    details_screen.dart
    home_screen.dart
    mood_screen.dart
    match_screen.dart
    material_screen.dart
    maps_screen.dart
    mission_screen.dart
    chat_screen.dart
  widgets/
    mood_emoji_picker.dart
    mission_task_tile.dart
```
