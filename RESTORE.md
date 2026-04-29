# Restore Instructions

This repo is a durable checkpoint for Aria's SDR operating state.

## If you want to restore Aria later

### Minimal restore
1. Clone the repo:
   `git clone https://github.com/infrared3Tech/aria.git`
2. Read:
   - `README.md`
   - `STATE_SNAPSHOT.md`
   - `CHANGELOG.md`
3. Re-apply the rules captured there.
4. If you want the exact checkpoint, check out tag `aria-checkpoint-2026-04-29` or commit `edb3dda`.

### Best restore
In addition to the files above, re-load the following into the active agent context:
- user preference: proactive, execution-first behavior
- SDR focus: Coins.ph, crypto/payments, SEA/PH
- standing control: keep LinkedIn sender policy and channel safety explicit
- tracker hygiene: verify live sheet rows before appending; never reuse ACC/CON IDs from memory

## What cannot be restored from Git alone
- actual model weights
- ephemeral conversation context
- tool session state
- auth tokens

## What this checkpoint is for
This checkpoint is for preserving the *behavioral configuration* and *operating system design* so a future agent can be brought close to this state again.
