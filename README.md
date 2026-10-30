# Photo Enhancer (Android / Kotlin)

## What this app does
- Selects a photo using Android's system photo picker.
- Applies conservative, non-generative tonal correction and mild sharpening.
- Exports a high-resolution image with its aspect ratio preserved (long edge 3840 px).
- Saves output under Pictures/PhotoEnhancer.

## Important limitation
This is a complete, locally running starter app, but it is **not a generative AI / Real-ESRGAN model**. It uses traditional image processing so it does not synthesize or reshape a face/body. Upscaling increases pixel dimensions; it cannot recover details absent from the source. For true AI super-resolution, a separate model/API and usually an API key or hosted backend are required.

## Build
1. Install Android Studio (latest stable) on a computer.
2. Open this `PhotoEnhancer` folder in Android Studio.
3. Let Gradle sync. Use JDK 17.
4. Connect an Android phone with USB debugging enabled, or create an emulator.
5. Press Run.

Package: `com.example.photoenhancer`

## Project structure
- `app/src/main/java/.../MainActivity.kt`: photo selection, enhancement, upscale, save.
- `app/src/main/res/layout/activity_main.xml`: interface.
- `app/src/main/AndroidManifest.xml`: app declaration.
