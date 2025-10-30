# Music Notes App

A concise React + TypeScript web app for entering musical notes, choosing an instrument, and playing the sequence using bundled audio samples. The app also provides a simple visual representation of the entered notes on a staff.

## Overview
This project demonstrates a lightweight, user-facing interface that maps textual note input to pre-recorded audio samples. Users can switch between available instruments and hear the sequence played back while seeing the notes rendered visually.

## Key features
- Instrument selection (Guitar, Piano).
- Enter notes as space-separated tokens (supported notes: C D E F G A B).
- Playback of each note using MP3 samples included under public/instruments.
- Simple staff visualization of entered notes.

## Project structure
music-notes-app/
- public/
  - index.html
  - instruments/
    - guitar/ (C.mp3, D.mp3, E.mp3, F.mp3, G.mp3, A.mp3, B.mp3)
    - piano/  (C.mp3, D.mp3, E.mp3, F.mp3, G.mp3, A.mp3, B.mp3)
- src/
  - App.tsx
  - index.tsx
  - styles.css
- tsconfig.json

## Important files
- public/index.html — application entry HTML.
- src/App.tsx — core logic for parsing notes, instrument selection, audio playback and visual rendering.
- src/index.tsx — React bootstrap and mounting point.
- src/styles.css — UI styling and basic layout.

## Usage (what the app does)
- Select an instrument from the dropdown.
- Type a sequence of notes separated by spaces (for example: `C D E F G`).
- Click the "Play Notes" control to hear the sequence and view the notes on the staff.

## Notes
- Audio samples are expected under public/instruments/<instrument> and must be named by note (e.g., C.mp3).
- Supported note names in the UI are the natural notes C, D, E, F, G, A, B. The app uses the provided MP3 samples for playback.
- If audio does not play, check browser audio/autoplay policies and console messages.

