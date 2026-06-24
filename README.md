# Ableton Live 12 Reference Manual Skill

A reference skill for **[Agent Kaizen](https://github.com/DirectorGunner/agent-kaizen)** covering the official Ableton Live 12 Reference Manual (the DAW). The prose is original (recontextualized); identifiers — device and parameter names, menu paths, key/mouse shortcuts, enum values, numbers, and units — are preserved exactly.

## What this skill covers

This skill is a faithful reference for Ableton Live 12. It covers the Arrangement and Session views; clips and the Clip View; audio warping and tempo; MIDI and MPE editing, MIDI tools, audio-to-MIDI conversion, and comping; stem separation; recording, routing and I/O, mixing, automation and clip envelopes; instrument, drum, and effect racks; the browser and managing files and sets; Live's built-in instruments, audio effects, and MIDI effects; Max for Live; Push 1 and Push 2; Link/tempo sync; tuning systems; keyboard shortcuts; and accessibility. It is a flat skill: a single `SKILL.md` plus a `references/` library of one focused topic file per subject (78 files). It is not for other DAWs.

## What's inside

- `SKILL.md` — the trigger description, when-to-use, workflow, and routing into the references library.
- `references/` — right-sized topic files (one subject per file, 78 reference files) plus `INDEX.md` (start here) and `topics.json` (metadata).
- `GOTCHA.md` — recurring failure modes and what to do instead.

## Status

Recontextualized into original prose (identifiers preserved); packaged in the skills store and ready to publish as the public `AI-SKILL-ableton-live` repository. Publication is performed by the maintainer.

## Reducing idle context cost (skill invocation policy)

Every installed skill costs a little context on every session: the agent sees each skill's name and description before you ever use it. If you rarely use this skill in a given project, you can keep it installed and still explicitly invocable while hiding it from the model's automatic listing.

Doing so does **not** modify this skill's source repo — the policy lives in your local agent settings. The Agent Kaizen **[skill-drafting](https://github.com/DirectorGunner/AI-skill-drafting)** repo ships a manager, `scripts/skill_policy.py`, that sets this for all your skills at once:

```bash
python skill_policy.py audit     # list every skill + its current policy + idle cost
python skill_policy.py plan      # write a decision file with recommendations (nothing applied)
# edit that decision file: set selected_policy + approved:true for the skills you choose
python skill_policy.py preview   # show the exact change
python skill_policy.py apply     # apply ONLY what you approved (backup + rollback recorded)
python skill_policy.py restore   # roll back
```

- **Claude Code (works today):** writes `skillOverrides: { "<skill>": "user-invocable-only" }` to `.claude/settings.local.json` — zero idle listing cost, still available from the `/skills` menu. Start a new session for it to take effect; invoke it any time via `/skills`.
- **Codex (currently unreliable):** explicit-only Codex skills are affected by an open bug ([openai/codex#23454](https://github.com/openai/codex/issues/23454)) where `$skill` invocation of an explicit-only local skill can fail. Until it's fixed, leave Codex skills implicit, or fully disable rarely-used ones with `[[skills.config]] enabled = false` in `config.toml`. The manager audits Codex but does not change Codex policy.
