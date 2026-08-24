<h1 align="center">👋 Hey, I'm zeph</h1>
<p align="center">
  <strong>Systems & Security Engineering · Reverse Engineering & Media Preservation</strong>
</p>
<p align="center">
  <a href="https://github.com/ZephyrCodesStuff"><img src="https://img.shields.io/badge/GitHub-ZephyrCodesStuff-181717?style=flat-square&logo=github" alt="GitHub" /></a>
  <a href="https://zeph.work"><img src="https://img.shields.io/badge/Website-zeph.work-c15f3c?style=flat-square" alt="Website" /></a>
  <a href="mailto:noreply@zeph.work"><img src="https://img.shields.io/badge/Email-noreply%40zeph.work-6b665c?style=flat-square&logo=maildotru" alt="Email" /></a>
  <a href="https://github.com/ZephyrCodesStuff/rf64"><img src="https://img.shields.io/badge/Status-Working%20on%20rf64-22c55e?style=flat-square" alt="Status" /></a>
</p>
<p align="center">
  <em>CompEng BSc Student · Building and securing software across the abstraction stack, from low-level firmware and binary reverse-engineering all the way up to scalable cloud systems. Sometimes I revive dead things: games, apps, hardware.</em>
</p>

---

## ⚡ Tech I work with
```text
Languages      ::  Rust 🦀 (Favorite), C / C++, Go, C#, TypeScript, Python
Binary & Rev   ::  IDA Pro, Ghidra, Jadx/Baksmali, GDB/LLDB
Platforms & OS ::  Arch Linux, NixOS, Debian (UKIs, LUKS2, TPM2), macOS / Metal
Cloud & Infra  ::  Google Cloud (GCP), Amazon AWS, Kubernetes, Docker
Databases      ::  MongoDB, SQLite, Redis
```
---
## 🛠️ Projects I work on
| Project | Domain | Description |
| :--- | :--- | :--- |
| [**Destination Home**](https://destinationhome.online/) | **Media Preservation** | Open-source preservation project (16,000+ members) for Sony's defunct *PlayStation Home* on PS3. Reverse-engineered game binaries, built custom API servers, and managed infrastructure. |
| [**rf64**](https://github.com/ZephyrCodesStuff/rf64) | **Bare-Metal Firmware** | Hyper-optimized bare-metal firmware for the MIDI Fighter 64 music controller. Runs on an ATmega32U4 chip with 28 KB flash and 2.5 KB SRAM. |
| [**Halo / rtaudio**](https://halowave.app) | **macOS / DSP** | Real-time audio waveform app for macOS using <1% CPU for 120 FPS rendering via custom DSP chain and a Metal renderer ([source](https://github.com/ZephyrCodesStuff/rtaudio)). |
| [**RPCS3 Sony Clans**](https://github.com/RPCS3/rpcs3/pull/17835) | **Emulation / PSN** | Full reverse-engineering and client + server reimplementation of the defunct Sony Clans PSN subsystem for PS3 and RPCS3. |
| [**hdk-rs**](https://github.com/ZephyrCodesStuff/hdk-rs) | **Rust / High-Perf** | High-performance toolchain for PS3 archive formats (SHARC, segmented zlib) accelerated with Intel ISA-L SIMD — ~300x faster than legacy tools ([CLI](https://github.com/ZephyrCodesStuff/hdk-cli)). |
---
## 🎮 Everything I wrote for PlayStation Home

Complete list of every repository that I've created and maintained for my PlayStation Home revival, "Destination Home".

> [!NOTE]
> Many of these are closed source because either (or both):
> - They might have major contributions from other people (thus I cannot open them without their permission)
> - There are security concerns with opening them (reducing the attack surface may be difficult or impossible)
>
> **Everything that is open is licensed AGPLv3**.

### Repos under my personal account (ZephyrCodesStuff)

| # | Repository | Type | Language | Description |
| :-: | :--- | :--- | :--- | :--- |
| **01** | [`hdk-rs`](https://github.com/ZephyrCodesStuff/hdk-rs) | Library | `Rust` | Blazing-fast Sony/Home archive unpacker, repacker & crypto suite. Everything to develop for Home. |
| **02** | [`hdk-cli`](https://github.com/ZephyrCodesStuff/hdk-cli) | CLI | `Rust` | Cross-platform CLI binary for the `hdk-rs` toolchain, with MCP support. |
| **03** | [`mallory-rs`](https://github.com/ZephyrCodesStuff/mallory-rs) | CLI | `Rust` | Simple development reverse proxy with automatic TLS support; made for PlayStation Home development. |
| **04** | `kitsune` | Gateway | `Rust` | TCP/UDP real-time event gateway (RT / Medius implementation) for PlayStation Home. |
| **05** | `kitsune-emu` | CLI | `Rust` | PlayStation Home player emulator: support for logging in, passing anti-cheat checks and joining a lobby. |
| **06** | `dh-cli` | CLI | `Rust` | Destination Home infrastructure management CLI, with MCP support. |
| **06** | [`psh-docs`](https://psh-docs.vercel.app) | Website | `TypeScript (NextJS)` | Complete, unbiased source of truth regarding every technical aspect of PlayStation Home. |
| **07** | `blahaj` | Monorepo | `Rust` | The predecessor of `hdk-rs`. |
| **08** | `blahaj-core` | Library | `Rust` | Core library powering `blahaj`; what then turned into `hdk-rs`. |
| **09** | `tss-rs` | API | `Rust` | API server for PlayStation Home. Handles the initial login flow. |
| **10** | `ssfw-rs` | API | `Rust` | API server for PlayStation Home. Handles player authentication and accounts. |

### Repos under the Destination Home org

| # | Repository | Type | Language | Description |
| :-: | :--- | :--- | :--- | :--- |
| **11** | [`game-ohs`](https://github.com/DestinationHome/game-ohs) | API | `Rust (Actix)` | API server for PlayStation Home. |
| **12** | [`game-xi`](https://github.com/DestinationHome/game-xi) | API | `Rust (Actix)` | API server for PlayStation Home. |
| **13** | [`game-veemee`](https://github.com/DestinationHome/game-veemee) | API | `TypeScript (Hono)` | API server for PlayStation Home. |
| **14** | [`game-juggernaut`](https://github.com/DestinationHome/game-juggernaut) | API | `TypeScript (Hono)` | API server for PlayStation Home. |
| **15** | [`game-heavywater`](https://github.com/DestinationHome/game-heavywater) | API | `TypeScript (Hono)` | API server for PlayStation Home. |
| **16** | `game-http-cdn` | API | `TypeScript (Hono)` | API server for PlayStation Home, handling various minor minigames in one service. |
| **17** | [`infra-catalogue-api`](https://github.com/DestinationHome/infra-catalogue-api) | API | `TypeScript (Hono)` | API server for Destination Home, powering the website's Object Catalogue. |
| **18** | [`website`](https://destinationhome.online/) | Website | `TypeScript (NextJS)` | Destination Home's official website. |
| **19** | `player` | CLI | `Rust` | Complete test-suite to make sure Destination Home's services are online. Checks everything, all the way from the DNS to joining the game. |
| **20** | `capone-service` | API | `ModuleJS` | API server accepting player reports ("grief reports"). |
| **21** | `infra-destinations` | API | `TypeScript (Hono)` | API server managing save data and quests progression for multiple game makers. |
