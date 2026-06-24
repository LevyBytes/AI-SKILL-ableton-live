---
name: ableton-live
description: Use when working with Ableton Live 12 (the DAW): the Arrangement and Session views; clips and the Clip View; audio warping and tempo; MIDI and MPE editing; MIDI tools; converting audio to MIDI; comping; stem separation; recording; routing and I/O; mixing; automation and clip envelopes; instrument/drum/effect racks; the browser and managing files/sets; Live's built-in instruments, audio effects, and MIDI effects; Max for Live; Push 1 and Push 2; Link/tempo sync; tuning systems; keyboard shortcuts; and accessibility. The official Live 12 Reference Manual. Not for other DAWs.
---

# Ableton Live 12 Reference

Faithful reference for Ableton Live 12, split into one focused file per subject across 78 reference files.
Identifiers (API/type/function names, flags, paths, enums, numbers) are preserved verbatim.

## When to use this

Use this skill when the task involves Ableton Live 12 — the Arrangement and Session views, clips, audio warping and tempo, MIDI and MPE editing, MIDI tools, audio-to-MIDI conversion, comping, stem separation, recording, routing and I/O, mixing, automation and clip envelopes, instrument/drum/effect racks, the browser and managing files and sets, the built-in instrument/audio-effect/MIDI-effect references, Max for Live, Push 1 and Push 2, Link and tempo sync, tuning systems, keyboard shortcuts, and accessibility.

## Workflow

1. Open `references/INDEX.md` (or `references/topics.json`) and pick the one file that matches.
2. Read only that file; open another only if the task spans subjects. Grep across files when needed: `rg -n "PATTERN" references/*.md`.
3. Treat every identifier as an exact reference fact — never invent or paraphrase.

## Gotchas

Recurring failure modes and what to do instead live in the sibling [GOTCHA.md](GOTCHA.md).

## References

All depth lives in `references/` — start at `references/INDEX.md`, metadata in `references/topics.json`. One subject per file.

## Verification

```powershell
python .agents/skills/skill-drafting/scripts/validate_skill_package.py D:/dev/SKILLS/AI/work/recon-staged/working/ableton-live
```
