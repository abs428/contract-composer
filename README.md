# contract-composer

Compose arbitrary financial contracts using Python.

This repository implements the ideas described in a research paper[^1] that defines a small set of composable primitives for building complex financial contracts. By implementing the precise language described in the paper, this project aims to make it possible to model, simulate, and reason about financial agreements in a principled way.

The long-term goal is to enable users to ask hypothetical questions about their finances (e.g., *What happens if interest rates change?, What is the future value of this agreement?*). Combining this framework with generative AI for natural-language interaction is a potential next step.

## Overview

Traditional financial products (loans, options, insurance, bonds, derivatives) can be expressed as combinations of simple contract primitives. This project provides:
- A **domain model** for financial contracts
- A **compositional framework** for building complex agreements
- Tools for **evaluation and simulation** of contract outcomes over time

Instead of hardcoding specific instruments, the system allows users to construct contracts from reusable building blocks.

## Core Ideas

The implementation follows a compositional approach where contracts are built using a small set of primitives such as:

- **Transfers** — movement of value between parties
- **Scaling** — multiplying contract value
- **Temporal constraints** — contracts that activate at specific times
- **Conditionals** — contracts dependent on external conditions
- **Composition operators** — combining multiple contracts

This allows complex financial instruments to be expressed declaratively and evaluated programmatically.

## Features

- Composable financial contract primitives
- Deterministic contract evaluation
- Time-based contract behavior
- Extensible design for custom contract types
- Foundation for financial simulation and scenario analysis

## Project Goals / Roadmap
- Complete implementation of the contract language
- Contract evaluation engine
- Market observables and external data integration
- Simulation tools
- Natural-language interface using generative AI
- Visualization and analysis tools

## Coming soon
- Installation
- Examples

## References
[^1]: Peyton Jones, E., Eber, J.-M., & Seward, J. *Composing Contracts: An Adventure in Financial Engineering*, ICFP 2000 ([link](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/07/contracts-icfp.pdf))