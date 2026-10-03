# StakeSensei

![StakeSensei logo](assets/logo.png)

Interactive sandbox where you run your own Solana validator and compare it to Ethereum.

## Overview

StakeSensei is a browser-based simulator built for Japanese crypto beginners and students who learn better by doing than by watching videos. It lets users spin up a simplified virtual validator, watch it get selected as leader, produce blocks via a mock Proof of History, and vote, then toggle the same scenario into Ethereum's validator/attester model for a direct, side-by-side comparison. It is designed as companion interactive content alongside short educational videos.

## Problem

Passive video explanations of validator consensus don't stick. Beginners struggle to intuitively grasp Proof of History, leader schedules, and stake-weighted voting, and Ethereum's slot/epoch/attestation system adds another layer of confusion when only explained in narration.

## Solution

StakeSensei gamifies the validator lifecycle into clickable steps: stake, delegate, get selected, produce a block, get voted on, and earn or lose rewards. A mirrored Ethereum mode maps each Solana concept to its Ethereum equivalent, turning abstract consensus mechanics into an interactive story that videos can reference and link to.

## Features (MVP)

- Mock validator setup flow: stake amount, delegate, see selection odds
- Visual leader rotation clock synced to simplified PoH ticks
- Vote/slash simulation with animated rewards and penalty scenarios
- Toggle switch "Solanaモード / イーサリアムモード" showing equivalent concepts side by side
- Shareable short clips/gifs of each simulation step for embedding in videos

## Tech Stack

- React
- Three.js or Canvas for animation
- Solana web3.js (real reference data)
- Ethereum Beacon Chain API (real reference data)
- Supabase for session state
- Framer Motion for UI transitions

## How It Works

The validator lifecycle runs entirely client-side as a simulation, while Solana web3.js and the Ethereum Beacon Chain API provide real reference data to ground the numbers and timing shown to the user.

```
[User] -> [React UI: stake/delegate] -> [Mock PoH clock] -> [Leader selected]
 -> [Block produced] -> [Simulated validators vote] -> [Rewards/Slash animation]
 |
 Solana web3.js (read-only)
 Ethereum Beacon API (read-only)
 |
 [Mode toggle: Solana <-> Ethereum]
 |
 [Supabase: session state]
```

## Roadmap

- Add multiplayer mode where users compete as validators
- Integrate real testnet validator deployment tutorial
- Localize to other languages and add quiz/certification mode

## Pitch

- [Pitch deck (PDF)](docs/pitch.pdf)
- [Pitch script](docs/pitch-script.md)

## Team

- Name / Role - placeholder
- Name / Role - placeholder
- Name / Role - placeholder

Built for the Colosseum hackathon (Solana and other chains).

---

🎬 Pitch video: [docs/pitch-video.mp4](docs/pitch-video.mp4)


## Prototype

Live prototype: https://hdeep04.github.io/stakesensei/

The source is [docs/index.html](docs/index.html) (served with GitHub Pages from the /docs folder). All data is simulated.

🎥 Demo video: [docs/demo-video.mp4](docs/demo-video.mp4)
