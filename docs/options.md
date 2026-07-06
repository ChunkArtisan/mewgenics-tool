# Options reference

## Trainer

| # | Option | Type | Notes |
|---|--------|------|-------|
| 0 | Activate Trainer | Master toggle | Required for all trainer modules |
| 1 | Unlimited HP | Toggle | Applies to player-controlled units |
| 2 | Unlimited MP | Toggle | MP costs ignored |
| 3 | One Hit Kill | Toggle | Combat only |
| 4 | Unlimited Item Uses | Toggle | Items and consumables |
| 5 | Instant Win | Action | Ends current encounter |
| 6 | Unlimited Attacks | Toggle | Per-turn attack limit removed |
| 7 | Unlimited Moves | Toggle | Per-turn movement limit removed |

## Save editor

| # | Option | Scope |
|---|--------|-------|
| 8 | Edit: Coins [Adventure] | Active adventure save |
| 9 | Edit: Food [Adventure] | Active adventure save |
| 10 | Edit: Coins [Home] | Home / hub save |
| 11 | Edit: Food [Home] | Home / hub save |

## Recommended workflow

1. Back up `%USERPROFILE%\AppData\LocalLow\<Company>\Mewgenics\` (path varies by build).
2. Use **Save Editor** with the game closed.
3. Use **Trainer** with the game running and **Activate Trainer** enabled.
4. Disable modules before saving if you want unmodified stat progression.

## Safety

- Save editor changes are immediate on apply.
- Trainer hooks are runtime-only unless paired with save edits.
- Not affiliated with the original game developers.
