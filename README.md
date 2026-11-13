# The Haunted — Mary vs Sister Morning

A first-person 3-lane forest runner: run toward the manor, **dodge the trees** (they can't be vaulted), **vault fallen trunks and stone fences**, and stay ahead of Sister Morning, who is rustling through the mist behind you.

## Play

```
open index.html   (double-click works — it's one self-contained file)
```

| Action | Desktop | Mobile |
|---|---|---|
| Change lane | `A`/`D` or `←`/`→` | swipe left / right |
| Vault | `Space` | swipe up, or quick tap |

Trunks and fences: **vault**. Trees: **dodge**. The Sister's rustle grows louder as she closes — when it reaches you, she does. Reach the manor and you win.

## What's inside

- **One file.** All art is embedded as base64 and the music is an embedded MIDI piano score rendered through a Web Audio synth (low, film-music style). The only external dependency is three.js from a CDN, so it needs a network connection on first load.
- **Sound is gesture-locked.** Browsers require a click/tap before audio may start — press **Run** and it comes up with the wind bed, dampened footsteps, and the piano. On iPhone, set the session to *playback* (done in code) so the silent switch doesn't mute it.
- **Mix knobs** (top of the script in `index.html`): `MUSIC_LEVEL`, `MUSIC_TRANSPOSE`, `SFX_LEVEL`, `WIND_LEVEL` — currently tuned to steps ≈ −20 dBFS, music ≈ −29, wind ≈ −45 (background).

## Assets

Source art by **The Legomen** (hand-drawn, near-black silhouettes on solid backdrops):

```
Assets/        generated source images (splash, Mary, Sister Morning, trees, obstacles)
Art Reference/ original references + Haunted_score.abc (the melody behind the piano track)
```

## Versions

- **v0.1** — first playable build (git tag `v0.1`)
