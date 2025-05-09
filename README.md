# OnTheGo AutoCare Front-End

This is a single code-base front-end using Flutter 3 (Dart) and a custom TypeScript service worker for PWA offline caching.

## Requirements

- Flutter SDK >= 3.0.0  
- Node.js >= 14 (for TypeScript)

## Setup

```bash
# 1. Clone or place these files in a folder:
cd onthego_frontend

# 2. Install and compile the service worker:
cd web
npm install
npm run build-sw
cd ..

# 3. Run on mobile or emulator:
flutter run

# 4. Build and serve the PWA:
flutter build web
cd build/web
# e.g. with Python's simple HTTP server:
python3 -m http.server 8000
