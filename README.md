# Cave Duel

A tiny browser-based **idle auto-battler / mini fighting game**, designed to run
as a small "corner widget" on a phone. Everything runs in a single HTML file
(sprites are embedded as base64), so there's nothing to install — just open it
in a browser.

> Türkçe: Tarayıcıda çalışan, telefonda köşe widget'ı olarak tasarlanmış mini
> dövüş oyunu. Her şey tek bir HTML dosyasına gömülü (base64), kurulum yok —
> dosyayı tarayıcıda açman yeterli.

## Play

Open **`3.html`** in any modern browser (this is the main game). On desktop you
can test with: `Space` / `Right Arrow` = attack, `Left Arrow` / `Shift` = shield.
On phones the hero fights automatically.

## Files

| File | Description |
|------|-------------|
| `3.html` | **Main game** — health bar, stage names, inventory, skills, shadowed sprites |
| `2.html` | UI 2 — wide world view with a sky/mountain parallax |
| `1.html` | UI 1 — close-up view (transparent background, minimal) |
| `index.html` | Old single-file prototype (archived) |
| `assets/` | Source art files (the game itself uses the embedded copies) |

Each UI keeps its own save under the `caveDuelSave` localStorage key.

## Gameplay

Kill the enemy → the hero runs forward while the terrain and mountains parallax
scroll → reach the next waiting enemy and the fight begins. Enemies come in four
flavors: **ORK** (green), **KIZIL ORK** (red), **GÖLGE ORK** (fast shadow) and
**ALTIN ORK** (gold tank, drops 2× coins).

## Credits & asset licenses

All art is free to redistribute:

- **Character sprites** (hero + all orc variants): original **CC0** pixel art,
  procedurally generated with this project's own *Pixel Hero Maker* tool.
- **Enemy sprites** (goblin / imp / ogre) and **weapon / coin icons**: from
  [0x72 "DungeonTileset II"](https://0x72.itch.io/dungeontileset-ii) — **CC0**.
- **Backgrounds** (`assets/arkaplan/`): _source not yet confirmed — verify the
  license before relying on it commercially._

Source code is licensed under the [MIT License](LICENSE).

## Roadmap

The plan is to grow this from a browser prototype into a real mobile app. See
[ROADMAP.md](ROADMAP.md).
