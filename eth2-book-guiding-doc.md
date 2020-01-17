# The Eth2 Book: Guiding Document

- - - -

**Note:**
This document is meant to act as the "source of truth" for The Eth2 Book (name very much subject to change!).
It attempts to solidify a vision for the project.
Hopefully this document will help avoid future confusion over project direction.

- - - -

## Project Vision
We're working to advance the development of [Eth2](https://github.com/ethereum/eth2.0-specs) by connecting **individuals** and **information**.

[Ethereum](https://ethereum.org/) presents us with new opportunities to build healthier societies.
Eth2 is crucial to the vision of Ethereum operating at global scale.
Information about Eth2, unfortunately, remains largely inaccessible.
Important discussions and publications are scattered over the internet.
Designs quickly become outdated and research indices go unmaintained.
Differences in writing style can make existing content difficult to digest.
As a result, potential Eth2 contributors are faced with significant barriers to even basic involvement.
**We see clear value in an educational resource that molds these disparate elements into a single, coherent knowledge base**.

We're also aiming to accelerate Eth2 development by **creating pathways between educational content and relevant projects**.
An educational resource should go further than information aggregation -- it should provide pipelines that help potential contributors get involved with relevant projects.
The many Eth2-related projects are, like the sources of information about Eth2, hidden in various corners of the web.
Readers will be vastly more likely to become contributors if there's an accessible bridge between knowledge and application.

## Target Audience
A well-constructed educational resource should attract, and provide opportunities for, readers from a wide range of backgrounds.
We're initially targeting the spectrum of **people with a basic knowledge of Ethereum and some interest in Eth2**.
These readers may or may not have an understanding of the technical underpinnings of Ethereum.

## Content Structure
We want to develop new ways to present content in order to accommodate the widest possible audience.
We're experimenting with a content structure that consists of a **knowledge base** and corresponding **educational experiences**. 

### Knowledge Base
The **knowledge base** component of this project is the core repository of knowledge.
It's intended to be a **searchable** database of information, much like a wiki.
Users should be able to use the base to find any piece of Eth2 information they might be looking for.

### Educational Experiences
Although large repositories of information are extremely useful, they tend to be inaccessible when a user doesn't already know what they're looking for.
Users shouldn't have to sift through piles of information by themselves.
For that reason, it's valuable to provide **educational experiences** that present information from the knowledge base in approachable ways.
We're still working on the exact form that these experiences will take.
However, because they rely on the knowledge base for any underlying information, these experiences can be developed once the knowledge base has been mostly completed.

## Collaboration
Much of the knowledge about Eth2 is "[tribal](https://en.wikipedia.org/wiki/Tribal_knowledge)."
It's important that members of the Eth2 R&D community be able to contribute knowledge to our project.
Contributors will be able to submit "raw" content from which an editing team will generate some final content.
We're hoping this will reduce friction across the board.

- - - -

## Design Requirements

### Website
* Should be easily discoverable online.
* Should use accessibility best-practices.
* Should be accessible on any device.
* Should take full advantage of the web platform.
* Should be designed to improve the learning experience.

### Language
* Should always strive for simplicity.
* Should avoid using confusing or overly technical terminology.
* Should avoid condescension.

### Content
* Should have different entry points for different users.
* Should be effectively linked to other content within the resource.

### Projects
* Should be fluidly integrated into the learning experience.
* Should be easily accessible.

- - - -
## The Eth2 Book: Release-0 Outline

**Note**: Headers between sections (e.g., "Introduction and Background") only intended to provide logical groups of sections, not part of final visible content structure.

### Introduction and Background
- Introduction
    - Friendly introduction
        - Onboarding and priming
        - Special note for Release-0
    - Motivation
    - Content overview
- Eth1 Overview
    - Blockchain basics
        - Signatures, key pairs
        - State, transactions, blocks
        - Merkle trees, block headers
        - Peer-to-Peer network basics (?)
    - Proof of Work
        - Consensus basics
        - Hashing, finding, publishing blocks
        - Transaction fees, block rewards ("incentives")
    - Forks
        - Fork explanation
        - Fork choice rules
        - Longest-Chain Rule
        - Inclusive protocol
    - EVM + App Basics
        - EVM core concepts
        - Smart contracts, gas metering
    - Scaling
        - Eth1 limitations
        - L1 and L2
        - L1 scaling options
- Eth2 Overview
    - Big picture
        - Lessons from Eth1
        - Design rationale
        - Eth2 structure in a nutshell
    - Proof of Stake
    - Beacon Chain
    - Shard chains
    - Ewasm + EEs
    - Rollout phases

### Proof of Stake
- Proof of Stake in Eth2
    - Core Proof of Stake concepts
        - Validators, blocks, slots
        - Epochs, EBBs (?)
    - Core operation
        - Proposers, attestation committees, voting, honest majority
        - Dynamic validator pools
    - Attack surfaces
        - Catastrophic Crashes
            - Basic problem description
        - Long Range Attacks
            - Weak subjectivity problem
            - Long Range Attack methods
                - Simple (future timestamps)
                - Stake bleeding (?)
                - Withdrawn validator bribery/hacking attacks
    - LMD GHOST
        - Intro as counter-mechanism shorter-range attacks
        - Brief GHOST background
        - LMD GHOST mechanism detail
        - Methodology for countering shorter-range attacks
        - Remaining open problem with longer-range attacks
    - Casper FFG
        - Reiteration of longer-range attacks
        - Finality basics, intro as counter-mechanism to longer-range attacks
        - Definitions
            - Deposits
            - Checkpoints
            - Votes
            - Supermajority links, justified checkpoints
            - Finalized checkpoints
        - Commandments
        - Guarantees
            - Proofs for each

### Beacon Chain
- Core Beacon Chain Components
    - BLS signatures
        - Explanation of ECDSA limitations
        - Aggregation & verification fundamentals
    - RANDAO + Swap-or-Not
        - Randomness
        - RANDAO details
            - Basic concepts & purpose
            - Mixing functions
            - Known-value attacks
            - Commit-reveal RANDAO
                - Hash commitments, signature commitments
        - Swap-or-Not
            - Basic concepts & purpose
            - Basic functionality
    - SSZ (?)
- Beacon Chain
    - Validator life-cycle
        - Deposited, active, exited, withdrawn
    - Structure (in detail)
        - State
        - Blocks

### Potential Additions
- Networking?
- Ecosystem?
    - Links to relevant Phase 0 projects
    - Contributor guides
- Meta?
    - Credits, full bibliography, etc
