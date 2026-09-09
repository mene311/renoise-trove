RENOISE PHRASE LIBRARY — curated edition (400 shipped + 230 local-only)
========================================================================
Renoise 3.5.x · plain-XML phrase presets (.xrnz) · LPB 4 (1 line = 1/16) ·
Loop on · Pattern mode · BaseNote C-4 (48) · KeyTracking = TRANSPOSE
=> everything layers, everything transposes with the key you play.

CURATED 2026-09-08: removed the giant MIDI corpora (Bach basslines 2,858,
Irish folk 1,195, full chorales 468). Corpus archives live in
~/Projects/renoise/_archive/phrases-corpus-2026-09-08/ and are still
regenerable from _tools/ (midi2phrase etc). Shipped content is now ~97% ours.

FOLDERS
-------
00-12   original/generated: themes (Planets/Elements/Seasons/Nature/Moods),
        bass lines, arps, chords, rhythms, FX, riffs, melody ideas  (216)
13_Classics (123)   famous Bach chorale melodies (public domain), curated
        sampler of the 468-file corpus — titled: Wachet auf, Jesu meine
        Freude, O Haupt, Nun komm, Befiehl du deine Wege, Vom Himmel hoch…
14_Dark_Synth (13)  dubstep/neuro riffs, growl basslines, pad chords
15_Latin (12)       8 melodic + 4 chord phrases, Latin motifs
16_RnB_Dark (12)    dark neo-soul / low-light R&B
17_Happy (12)       upbeat pop/bounce
18_Wild (12)        experimental/psychedelic
99_Ableton_Melodies (230)  local-only licensed Ableton pack clips — NEVER push

SUBFOLDER RULE: keep any phrase folder <= ~240 files.

PROGRAM-CHANGE PLAYBOOK
- Load a family's phrases into phrase slots IN ORDER -> each = a program.
- Automate Zxx or MIDI program changes: Z01.. = program 1.., Z00 off, Z7F keymap.
- Mix speeds: 32-line (2-bar) riffs vs 64-line (4-bar) melodies/basses.

SOURCES & LICENSES
- 00-12 + 14-18: generated originals (AI-assisted), humanized where noted.
- 13_Classics: public-domain Bach chorale melodies (our transcriptions from
  the infinite-bach / Riemenschneider corpus). Full corpus + commentary
  archived (see above).
- 99_Ableton: licensed pack, personal use only.

BUILDERS: _tools/ (alc2phrase, midi2phrase, melody_ideas, variants64,
make_original_packs, etc.). Corpus regen: point SRC/OUT envs at the archive.

NEW (2026-09-09)
- 19_PD_Ragtime (10)  Scott Joplin classics (public domain, Mutopia transcriptions):
  Maple Leaf, The Entertainer, Bethena, Magnetic Rag, Sugar Cane…
- 22_Reggae_Roots (12) original reggae/roots basslines (ours)
- 23_Salsa_Son (12)    original son/tumbao basslines (ours)
- 24_Boogie_Blues (12) original boogie-woogie walking lines (ours)
- PENDING: 20_PD_Early_Jazz, 21_Trad_Dance (sources blocked this round;
  see handoff: early-jazz via piano-roll site needs session; trad site has no
  direct .mid links — alternate sources planned).
