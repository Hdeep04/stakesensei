# StakeSensei

_Interactive sandbox where you run your own Solana validator and compare it to Ethereum_

## Summary

A browser-based simulator that lets beginners spin up a simplified virtual validator node, watch it get selected as leader, produce blocks via mock Proof of History, and vote, while a toggle switches the same scenario to Ethereum's validator/attester model for direct comparison. Designed as companion interactive content alongside short videos.

## Target users

Japanese crypto beginners and students wanting hands-on learning instead of passive video watching

## Problem

Passive video explanations of validator consensus don't stick; beginners struggle to intuitively grasp PoH, leader schedules, and stake-weighted voting versus Ethereum's slot/epoch/attestation system.

## Solution

Gamify the validator lifecycle into clickable steps (stake, get selected, produce block, get voted on, earn/lose rewards) with a mirrored Ethereum mode, turning abstract consensus into an interactive story that videos can reference.

## MVP features

- Mock validator setup flow: stake amount, delegate, see selection odds
- Visual leader rotation clock synced to simplified PoH ticks
- Vote/slash simulation with animated rewards and penalty scenarios
- Toggle switch 'Solanaモード/イーサリアムモード' showing equivalent concepts side by side
- Shareable short clips/gifs of each simulation step for embedding in videos

## Chains

Solana, Ethereum

## Tech

React, Three.js or Canvas for animation, Solana web3.js (for real reference data), Ethereum Beacon Chain API, Supabase for session state, Framer Motion

## Category

Consumer / Gaming / Education

## Why now

As Solana's validator economics evolve (Alpenglow, Firedancer), there's demand for intuitive, interactive explainer tools beyond static videos, especially for non-English speakers.

## Roadmap

- Add multiplayer mode where users compete as validators
- Integrate real testnet validator deployment tutorial
- Localize to other languages and add quiz/certification mode
