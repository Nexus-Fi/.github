## NexusFi
<img width="1680" alt="Screenshot 2024-06-14 at 17 01 50" src="https://github.com/Nexus-Fi/.github/assets/165198082/2d2a76c2-0f1f-4116-9d6d-dce6ca3d3481">
<br> <br>

Participants have the option to directly engage with the platform through a process known as native restaking. 

Unlike liquid staking, where tokens are staked through a liquid staking protocol, native restaking involves committing NIBI directly within a validator for additional commitments. This NIBI serves as a form of collateral, and if the validator deviates from its commitments, it risks losing the NIBI held within.


## Table of Contents

1. [Introduction](#introduction)
2. [Architecture](#architecture)
3. [Smart Contracts](#smart-contracts)
4. [Quick Start](#quick-start)
5. [Glossary](#glossary)

## Introduction

Nexus Finance provides a robust platform for users to maximize their staking rewards through innovative restaking strategies. By locking tokens into the Nexus Finance system, users can earn compounded interest, interact with DeFi protocols, and manage their assets seamlessly.

## Architecture

The Nexus Finance architecture is composed of several interconnected modules that handle different aspects of the restaking ecosystem. Below is the architecture diagram, followed by a brief explanation of each component.

![Architecture Diagram](./images/architecture.jpeg)

### Components

1. **Staking Module**: 
   - Handles the staking and unstaking of tokens.
   - Users can lock their tokens to earn rewards over time.
   - Integrates with the staking issuance module for minting and burning operations.

2. **Staking Issuance Module**:
   - Manages the issuance of pegged tokens when users stake their assets.
   - Handles the burning of pegged tokens during the unstaking process.

3. **Mint**:
   - Mints new pegged tokens corresponding to the staked amount.

4. **Burn**:
   - Burns pegged tokens during the unstaking process to release the original tokens.

5. **Rewards and Yields**:
   - Calculates and distributes rewards to users based on their staked amount and the duration of staking.

6. **Restake Module**:
   - Allows users to restake their rewards to earn compound interest.
   - Integrates with strategy managers and validators for optimized staking strategies.

7. **Strategy Manager**:
   - Manages various staking strategies to maximize yields.
   - Works with DeFi protocols and validators to ensure optimal returns.

8. **Validators**:
   - Validates transactions and ensures the security of the staking process.
   - Works in conjunction with the delegation module to manage user stakes.

9. **Delegation Module**:
   - Allows users to delegate their stakes to preferred validators.
   - Manages the delegation and redelegation process.

10. **Nexus Pod**:
    - Central hub for managing all staking and yield farming activities.
    - Coordinates with the rest of the modules to ensure seamless operations.

## Smart Contracts

Nexus Finance is powered by a suite of smart contracts, each responsible for a specific functionality within the ecosystem. The following are the key smart contracts:

1. **Staking Contract**: Manages the staking and unstaking of tokens.
2. **Pegged Token Contract**: Handles the minting and burning of pegged tokens.
3. **Reward Distribution Contract**: Manages the calculation and distribution of staking rewards.
4. **Restake Contract**: Facilitates the restaking of earned rewards.
5. **Strategy Manager Contract**: Implements various yield optimization strategies.
6. **Delegation Contract**: Manages the delegation of stakes to validators.
