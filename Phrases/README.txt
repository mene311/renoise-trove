MODULAR PHRASE LIBRARY — 5,028 phrases
========================================
Renoise 3.5.x · plain-XML phrase presets (.xrnz) · LPB 4 (1 line = 1/16) ·
Loop on · Pattern mode · BaseNote C-4 (48) · KeyTracking = TRANSPOSE
=> everything layers, everything transposes with the key you play.

FOLDERS — renumbered 2026-09-08 (unique & sequential 00-21)
-----------------------------------------------------------
00_Originals (3)         Jupiter, Dorian Arp + multiprogram example (yours)
01_Planets (40)          Sun..Pluto character themes + V2/V3/V4 variants
02_Elements (16)         Earth/Water/Fire/Air + variants
03_Seasons (16)          Spring/Summer/Autumn/Winter + variants
04_Nature (16)           Ocean/Forest/Desert/Mountain + variants
05_Moods (16)            Joy/Sorrow/Rage/Calm + variants
06_Bass_Lines (10)       grooves: chug, pump, 5th-pop, walks, 3-3-2, reggae…
07_Arpeggios (11)        Maj7/Min7/Dom7/Add9/Sus2/Dim7, 16th ripple, broken 10ths…
08_Chords (10)           multi-column: stabs, pads, I-vi-IV-V, ska, power 5ths…
09_Rhythms_Syncopation (10)  3-3-2, son clave 3-2/2-3, backbeat, offbeat, gallop…
10_FX_Texture (8)        shimmer, trill, delay echo, riser/fall, clock, heartbeat
11_Riffs_Motifs (12)     genre riffs (blues/funk/techno/synthwave/drill…)
12_Melody_Ideas (48)     8 moods x6, 64-line half-tempo versions
13_MIDI_Bach_Chorales (468)    soprano melodies, real titles -> Chorales 1-3
14_MIDI_Bach_Basslines (2858)  chorale basses -> Bases / Windows W2+W3 /
                    Variants V2+V3+V4, each split into ~170-file parts
15_MIDI_Irish_Folk (1195)      monophonic Irish trad -> Folk 1-5
16_Ableton_Melodies (230)      Ableton tonal clips -> Basslines/Melodic/Chords/Singles parts
                    !! licensed pack, personal use only — NEVER push/distribute
17_Dark_Synth (13)       dubstep/neuro: riffs, growl basslines, pad chords
18_Latin (12)            8 melodic + 4 chord phrases, Latin motifs
19_RnB_Dark (12)         dark neo-soul / low-light R&B
20_Happy (12)            upbeat pop/bounce
21_Wild (12)             experimental/psychedelic
Root: 13_MIDI_Bach_COMMENTARY.txt (344 chorales: meter/range/BWV)

SUBFOLDER RULE: keep any phrase folder <= ~240 files — Renoise's browser gets
slow parsing thousands. Re-run subdividing after any regeneration.

PROGRAM-CHANGE PLAYBOOK (one patch, many programs)
- Load a family's phrases into phrase slots IN ORDER -> each = a program.
- Automate Zxx in patterns or MIDI program changes: Z01.. = program 1.., Z00 off, Z7F keymap.
- Families ship as base + V2 Sparkle (+1 oct) / V3 Retro (reversed) / V4 Half (sparse).
- Mix speeds: 32-line (2-bar) riffs vs 64-line (4-bar) melodies/basses.

SOURCES & LICENSES
- 16_Ableton_Melodies: your licensed Ableton pack (Tonal/MIDI Clips) - personal use only.
- 13/14/15_MIDI: public domain Bach chorales (infinite-bach corpus, jsbchorales.net
  codes; titles via Riemenschneider/DCMLab) + Irish trad CC-BY corpus
  (Ceol Rince na hÉireann / Polifonia). Commentary file gives meter/range/BWV.
- 00-12 + 17-21: generated originals (AI-assisted); humanized where noted
  (velocity + micro-delay).

HOW IT WAS BUILT (all in _tools/)
- alc2phrase.py: Ableton 12 .alc (gzip XML) -> phrases. NOTE: pitch lives in
  <KeyTrack><MidiKey Value/>, NOT on the events or the KeyTrack Id.
- midi2phrase.py: MIDI -> phrase. env: SRC_DIR OUT_DIR MIDI_MAX TRACK=melody|bass
  START_BEAT (windows) NAME_SUFFIX MAP_FILE HUMANIZE. Trims lead-in to line 0,
  keeps velocity -> hex volume, optional humanization (delay ticks).
- melody_ideas.py: seeded generator, stats-tuned (density, intervals, no repeats).
- variants64.py: V2/V3/V4 for 64-line files (basses). _build_variations.py: 32-line.
- make_original_packs.py: genre packs 18-21 engine (motif+consequent, seeded).
- make_motifs.py, reroll_all.py, make_simple_insts.py, make_sm_parts.py,
  sfz2xrni.py: riff pack, theme re-roll, sample instruments, per-part drums.
- backup/: pre-v2 takes of the crafted folders (pull any single old file back).
