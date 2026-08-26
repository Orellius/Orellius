## Orel Ohayon

Systems software and agent infrastructure. I instrument what other people estimate.

Everything below is measured, not asserted: the numbers in these READMEs come from a
run you can reproduce, and where a claim could not be measured it is not made.

---

### macOS, native

**[termisu](https://github.com/Orellius/termisu)** &mdash; a terminal emulator written in Swift.
A real shell, real mouse selection, and none of the input paths that a synthetic-event
harness would report as working when they are not. *Swift, 433 commits*

**[OpenDisplay](https://github.com/Orellius/opendisplay)** &mdash; a display control panel in the
menu bar. The HiDPI modes the system generates and then filters out of its own list, plus
brightness that keeps going below the panel's own floor. No driver, no kernel extension. *Swift*

**[Trumpet](https://github.com/Orellius/trumpet)** &mdash; a per-application volume mixer, built
on CoreAudio process taps. One slider per app that is making sound, and nothing is left in
your audio path when you quit it. *Swift*

**[ozen](https://github.com/Orellius/ozen)** &mdash; hold a key, speak Hebrew, release, and clean
text lands in the focused app. Recognition and cleanup both run on-device. *Rust, Tauri*

**[Yayin](https://github.com/Orellius/yayin)** &mdash; run Windows games on a Mac. A native
SwiftUI Wine bottle manager and launcher. *Swift*

### Agents and developer tools

**[octootter](https://github.com/Orellius/octootter)** &mdash; a desktop app that wraps the
`claude` CLI as a subprocess, so hooks, skills and MCP servers keep working while the
permission prompts stop yanking you back into a shell. *TypeScript, Tauri 2, Rust*

**[januas-ade](https://github.com/Orellius/januas-ade)** &mdash; a native-Rust development
environment: a GPU-rendered terminal multiplexer with wizard-driven setup. *Rust*

**[ISQ](https://github.com/Orellius/isq)** &mdash; a tribute to ICQ rebuilt for 2026, where AI
agents are real members of the chat rather than bots in a sidebar, on the same sequential-number
identity primitive. *TypeScript, Tauri*

### Systems and data

**[glyphcast](https://github.com/Orellius/glyphcast)** &mdash; video as text. A typography-only
codec: every frame is a Unicode glyph grid rendered in one GPU draw call, on a byte-aligned wire
format a terminal can decode. 1,248,000 cells at 67 fps, measured. *TypeScript, WebGL2*

**[Azaka](https://github.com/Orellius/azaka)** &mdash; a live Red Alert map for Israel. Official
Home Front Command alerts on MapLibre with per-area shelter countdowns, a Telegram bot and four
locales. It never fakes an impact point, because open data cannot produce one.
*TypeScript, React 19, Bun*

**[orellius-TCM](https://github.com/Orellius/orellius-TCM)** &mdash; a Telegram OSINT monitoring
pipeline: LangGraph agents, local-LLM translation, human-in-the-loop review. Published for study.
*Python*

### Smaller things

**[MEL](https://github.com/Orellius/mel)** &mdash; the Minecraft Enchantment Language. A real
language, with its own lexer, parser and interpreter, whose canonical source form is the
enchanting-table alphabet. *TypeScript*

**[Responsive Viewer](https://github.com/Orellius/responsive-viewer)** &mdash; an MV3 extension
that previews the page you are on at any device resolution, in place. 168 presets, no paywall.
*JavaScript*

**[wisp-adblock-test](https://github.com/Orellius/wisp-adblock-test)** &mdash; a one-screen test
of what your ad blocker, DNS filter or VPN actually catches. An independent continuation of
[Turtlecute33/adblocktest](https://github.com/Turtlecute33/adblocktest), itself a fork of
[d3ward/toolz](https://github.com/d3ward/toolz), under CC BY-NC-SA 4.0. *EJS*

---

Most of the above is **AGPL-3.0**: read it, run it, fork it, and if you run a modified version
as a service, publish that source. The small ones are MIT, and the one continuation keeps the
licence it inherited.

[orel@orellius.ai](mailto:orel@orellius.ai) &nbsp;&middot;&nbsp; [orellius.ai](https://orellius.ai)
