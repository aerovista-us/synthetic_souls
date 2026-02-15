# Synthetic Souls - Digital Music Experience

A cyberpunk-themed music project featuring interactive elements and immersive character lore.

## Features

### Interactive Character Dial
- Circular interface with segments for each band member
- Click on a character segment to reveal their lore in a modal
- Hover effects with character-specific audio cues

### Custom Audio Player
- Unified audio player for all tracks
- **Controls inside the visualizer drop-in**: play/pause, prev, next, volume, progress bar, and time display sit in a standard bar at the bottom of the artwork/visualizer; same layout for every track, with per-track theming (accent colors, progress gradient) to match the song
- Playlist functionality with track navigation
- Album artwork or HTML visualizer display that changes with each track

### Character Lore Modals
- Detailed backstories for each character
- Character statistics and abilities
- Immersive world-building details

### Tracks & Visualizers
Each of the six tracks has a matching HTML visualizer in `assets/Visualizers/`, shown in the player when that track is selected:

| Track | Artist | Visualizer |
|-------|--------|------------|
| Neural Drift | Synthetic Souls | `neural_drift.html` |
| Signal Cascade | Synthetic Souls | `signal_cascade.html` |
| Echo Pulse | Synthetic Souls | `echo_pulse.html` |
| Rhythm Hack | PH4ZE | `rhythm_hack.html` |
| Tremor Bass | VEKTOR | `tremor_bass.html` |
| Ether Bloom | X1NTH | `ether_bloom.html` |

## Directory Structure

```
synthetic-souls/
├── assets/
│   ├── audio/
│   │   ├── neural_drift.mp3
│   │   ├── signal_cascade.mp3
│   │   ├── echo_pulse.mp3
│   │   ├── rhythm_hack.mp3
│   │   ├── tremor_bass.mp3
│   │   └── ether_bloom.mp3
│   └── images/
│       ├── cosmic-tour-poster.png
│       ├── glitch-portraits.png
│       ├── noise-overlay.png
│       ├── soul-clash.png (X1NTH character portrait)
│       ├── soul-reflection.png (VEKTOR character portrait)
│       ├── soul-tiger.png (PH4ZE character portrait)
│       ├── spectrogram-bg.gif
│       ├── synthetic-souls-banner-alt.png
│       ├── synthetic-souls-banner.png
│       └── synthetic-souls-square.png
├── synthetic-souls.css
├── synthetic-souls.html
├── synthetic-souls.js
├── create-character-images.html
└── README.md
```

## Recent Upgrades

1. **Unique Character Art Integration**
   - Each character now has distinct portraits and lore
   - Interactive glitch dial for character selection
   - Enhanced visual effects for character segments

2. **Interactive Lore with Glitch Dial**
   - Circular dial interface with rotating segments
   - Character-specific modal windows with detailed backstories
   - Audio integration with character profiles

3. **Unified Custom Audio Player**
   - Replaced multiple audio players with a single, responsive player
   - Added playlist functionality and track management
   - Enhanced visual feedback for playback status

## Usage

1. Open `synthetic-souls.html` in a modern web browser
2. Explore the character dial by hovering and clicking on different segments
3. Use the custom audio player to navigate through the tracks
4. Read the lore and backstories for the band and characters

## Technical Details

- Built with vanilla HTML, CSS, and JavaScript
- Uses CSS transitions and animations for visual effects
- HTML5 Audio API for sound playback
- Responsive design for various screen sizes

## Credits

Created by AeroVista Labs 