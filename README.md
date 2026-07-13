# Orel Ohayon

Self-taught builder out of Israel. I work top-to-bottom — Chromium internals and
Wine→Metal translation at the metal, Hebrew-first web and real-time infra at the
surface — and ship the whole thing myself.

### Live

- **[Azaka](https://azaka.orellius.ai)** — real-time Red Alert map for Israel.
  Official Pikud HaOref alerts rendered live: threat zones on the map, per-city
  shelter countdowns, four locales, plus a Telegram channel and per-city bot.
- **[Glyphcast](https://glyphcast.tv)** — video as text. A typography-only
  codec: every frame is Unicode glyphs + color, so a browser, a terminal, or
  even an LLM can decode and *see* the video. Open core below.

### Open source

- **[glyphcast-core](https://github.com/Orellius/glyphcast-core)** — the
  typography codec itself. GPU-rendered in one draw call, lossless on a
  byte-aligned wire, zero runtime deps. Apache-2.0.
- **[opendisplay](https://github.com/Orellius/opendisplay)** — HiDPI
  resolutions macOS hides on sub-4K monitors on Apple Silicon. Swift, no kernel
  extension.

### Stack

Rust · Swift / AppKit · C++ → wasm · TypeScript / Next.js · Tauri 2 · Three.js

---

[orellius.ai](https://orellius.ai) · orel@orellius.ai
