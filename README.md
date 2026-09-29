# Watchly 🎬

Watchly is a free Android application for keeping track of movies and TV shows and answering a simple question:

> **How much content do I have left to watch?**

The app lets users search for movies and TV shows, save them to a personal library, track watched episodes and movies, and calculate remaining watch time, episodes, seasons and pack progress.

## Features

- 🔎 Search movies and TV shows with TMDB.
- 🎬 Movie details, runtime, genres, rating, synopsis and cast.
- 📺 TV show details with seasons and episodes.
- ✅ Mark movies as watched.
- ✅ Mark individual episodes as watched or unwatched.
- ✅ Mark complete seasons as watched.
- ⏱️ Calculate remaining watch time automatically.
- 📚 Personal offline library.
- 📦 Custom packs/franchises containing movies and TV shows.
- 📊 Overall progress and statistics.
- 🌙 Material 3 interface with light and dark themes.
- 💾 Local persistence with Room.
- ☁️ TMDB metadata and images loaded through the TMDB API.

## Technology

Watchly is built as a native Android application using:

- Kotlin
- Jetpack Compose
- Material 3
- Android Architecture Components
- MVVM
- Navigation Compose
- Kotlin Coroutines
- Flow / StateFlow
- Retrofit
- Gson
- Room
- Hilt
- Coil

The application package is:

```text
com.example.watchly
```

The current prototype intentionally keeps the Android implementation in a single Kotlin file:

```text
app/src/main/java/com/example/watchly/MainActivity.kt
```

## TMDB

Watchly uses **The Movie Database (TMDB)** for movie and TV metadata and images.

> **This product uses the TMDB API but is not endorsed or certified by TMDB.**

The TMDB website:

https://www.themoviedb.org

TMDB API documentation:

https://developer.themoviedb.org/

TMDB API usage is subject to TMDB's current terms and requirements:

https://developer.themoviedb.org/docs/faq

## Non-commercial project

Watchly is intended to be a free, non-commercial mobile application.

There are currently:

- No advertisements.
- No subscriptions.
- No paid features.
- No in-app purchases.

This statement describes the current project intention and should be kept up to date if the business model changes.

## API key

The TMDB API token must never be committed to this repository.

Create a local `local.properties` file and add:

```properties
TMDB_API_KEY=YOUR_TMDB_API_READ_ACCESS_TOKEN
```

The Android build exposes it to the application through:

```kotlin
BuildConfig.TMDB_API_KEY
```

`local.properties` should remain uncommitted.

## Running the project

1. Open the project in Android Studio.
2. Use JDK 17.
3. Configure `TMDB_API_KEY` in `local.properties`.
4. Sync Gradle.
5. Build and run the application on an Android device or emulator.

## Project structure

The project is currently centered around:

```text
app/
└── src/
    └── main/
        ├── AndroidManifest.xml
        └── java/
            └── com/
                └── example/
                    └── watchly/
                        └── MainActivity.kt
```

## Privacy

Watchly is designed to keep the user's personal library and watch progress locally on the device.

The application does not require an account for the local library.

A separate privacy policy will be provided before Google Play publication where required by Google Play policies.

## Status

Watchly is under active development.

The repository may contain prototype code while the application is being prepared for its first public release.

## Disclaimer

Watchly is an independent application and is not affiliated with, endorsed by, or certified by The Movie Database (TMDB).

TMDB names, logos, data and images remain subject to their respective rights and terms.

## Contact

For project issues and development discussions, please use the GitHub repository's Issues section.

---

**Watchly** · Track what you watch. Know what remains.
