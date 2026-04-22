# Technical Specification & Software Stack

This document defines the architecture and the software tools used to build the **High-Fidelity Music Player**.

## 1. Development Environment
- **IDE**: Android Studio (Ladybug 2024.2.1+)
- **Build System**: Gradle (Kotlin DSL)
- **Version Control**: Git / GitHub

## 2. Frameworks & Libraries

### Core App Logic
- **Kotlin**: The primary language, utilizing Coroutines for non-blocking I/O and Flow for reactive data streams.
- **Jetpack Media3 (ExoPlayer)**: Used for the audio playback engine. It supports high-bitrate audio, lossless formats (FLAC, ALAC), and low-latency rendering.
- **MediaStore API**: Used to query the local file system (Downloads directory) for audio files while respecting Android's Scoped Storage permissions.

### User Interface (UI)
- **Jetpack Compose**: A modern declarative UI toolkit.
- **Material Design 3 (M3)**: Implementing the latest design system from Google for a premium look.
- **Horizontal & Accompanist**: For smooth carousels and pager layouts (e.g., song queue or album covers).

### Data Management
- **Room Persistence Library**: A SQLite abstraction used to cache metadata like playlist data, play counts, and favorites.
- **Datastore (Preferences)**: For storing user settings like EQ presets and theme preferences.

### Architecture
- **Hilt (Dagger)**: For robust Dependency Injection.
- **ViewModel**: To handle UI state and data survive configuration changes.
- **Repository Pattern**: To abstract the data sources (Local Storage + Room DB).

## 3. High-Quality Audio Features
- **ExoPlayer Extensions**: Using the FLAC extension for superior decoding.
- **Audio Attributes**: Configured for `USAGE_MEDIA` and `CONTENT_TYPE_MUSIC` to ensure the Android system grants high-priority audio routing.
- **Volume Normalization**: Optional software-level normalization for a consistent listening experience.

---
*Created by Antigravity AI*
