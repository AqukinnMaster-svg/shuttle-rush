# Badminton 3D

A 3D badminton game for mobile and the web, built with JavaScript and Three.js. It works offline and needs no account.

## Features
- Singles and doubles, with badminton rally scoring (best of 3)
- Practice mode with hit, miss and accuracy stats
- 3-round tournament against harder AI
- Touch controls: joystick, camera pad, Hit (hold to charge), Bunt, Dash, Lift
- Over-the-shoulder camera that switches sides
- Shuttle trail, racket sparks, announcer voice, music and hit sounds
- Settings: game, controls, video, audio, crosshair and GUI scale
- Local save data (settings and stats stored on the device)

## Run it
Open `index.html` in a browser. The game libraries are loaded from `lib/` if present, otherwise from a CDN.

For offline use, put these three.js r128 files in a `lib/` folder:
- three.min.js
- GLTFLoader.js
- SkeletonUtils.js

## Build the Android APK
1. Install Node.js and Android Studio.
2. Run `npm i @capacitor/core @capacitor/cli @capacitor/android`
3. Run `npx cap init Badminton com.yourname.badminton --web-dir www`
4. Put `index.html` and `lib/` in `www/`
5. Run `npx cap add android` and `npx cap sync`
6. In AndroidManifest.xml, add `android:screenOrientation="sensorLandscape"`
7. Run `npx cap open android` and build the APK

## Tech
JavaScript, HTML/CSS, Three.js, Web Audio API.

## Credits
Add credit and license details for the character, racket, shuttlecock and sounds here.