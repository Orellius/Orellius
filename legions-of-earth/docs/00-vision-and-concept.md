# 00 — Vision & Concept: *Legions of Earth*

> **Status:** Anchor document. Every other document in this repository builds on the concepts, terminology, and pillars defined here. If another document conflicts with this one, this one wins until explicitly amended.

---

## 1. What we are building — in one paragraph

**Legions of Earth** (working title, "LoE") is a **free, browser-based, massively-multiplayer territory-control strategy game** played on a single persistent, stylized map of Earth. Every player is a **Commander** leading a small warband; real power comes from joining a **Legion** — a player-run company of up to 100 Commanders — and coordinating with Legions across the globe to capture and hold **Provinces** through **Seasons** that last roughly eight weeks before the world resets. It is designed from day one for a **worldwide audience**: no install, under-5-MB initial load, playable in meaningful 5-minute sessions on a mid-range phone over 3G, localized into 20+ languages with built-in cross-language chat translation, priced regionally, and monetized only through cosmetics and convenience — never power.

### Genre reference

The project is inspired by the spirit of small viral persistent web games such as **legionnaire.xyz** — a shared world, low-friction entry through a URL, and emergent mass cooperation. This plan treats it as a *genre reference* (persistent browser world, legion-based mass multiplayer, territory conquest), not a feature checklist. Legions of Earth is an original design.

---

## 2. Core fantasy

> *"I opened a link on the bus, and now four thousand strangers and I hold the Andes."*

The player fantasy is **belonging to something enormous that notices you**. One Commander cannot take a Province. A Legion can. A coalition of Legions can take a continent. The game makes an individual 5-minute contribution — a supply run, a scouting report, a wall repaired at 3 a.m. in your time zone while your Legion-mates sleep in theirs — visibly matter to a planet-scale campaign.

Because the player base is global, the world never sleeps. **Time zones are a game mechanic**: a Legion with members in São Paulo, Lagos, Warsaw, and Manila can keep watch around the clock; one clustered in a single country has a nightly blind spot. Worldwide reach is not just an audience goal — it is a competitive advantage inside the game.

---

## 3. Design pillars

Every feature decision is tested against these five pillars, in priority order:

1. **One shared world.** A single persistent Earth per Shard. Thousands of concurrent players see the same map state. No private instances of the core game.
2. **Legion first.** Cooperation is the core verb. Solo play is a viable on-ramp, but the design pushes every player toward a Legion within their first three sessions, and every meaningful strategic act is collective.
3. **Five minutes matter.** Every session length is respected. A 5-minute check-in accomplishes something visible; a 2-hour siege evening is a peak experience, not a requirement. All timers and mechanics are async-friendly.
4. **Worldwide by design.** Localization, low-end devices, low bandwidth, regional pricing, worldwide payment methods, time-zone fairness, and cultural neutrality are launch requirements, not post-launch patches.
5. **Fair free-to-play.** Spending money buys identity (cosmetics), story (battle pass), and comfort (convenience) — never combat power, never territory. This is a hard line.

---

## 4. The game in outline

### 4.1 The world

- The map is a **stylized hex-tiled Earth** of roughly **40,000–60,000 land Provinces**, generated from real geography (coastlines, mountains, rivers, biomes) but **deliberately free of modern political borders, country names, and flags**.
- Provinces have **biomes** (steppe, forest, desert, highland, coast, tundra, jungle) that determine resources, movement cost, and defensive value.
- **Supply lines** are central: a Province can only be held if it traces an unbroken friendly path to a Legion **Stronghold**. Deep raids are possible; deep occupation is not. This keeps front lines legible and comebacks possible.
- A **Shard** is one complete copy of the world with a target population of **~100,000 registered Commanders / ~15,000 peak concurrent**. New Shards open as population grows; Shards are region-agnostic (players choose any Shard; latency matters little in an async-first design).

### 4.2 The player: Commander and warband

- Each player is a **Commander** with a persistent identity, and per-Season: a **warband** of units, a doctrine loadout, and a home Province.
- Units are trained with **real-time timers** (minutes to hours), recruited from archetypes: *Shieldline* (hold), *Skirmishers* (harass), *Riders* (mobility), *Engineers* (siege/build), *Wayfinders* (scout/logistics).
- **Doctrines** are pre-set orders (formation, aggression, retreat thresholds) — combat resolves **server-side and asynchronously** in short deterministic auto-battles that players can replay as visualizations. No twitch skill, no latency advantage: strategy, preparation, and coordination decide fights.
- Player verbs, all completable in under five minutes: move/queue orders, train, build, repair, scout, escort a supply run, reinforce a garrison, vote, chat, plan.

### 4.3 The Legion

- A **Legion** is a named, player-founded company of up to **100 Commanders**, with a banner, colors, ranks (Legate, Officers, Veterans, Recruits), shared treasury, and a Stronghold.
- Legions form **Coalitions** (up to 10 Legions) with shared objectives, diplomacy (alliances, non-aggression pacts, tribute), and a coalition map layer for planning.
- **Fictional banners, not nations.** All faction identity in the game is invented (e.g., the *Aurelian Legion*, the *Ashen Horde*, the *Tidewalkers*, the *Verdant Pact*) with mythic-historical flavor drawn respectfully from many world cultures. Players may not register Legions that represent real countries, ethnic groups, or political movements — a Trust & Safety rule enforced at naming and reporting level. The game is about holding *terrain on a map of Earth*, never about "my country versus yours."

### 4.4 Conflict and fairness across time zones

- **Skirmish layer (always on):** raids, scouting, supply interdiction resolve continuously and asynchronously.
- **Clash Windows (scheduled):** decisive siege battles for Strongholds and capital Provinces occur in pre-declared 24-hour windows during which both sides accumulate contribution; the resolution moment **rotates across time zones** by rule so no region is structurally advantaged. Defenders schedule within constraints; attackers get notice.
- **New-player protection:** fresh Commanders spawn under a 7-day shield in low-conflict frontier zones; Provinces held by very small/new Legions have attack-cost multipliers.

### 4.5 Seasons and legacy

- A **Season** lasts **~8 weeks**, ending in a scored finale (territory, objectives, event victories). The map then **resets** with fresh geography variations.
- **Legacy persists:** Commander profile, cosmetics, titles, battle honors, Legion history, and the **Hall of Ages** (permanent monument records of past Seasons' great deeds — visible in-world).
- Seasons carry a light **narrative arc** (world events: comet winters, migrations, ancient ruins awakening) that redraws strategic incentives mid-season and gives lapsed players a reason to return.

### 4.6 Economy

- Resources (grain, timber, stone, iron, silver) are produced by Provinces, moved along supply lines, and consumed by training, building, and upkeep. Sinks are strong; hoarding decays.
- A **player-driven regional market** lets Legions trade; trade routes are physical and raidable, making commerce a strategic surface, not a menu.

---

## 5. Worldwide-audience requirements (non-negotiable at launch)

| Area | Requirement |
|---|---|
| **Access** | Playable from a URL in any modern browser; installable as a PWA; no app store required (store wrappers may come later). |
| **Performance** | Initial interactive load **< 5 MB / < 10 s on 3G**; playable on a 2 GB-RAM Android phone from 2019; data-saver mode. |
| **Languages** | 20+ languages at launch (see doc 07), including RTL (Arabic) and full CJK support; community translation program for the long tail. |
| **Chat translation** | Built-in machine translation in Legion/Coalition/diplomacy chat, so a Legion can span languages. |
| **Time-zone fairness** | Rotating Clash Windows; asynchronous core loop; no mechanic that rewards being awake at a specific UTC hour. |
| **Pricing & payments** | Regional (PPP-informed) pricing; support for cards, PayPal, Pix, UPI, M-Pesa-style mobile money, carrier billing, and prepaid codes via aggregators (see doc 06). |
| **Cultural neutrality** | No real-world political borders, flags, or modern nations; fictional banners; global-holidays event calendar that celebrates broadly without appropriating (see docs 05 and 10). |
| **Compliance** | GDPR/CCPA/LGPD-grade privacy by default; age gates; per-country monetization law compliance (see doc 12). |
| **Accessibility** | WCAG 2.2 AA target: colorblind-safe map palettes, screen-reader-navigable menus, no reflex-dependent gameplay (see doc 09). |

---

## 6. Business model in one paragraph

Free to play, funded by: **cosmetics** (banners, unit skins, Stronghold architecture styles, map flair, victory monuments), a **seasonal Warpath Pass** (battle pass: cosmetic + QoL track, earnable premium currency), and **convenience** (extra order queues, build-queue slots, cosmetic loadouts — capped so free players reach the same caps through play). **Hard exclusions:** no purchasable resources, units, speed-ups of combat-relevant timers beyond the free cap, territory, or gacha/loot boxes anywhere. Regional pricing everywhere. Target: modest ARPPU across a very wide, worldwide funnel rather than whale-hunting (details and projections in doc 06).

---

## 7. Technology in one paragraph

TypeScript end-to-end. Client: WebGL canvas map renderer (PixiJS-class) + React UI shell, delivered as a PWA from a global CDN. Server: authoritative deterministic simulation, sharded by world region into actor-style processes, with WebSocket push for live layers and plain HTTPS for async actions; PostgreSQL system-of-record, Redis-class cache/queues, edge presence worldwide. Deterministic battle resolution enables tiny replay payloads and server-authoritative anti-cheat. Target: one Shard ≈ 100k registered players / 15k CCU on a modest cost envelope (full architecture, alternatives, and cost model in doc 04).

---

## 8. Shared vocabulary (use these terms everywhere)

| Term | Meaning |
|---|---|
| **Commander** | A player. |
| **Warband** | A Commander's units for the current Season. |
| **Legion** | Player-run company of up to 100 Commanders. |
| **Coalition** | Alliance of up to 10 Legions. |
| **Province** | One hex territory on the map. |
| **Stronghold** | A Legion's anchor structure; root of its supply. |
| **Supply line** | Unbroken friendly path from Province to Stronghold. |
| **Skirmish layer** | The always-on asynchronous conflict system. |
| **Clash Window** | Scheduled 24-hour decisive-battle window, time-zone rotated. |
| **Season** | ~8-week world cycle ending in reset + legacy awards. |
| **Hall of Ages** | Permanent cross-Season monument/history system. |
| **Shard** | One complete instance of the world. |
| **Warpath Pass** | The seasonal battle pass. |
| **Doctrine** | A Commander's pre-set combat orders/loadout. |

---

## 9. Success criteria (v1 targets, 12 months post-global-launch)

- **Reach:** 5M registered accounts across ≥ 60 countries; no single country > 30% of MAU.
- **Retention:** D1 ≥ 40%, D7 ≥ 18%, D30 ≥ 8% (browser F2P strategy benchmarks; see doc 05/09).
- **Social:** ≥ 55% of D7-retained players in a Legion; median Legion spans ≥ 3 countries.
- **Revenue:** self-sustaining live team by month 12 (model in docs 06 and 13).
- **Performance:** p75 first-interaction < 6 s worldwide, including South Asia, Africa, and South America.
- **Integrity:** < 2% of accounts actioned for botting/multi-boxing per Season, with measured downward trend.

---

## 10. Document map

| Doc | Title | Covers |
|---|---|---|
| 00 | Vision & Concept | This document. |
| 01 | Game Design Document | Core loop, units, combat, progression, balance. |
| 02 | World, Map & Seasons | Map generation, territory, supply, seasons, shards. |
| 03 | Legions, Social & Diplomacy | Legion systems, coalitions, chat, diplomacy, congress. |
| 04 | Technical Architecture | Client, server, sim, data, scaling, costs. |
| 05 | Live-Ops, Content & Analytics | Cadence, events, pipeline, telemetry, experimentation. |
| 06 | Economy & Monetization | In-game economy, F2P model, worldwide pricing & payments. |
| 07 | Localization & Internationalization | Languages, i18n engineering, culturalization, LQA. |
| 08 | Art & UX Direction | Style, UI system, map readability, sound, brand. |
| 09 | Onboarding, Retention & Accessibility | FTUE, retention loops, low-end support, WCAG. |
| 10 | Security, Anti-Cheat & Trust/Safety | Server authority, bots, multi-accounting, moderation. |
| 11 | Marketing, Community & Go-to-Market | Positioning, regional GTM, creators, launch. |
| 12 | Legal, Compliance & Privacy | GDPR-class privacy, age gates, per-country law. |
| 13 | Roadmap, Team & Budget | Phases, milestones, hiring, budget, risks. |
