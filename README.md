# Shuttle Rush[WIP]

A 3D badminton game for mobile and the web, built with JavaScript and Three.js.

> **Vibe-coded project:** Made with the help of Claude by Anthropic through vibe coding.

## Play now
**https://aqukinnmaster-svg.github.io/shuttle-rush/**

Note: the game runs in your browser, best on a phone in landscape. The first load needs an internet connection, because some libraries are loaded online. Sound starts after your first tap.

## Features
- Singles and doubles, with badminton rally scoring (best of 3)
- Practice mode with hit, miss and accuracy stats
- 3-round tournament against harder AI
- Touch controls: joystick, camera pad, Hit (hold to charge), Bunt, Dash, Lift
- Over-the-shoulder camera that switches sides
- Shuttle trail, racket sparks, announcer voice, music and hit sounds
- Settings: game, controls, video, audio, crosshair and GUI scale
- Local save data (settings and stats stored on the device, no account needed)

## Run it yourself
Open `index.html` in a browser. The game libraries are loaded from `lib/` if present, otherwise from a CDN.

For offline use, put these three.js r128 files in a `lib/` folder:
- three.min.js
- GLTFLoader.js
- SkeletonUtils.js

## Build the Android APK
1. Install Node.js and Android Studio.
2. Run `npm i @capacitor/core @capacitor/cli @capacitor/android`
3. Run `npx cap init ShuttleRush com.yourname.shuttlerush --web-dir www`
4. Put `index.html` and `lib/` in `www/`
5. Run `npx cap add android` and `npx cap sync`
6. In AndroidManifest.xml, add `android:screenOrientation="sensorLandscape"`
7. Run `npx cap open android` and build the APK

## Tech
JavaScript, HTML/CSS, Three.js, Web Audio API.

## Credits
Music
- "Departure" by DOVA-SYNDROME, https://youtu.be/4Qy8UbMFkNo?si=C0arK8f58VoLATgQ
- "Above" from Haikyuu!, https://youtu.be/QHRcpLQhE0Q?si=i4kojPJp_JxeqA4A

3D models
- Character: "Mii (Nintendo Switch Sports ver.)" by 5468483497, Sketchfab (https://sketchfab.com/3d-models/mii-nintendo-switch-sports-ver-8632ed9250c24b9093e4e3cb4675aedf)

- Racket: "Badminton Racket" by farooq.smurf, Sketchfab (https://sketchfab.com/3d-models/badminton-racket-6b24681f8f254d499c56186825034b7a)

- Shuttlecock: "Badminton" by liuyi1song, Sketchfab (https://sketchfab.com/3d-models/badminton-adec67a4e355451dbf189c9e04735ffe), license
