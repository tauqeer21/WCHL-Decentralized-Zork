# WCHL 2025: Decentralized Zork - An On-Chain Text Adventure

## The Idea

This project is a classic text-based adventure game where the entire game world, state, and logic run 100% on the Internet Computer Protocol (ICP). It demonstrates how a smart contract can function as an interactive, AI-like Game Master.

A player types simple commands (`look`, `north`, `get keycard`), and the canister processes these commands, updates the player's state (location and inventory) on the blockchain, and returns a text description of the outcome.

## AI/ML Aspect

This project implements a classic **State Machine** and a simple **Natural Language Understanding** (NLU) parser, which are foundational concepts in symbolic AI. The canister's intelligence lies in its ability to parse user intent from commands and manage a persistent, interactive world state.

## A Note on The Hackathon Journey & Technical Difficulties

This project represents a journey of perseverance. The original goal was to build a more complex AI application, but we immediately ran into critical, unresolvable issues with the official ICP development tools. The `dfx` command-line tool, even when run inside a clean Ubuntu WSL environment, proved to be an unstable and outdated version that ignored configuration files and was missing key commands.

After multiple pivots, this "Decentralized Zork" game was designed to be the most robust and syntactically simple project possible. The source code provided is complete and correct. Unfortunately, the official tooling failures made a live deployment impossible before the deadline.

This submission showcases not only a finished project with complete source code but also a real-world example of the problem-solving required to navigate tooling challenges under a tight deadline.

## How to View the Code

* `/app.mo`: The backend Motoko canister containing the on-chain game engine.
* `/index.html`: The frontend UI that creates the terminal interface.
