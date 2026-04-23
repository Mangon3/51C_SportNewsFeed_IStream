# 5.1C Media & Content Apps

This project contains two mini applications that demonstrate dynamic content and media handling in an Android architecture with RecyclerView, fragments, media playback, and user authentication.

## Projects

1. SportNewsFeed: a sports news feed app built using a "Single Activity" architecture with a horizontal and vertical RecyclerViews to display news and matches
2. **iStream**: a personal video playlist app utilizing the YouTube Player API for media playback and a local Room database for user authentication and playlist management

## NOTE

For general users, open each project directory (`SportNewsFeed` or `iStream`) in Android Studio and run through the gradle runtime.

## DEV NOTE

For Linux users, if the Android Studio emulator is broken on your machine or you want a more streamlined development environment, use the following commands to run the applications:

---

## App 1: SportNewsFeed

### On the 1st Terminal

**1. Start emulator**
```bash
QT_QPA_PLATFORM=xcb ~/Android/Sdk/emulator/emulator -avd Pixel_7_Pro -gpu software -no-snapshot-load
```

### On the 2nd Terminal

**2. Build and install app**
```bash
cd SportNewsFeed
./gradlew installDebug
```

**3. Launch app in emulator**
```bash
adb shell am start -n com.example.sportnewsfeed/.MainActivity
```

---

## App 2: iStream

### On the 1st Terminal

**1. Start emulator** (If not already running)
```bash
QT_QPA_PLATFORM=xcb ~/Android/Sdk/emulator/emulator -avd Pixel_7_Pro -gpu software -no-snapshot-load
```

### On the 2nd Terminal

**2. Build and install app**
```bash
cd iStream
./gradlew installDebug
```

**3. Launch app in emulator**
```bash
adb shell am start -n com.example.istream/.MainActivity
```
