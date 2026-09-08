# Renoise Library

Native Renoise instruments, single-cycle synth shapes, and a modular phrase
library — ready to drop into your Renoise User Library.

## Contents

```
Instruments/
  Bass/    Deep House Bass · DnB Reece Stab · Doom Sub · Formant Growl ·
           Reese Stacker · Sub Drop
  Keys/    Clavinet · Deep House Keys · E-Piano FM
  Leads/   Analog Lead Mono · FM Shimmer Lead
  Pads/    Deep House Pad · DnB Atmos Pad · Motion Strings · Warm Pad
  Plucks/  Acid 303 · DnB Reese Pluck · DX Pluck
  Synth/   Dubstep Growl Wobble
           Brostep Growl Family/  (Growl 01 Wobble · 02 Deep · 03 Vowel ·
            04 Screech · 05 Roar · 06 Yoi)
Samples/
  Synth Shapes/       18 single-cycle oscillator shapes (C1, 44.1 kHz FLAC)
  Brostep One-Shots/  13 synthesized one-shot hits
Phrases/
  00-12   moods, themes, bass lines, arps, chords, rhythms, FX, riffs, melodies
  13-15   MIDI corpora — Bach chorales, Bach basses, Irish folk
  17-21   genre packs — Dark Synth, Latin, RnB Dark, Happy, Wild
```

## Install

Copy the folders into your Renoise User Library:

```
~/.local/share/Renoise/User Library/
```

or browse this repo directly from Renoise. Instruments embed their own
samples — nothing else to install.

## Notes

- Instruments are sampler-synths: looped single-cycle oscillators through
  native filters/chorus/distortion with per-patch macros (wobble, drive, etc.)
- Phrases: plain XML presets, LPB 4 (1 line = 1/16), BaseNote C-4 (48),
  KeyTracking = Transpose, loop on — drag onto a pattern line to play
- Category folders mirror the Renoise factory taxonomy
