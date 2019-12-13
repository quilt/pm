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
## Outline

### Examining Ethereum
* Overview of Eth1
	* Historical context
	* Structure
	* Limitations
* Overview of scaling options
	* Supernodes
	* Sharding
	* L2

#### Sources
* [Eth1 Design Rationale](https://github.com/ethereum/wiki/wiki/Design-Rationale)

### Eth2 Overview
* Overview of Eth2
	* Historical context
	* Eth2 Protocol
		* Design rationale
		* Principles
		* How Eth2 addresses limitations of Eth1
	* Protocol explanation
		* PoS (Casper)
		* Forking & fork choice rules
		* Rewards
		* Slashing
		* Sharding
		* Crypto (BLS, randomness)
		* Proof of Custody
		* Validator lifecycle
		* Security guarantees
                * Networking
	* Current status of Eth2 R&D
* Introduction to Eth2 phases
	* Purpose of the phase system
	* General transition overview
	* Brief overview of each phase
* Introduction to Eth2 Ecosystem
	* Overview of resources
	* Overview of research process
	* Overview of projects

#### Sources
* [Serenity Design Rationale](https://notes.ethereum.org/@vbuterin/rkhCgQteN?type=view)

### Phase 0
* Beacon chain
	* Purpose & reasoning
	* Alternatives
* Fork choice rules
* Assumptions (Honest Validator)
* Deposit contract
	* ETH2 tokens
	* Purpose & reasoning
	* Impact on ETH1 tokens
* Sharding introduction

#### Sources
* [Eth2 Specs](https://github.com/ethereum/eth2.0-specs)
* [Eth2 Shard Simplification Proposal](https://notes.ethereum.org/@vbuterin/HkiULaluS)

### Phase 1
* Custody game
	* Purpose & reasoning
	* Technical explanation
* Shard data chains
	* Overview
		* Shards as containers for blobs of data
	* Protocol overview
		* Shard format & purpose
		* Crosslinks
		* Fork choice rules
		* Validator shuffling
		* Fraud proofs
	* Data availability use-cases
		* L2
			* Plasma
			* Optimistic rollups
			* ZK rollups
* Beacon chain updates

#### Sources
* [Eth2 Specs](https://github.com/ethereum/eth2.0-specs)
* [NEAR Whiteboard Series: Justin Drake](https://www.youtube.com/watch?v=S262StTwkmo)
* [Formalizing and Improving Eth2's Approach Toward Finalization of Invalid Shard Blocks](https://ethresear.ch/t/formalizing-and-improving-eth2s-approach-toward-finalization-of-invalid-shard-blocks/6263)

### Phase 2
* EEs
	* Eth1 EEs
		* Purpose & reasoning
		* Challenges
			* Stateless model conversion
			* Account model
		* Status
			* SMPT
			* Turbo Token
			* EVM interpreter
	* Novel EEs
		* C Merkle Token
		* ZK rollup EE
		* Shard Ether
		* SimpleUmbrella
* eWASM
	* Interpreters vs Compilers
	* Metering
		* Purpose
		* Challenges
* Economics
	* Relayers
	* State providers
	* Fee markets
* Cross shard transactions
	* Purpose & reasoning
	* Proposals & models
		* Simple async
		* Actor model
		* 2-phase commit
		* Locking R/W
* Toolchain
	* Simulation
	* Developer tools (Truffle-like)
	* Proof generation tools
	* eWASM-centric contract languages
	* Relayer & state provider tooling

#### Sources
* [Roadmap for an Eth1.x Execution Environment](https://notes.ethereum.org/cISMnGRMR6-EWka8QLLlYw)
* [Stateless MPT Token](https://github.com/poemm/stateless_merkle_token)
* [Turbo Token](https://github.com/ewasm/biturbo)
* [Shard Ether](https://github.com/quilt/sheth)
* [Kernel](https://github.com/quilt/kernel)
* [State Execution in Eth2.0](https://www.youtube.com/watch?v=8H1TCbW0LJQ&t=1h34m41s)
* [eWASM: Past, Present, Future](https://www.youtube.com/watch?v=aoaJIaq_fF8)
* [Relay Networks and Fee Markets in Eth2.0](https://medium.com/@adlerjohn/relay-networks-and-fee-markets-in-eth-2-0-878e576f980b)
* [Eth2.0 Shard Chain Simplification Proposal](https://notes.ethereum.org/@vbuterin/HkiULaluS)
* [Layer 2 State Schemes](https://ethresear.ch/t/layer-2-state-schemes/5691)

### Eth2 Ecosystem
* Resources
	* Where to find more information about Eth2.0
* Research process
	* Where research happens
	* How to participate in research
	* Who's working on research
* Projects
	* Easing into Eth2 projects
	* Types of available projects
	* Connections to specific projects
	* Guides to getting involved

#### Sources
* [ethresear.ch](https://ethresear.ch)
