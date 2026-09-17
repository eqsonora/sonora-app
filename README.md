<div align="center">

<img src="assets/icona-512.png" width="96" alt="Sonora">

# Sonora

**A system equalizer for macOS. Ten bands, real effects, real spaces, one
menu-bar app.**

[Website](https://eqsonora.com) · [Download](https://eqsonora.com/download) · [Features](https://eqsonora.com/features) · [Pricing](https://eqsonora.com/pricing)

</div>

---

## What it is

Sonora sits in the macOS menu bar and shapes the audio of the whole system,
not one app at a time. Drag the curve, hear it change while the music keeps
playing.

This repository is **documentation only**. There is no source code here -
Sonora's engine, its site and its admin tools live in a private repository.
What you'll find on this page is an overview of what the app does, real
screenshots, and links to the actual product. If you're looking for the app
itself, go to [eqsonora.com](https://eqsonora.com).

<div align="center">
<img src="assets/app-eq-2200.webp" width="800" alt="Sonora - equalizer page">
</div>

## Features

- **10-band equalizer** - 10 bands from 31 Hz to 16 kHz, or 15, 20, 31 and 41
  bands spread from 20 Hz to 20 kHz. Drag the curve, hear it at once, with a
  live spectrum behind it. An automatic preamp and a safety limiter keep
  distortion away.
- **Bass, on its own page** - one shelf plus four bands devoted to the low
  end: Sub, Punch, Body, Mud.
- **24 effects** - compressor, limiter, de-esser, crossfeed and mono bass for
  headphones, explained in plain words with a bar that shows how hard each
  one is working.
- **13 space scenes** - concert, stadium, club, cinema, cathedral and more,
  one click each. They never touch your curve.
- **Presets** - factory ones, full tunings for specific headphones, and your
  own. Each is remembered per audio output.
- **Room correction** - a guided measurement that tunes the curve to the
  room you're actually in.
- **An AI assistant that can only touch the sound** - a chat panel that can
  turn its own tool calls into an audible trial before anything is applied.
  It cannot touch a file, a shell, a network call or an account.
- **Two windows** - the full three-column interface, or Sonora minimal, a
  small panel under the menu-bar icon for when that's all you need.

<div align="center">
<img src="assets/app-bassi-2200.webp" width="49%" alt="Sonora - bass page">
<img src="assets/app-spaces-2200.webp" width="49%" alt="Sonora - spaces page">
</div>

## How it's built

- **The app** - native Swift and SwiftUI, macOS only, a menu-bar
  (`LSUIElement`) app with no Dock icon.
- **The site, the API, the admin panel** - TypeScript on Cloudflare Workers.
- **The AI assistant** - either a local model through Ollama, or a hosted one
  (Claude, GPT) reached through a closed list of audio-only tools, gain
  ceilings, and a hear-before-you-keep trial for every change.

That's the shape of it. Implementation details, the actual engine, the API
and the admin tooling stay in the private repository - this page is a map of
what exists, not how it's written.

## Pricing and availability

**Sonora is a free app everywhere in the world.** A paid plan exists, and it
unlocks more (all effects, more bands, room correction, volume rules and
scenes, automatic correction, the AI assistant beyond the free minutes) - but
**that plan can only be purchased from Switzerland or Liechtenstein**. Outside
those two countries, Sonora runs on the free plan, indefinitely, with no
paywall to hit.

The reason is regulatory, not a limitation of the app: selling into other
markets means tax registration and legal representation Sonora doesn't have
set up yet. The current price, in Swiss francs, is always shown on
[eqsonora.com/pricing](https://eqsonora.com/pricing) - it isn't repeated here
because it can change on the site before this page catches up.

| | Switzerland & Liechtenstein | Everywhere else |
|---|---|---|
| Free plan | ✅ | ✅ |
| Paid plan | ✅ - see [eqsonora.com/pricing](https://eqsonora.com/pricing) | Not sold. The app stays free. |

## Get the app

macOS only, for now. Get it from
**[eqsonora.com/download](https://eqsonora.com/download)**.

<div align="center">
<img src="assets/app-preset-2200.webp" width="49%" alt="Sonora - presets page">
<img src="assets/app-cuffie-2200.webp" width="49%" alt="Sonora - headphones page">
</div>

## Questions, feedback, feature requests

This repository has [Discussions](../../discussions) open for questions and
feature ideas, and [Issues](../../issues) for anything specific you'd expect
a maintainer to track. Since there's no code here to send a pull request
against, the fastest way to report a bug in the app itself is still the
feedback button inside Sonora - it attaches a screenshot and reaches the team
directly.

## License

The contents of this repository (this README, its text and its images) are
© Sonora. The Sonora application, its source code and its brand are not
licensed for reuse. This repository exists to describe the product publicly,
not to distribute it.
