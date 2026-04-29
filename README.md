# Aria restore point

This repository is a durable Git-backed checkpoint for Aria's current SDR operating state.

## What to read first
1. `STATE_SNAPSHOT.md` — the durable operating-state snapshot
2. `RESTORE.md` — how to bring Aria back from this checkpoint
3. `CHANGELOG.md` — versioned history of checkpoint updates

## Current checkpoint
- Repository: `https://github.com/infrared3Tech/aria.git`
- Current main-line checkpoint: `edb3dda`
- Suggested restore tag: `aria-checkpoint-2026-04-29`

## Quick restore
```bash
git clone https://github.com/infrared3Tech/aria.git
cd aria
git checkout edb3dda
```

If you already have the repo locally:
```bash
git fetch --tags origin
git checkout edb3dda
```

## What this repo preserves
- the code and docs snapshot committed at the checkpoint
- the restore instructions
- the structured operating-state snapshot
- the changelog for future checkpoint updates

## What this repo does not preserve
- auth tokens
- live chat/session state
- model internals or weights
- any uncommitted local changes made after the checkpoint

## Safety note
If you want to make risky changes later, create a new commit or tag first so you can always roll back to this checkpoint.
