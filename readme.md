# NEXUS

**N**etworked **E**mergency **E**xchange & **U**nified **S**ignaling

An interactive systems design study simulating emergency mesh network topology design and crisis response under failure cascades. Build a network topology, run a crisis simulation, analyze outcomes.

## What is NEXUS?

NEXUS explores the design constraints of decentralized communication infrastructure when centralized systems fail. You design a mesh topology under budget, then stress-test it against cascading failures, misinfo propagation, and battery depletion.

Three acts:
**Act I: Design** - Place relay hubs, nodes, shelters, and devices. Optimize for coverage and resilience within a 12-unit budget.
**Act II: Crisis** - Run a simulated emergency. Watch your topology fail under stress. Predict outcomes. Make real-time decisions.
**Act III: Analysis** - Compare designs side-by-side. Get topology-specific insights. Explore counterfactuals.

## Features

- **Guided tutorial** - 5-step onboarding explains nodes, budget, crisis mechanics.
- **Difficulty modes** - Mild / Moderate / Severe (changes failure rates, message volume, battery drain).
- **Undo system** - Ctrl+Z, 30-step stack, full design rewind.
- **Save & compare** - Run two designs through the same crisis, compare metrics side-by-side.
- **Live prediction** - Make a prediction at Hour 3 checkpoint, get verdict in analysis.
- **Impact visualization** - Coverage over time rendered as the crisis unfolds.
- **Topology-specific analysis** - Diagnosis reads your actual node placement and explains failure modes (bridge collapse, device-heavy limits, shelter anchoring, etc.)
- **Interactive counterfactuals** - "What if +1 relay?" "What if strict verification?" Estimate outcomes.
- **Decision journal** - All placement, save, and priority decisions logged with impact notes.

## Live Demo

[**Play NEXUS**](https://nexus-git-main-wsup.vercel.app/)

## How to Play

1. **Place nodes** — select node type (device, node, relay, shelter) and click the grid. Each has different cost, bandwidth, range, battery.
2. **Check coverage** — must reach 40% grid coverage to unlock crisis simulation
3. **Save Design A** — lock your topology before running the crisis
4. **Run crisis** — select difficulty, watch nodes fail, route messages, manage priorities
5. **Make prediction** — at Hour 3, guess if delivery improves, stays same, degrades, or collapses
6. **Analyze** — see topology-specific insights, decision impact, and counterfactuals
7. **Compare** — save the results as Design B, run a second topology, compare side-by-side

## Architecture

Single-file HTML/CSS/JavaScript. No dependencies, no build step.

- **Canvas rendering** — topology visualization + crisis simulation + comparison graphics.
- **A\* pathfinding** — message routing with hop limits.
- **Dynamic difficulty** — adjusts failure rates, latency, battery drain.
- **Persistent state** — undo stack, design saves, prediction tracking.

## Project Context

Goal was to build a teaching tool that makes systems design constraints visible through play. Developed iteratively: V2 (base), V3 (polish + accessibility), V4 - the current active one, (full feature set with comparison, prediction, analysis).

## Author
Built and maintained by Supreeth - V2.S4 / A project exploring design constraints of decentralized communication infrastructure when centralized systems fail.

---

**Deploy, play, share.**
