<div align="center">

# Martin Tøndel

**Self-hosted software, local-first tools, and a dislike of claims you can't check.**

[![Trondheim, Norway](https://img.shields.io/badge/Trondheim-Norway-0b7285?style=flat-square)](#)
[![MTENK](https://img.shields.io/badge/company-MTENK-6d28d9?style=flat-square)](https://github.com/martintondel02)
[![TypeScript · Rust · Python](https://img.shields.io/badge/stack-TypeScript%20%C2%B7%20Rust%20%C2%B7%20Python-334155?style=flat-square)](#)

</div>

I'm a student in Trondheim, Norway (Digital Communications & Marketing at BI), and the person behind **MTENK**. I build tools you run yourself — a video editor, media, chat, mesh networking, radiation dashboards — and I try to say plainly what works, what doesn't, and what has actually been verified.

Most of my work lives in private repositories, so the public history here is a thin slice of it. Below is the slice I've been shipping in the open, most active first.

## Aava — what I'm on right now

**[Aava](https://martintondel02.github.io/aava-site/)** is my public product house: professional creative and productivity software that feels calm, coherent and local-first. Mtenk is the company, Aava is the house, and **Aava Cut** is the first product.

### [Aava Cut](https://github.com/martintondel02/aava-cut) — a local-first video editor for Linux

22 tagged releases between 7 and 12 November 2026, from the first LumaCut build to **Aava Cut 2.1.1**. It installs and cuts video on Fedora, Debian/Ubuntu and anywhere an AppImage runs — it is not a demo.

| | |
| --- | --- |
| **Edit** | Multi-track timeline (video, overlay, titles, captions, soundtrack, SFX), trim/split/ripple delete, snapping, marquee select, 12–220 px/s zoom |
| **Animate** | Keyframes 2.0 across position, scale, rotation, opacity, colour, filters, text and volume — with spring, bounce and ease easing, auto-key and colour-coded keyframe lanes |
| **Audio** | 10-band master EQ and per-track 3-band tone, 0–1000% gain with a limiter, voiceover and a spectrum visualizer — the same bus feeds monitor and export |
| **Captions** | Local whisper.cpp (large-v3-turbo on AMD Vulkan, CPU fallback) with Silero VAD and review-before-apply. Word timings, SRT import/export |
| **Delivery** | AMD Radeon VAAPI hardware encoding with automatic CPU retry, Auto/H.264/H.265/AV1, 10-bit HDR10 for MP4, 720p–4K, 24/30/60 fps |
| **Agents** | A live MCP bridge: your own agent gets a validated command surface, frames, contact sheets and proposals — bring your own agent, no account |
| **Install** | Fedora RPM, Debian/Ubuntu DEB and an AppImage. No Node.js at runtime; FFmpeg/ffprobe do the work |

Local-first by design: media, waveforms, projects and exports stay in folders on your machine, the local server binds to `127.0.0.1`, and there is no account, no upload and no telemetry. It also never pretends a software encode was hardware. Releases are gated by 37/37 Playwright tests, typecheck and a CI job that builds all three packages.

**[Download the latest release →](https://github.com/martintondel02/aava-cut/releases/latest)** · **[Website preview →](https://martintondel02.github.io/aava-site/)** <sub>(`aava.dev` is registered but still parked, so Pages is the working link for now)</sub>

## Most active in the open

| Repository | What it is | Last work | Stack |
| :--- | :--- | :--- | :--- |
| **[Aava Cut](https://github.com/martintondel02/aava-cut)** | A local-first video editor for Linux, packaged for real use | v2.1.1 · Nov 2026 | TypeScript · Electron · FFmpeg |
| **[Radiadash](https://github.com/martintondel02/radiadash)** | Native Linux dashboard and spectrometer for the RadiaCode 110: live counts, dose, spectra, isotope candidates and geotagged survey maps | v0.2.0 · Oct 2026 | Rust · Tauri |
| **[AirPlay for Linux](https://github.com/martintondel02/airplay-linux)** | Mirror a Fedora/GNOME Wayland desktop to an Apple TV — top-bar indicator, GTK4 app, and an installer that builds doubletake; verified on a real Apple TV 4K | Oct 2026 | GNOME Shell · Python · GStreamer |
| **[Fluxbot](https://github.com/martintondel02/fluxbot)** | Self-hostable, all-in-one Fluxer bot with a real web dashboard — levels, roles and community modules. Works with any instance | v0.1 · Oct 2026 | TypeScript |
| **[MeshDeck](https://github.com/martintondel02/meshdeck)** | All-in-one Reticulum app: encrypted LXMF chat, file sharing and NomadNet-compatible page hosting over mesh networks; interop tested against NomadNet and the official lxmf | v0.2.0 · Oct 2026 | Python |
| **[mcgen](https://github.com/martintondel02/mcgen)** | A bit-exact Rust reimplementation of Minecraft's world-generation density layer, running inside a real NeoForge 1.21.1 server — correct, verifiable, and honestly slower than vanilla | v0.2.0 · Oct 2026 | Rust · Java |

## Also public

- **[Cove](https://github.com/martintondel02/cove)** — a personal, self-hostable home for video, livestreams and photos; one owner, anyone with the link can watch. Phase 1 of 7 is done — resumable upload, remux-or-transcode and HLS playback, verified end to end — and it is not ready to hand to someone else to self-host yet.
- **[Hammerhead](https://github.com/martintondel02/hammerhead)** — a thin desktop shell for Sharkord on Fedora/Linux; it always runs the web client your server ships, so there is no client/server version skew.
- **[Sharkcord Client](https://github.com/martintondel02/sharkcordclient)** — an unofficial native client for Sharkord: Rust core + egui UI, for Android, Linux and Windows.
- **[SENTINEL](https://github.com/martintondel02/sentinel)** — real-time global military awareness dashboard.
- **[GoonEconomy](https://github.com/martintondel02/gooneconomy)** — simulated institutional-grade trading terminal with a 100 ms market engine.
- **[OpenFront Evolved](https://github.com/martintondel02/openfront-evolved)** — OpenFront.io fork adding land resources (oil/ore extractors) and airstrikes.
- **[agent-seo](https://github.com/martintondel02/agent-seo)** — agent-first SEO toolkit: playbook, skills, audit CLI and templates.
- **[martintondel-no](https://github.com/martintondel02/martintondel-no)** — portfolio site built as a small, app-driven "OS".
- **[Umbrel app store](https://github.com/martintondel02/mtenk-community-appstore)** — my personal community app store for self-hosted apps.

## In the background

**[Studiehacks](https://studiehacks.no)** — a free, all-in-one study suite for BI students: notes, timetable, tasks, courses, study groups and an AI assistant in one place, in Norwegian. It's the project most people I know actually use daily. Like most of my Mtenk work, its repository is private; the site is not.

I also keep forks of things I actually run: **[Sharkord](https://github.com/martintondel02/sharkord)**, **[Jellyfin](https://github.com/martintondel02/jellyfin)** and **[Bitwarden clients](https://github.com/martintondel02/clients)**. The one fork with my own edits is **[dsh-claude-style-en](https://github.com/martintondel02/dsh-claude-style-en)**, an English edition of Nwflower's Claude Code Desktop theme for the DeepSeek Harness web GUI.

## Elsewhere

- 🌐 [studiehacks.no](https://studiehacks.no)
- 🎬 [Aava Cut releases](https://github.com/martintondel02/aava-cut/releases)
- 🏢 MTENK — [@martintondel02](https://github.com/martintondel02)

<sub>Licenses are per repository: MIT on most, AGPL-3.0 on Cove and OpenFront Evolved, GPL-3.0 on mcgen, MIT + LGPL-3.0 on AirPlay for Linux through doubletake. A few old experiments still have no license file — treat those as all rights reserved. Nothing I build phones home: no analytics, no accounts you don't own, no telemetry.</sub>
