# Lisen: The Audiophile's Local Player

## Concept
**Lisen** is born from the idea that local music libraries deserve the same level of care and aesthetic excellence as streaming services, but with the uncompromising quality that only local lossless files can provide. It's not just a music player; it's a high-fidelity experience tailored for the modern Android ecosystem.

## Vision
The vision for Lisen is to bridge the gap between technical audiophile tools and beautiful, accessible consumer apps. We believe you shouldn't have to sacrifice a beautiful UI to get Bit-Perfect audio output.

## Core Pillars
1. **Purity of Sound**: Leveraging Jetpack Media3 and advanced audio routing to ensure that what you hear is exactly what was recorded. Support for specialized DACs via high-resolution output pathways.
2. **Immersive Aesthetics**: A design language based on "Glassmorphism" and "Material You," creating a sense of depth and focus on the album art.
3. **Smart Management**: Intelligent scanning of local storage with deep metadata support, ensuring your library is always organized and beautiful.
4. **Performance**: Built with Jetpack Compose and Kotlin Coroutines for zero-lag interactions, even with libraries containing thousands of FLAC files.

## High-Level Architecture
Lisen follows the **Clean Architecture** principles:
- **UI Layer**: Jetpack Compose with a focus on micro-interactions.
- **Domain Layer**: Pure Kotlin logic defining the business rules of music playback and library management.
- **Data Layer**: Room for caching metadata, and Media3 for the heavy lifting of audio decoding and playback.

## Why "Lisen"?
The name is a playful, minimal take on "Listen." It represents our focus on the core act of music appreciation—stripping away the noise and focusing on the sound.
