## NexusFi
<img src="./nexusfiGif.gif" width="100%" alt="NexusFi banner">

NexusFi is a staking and restaking infrastructure layer built on Nibiru.
We are building the primitives that make NIBI capital more useful: stake it, receive a liquid receipt, restake it across the protocol, and manage the validator and reward lifecycle through secure smart contracts.

## Why NexusFi exists

Staking alone locks capital. Restaking turns that same capital into a more productive asset.
NexusFi was created to give Nibiru users a cleaner, more composable way to participate in network security while keeping their assets liquid, trackable, and usable across the ecosystem.

The project focuses on three goals:

- make staking feel simple for end users
- make restaking operationally safe and transparent
- provide the on-chain infrastructure needed for a real liquid staking ecosystem

## What we built

NexusFi is more than a single contract. It is a coordinated protocol stack made up of staking, liquid staking, reward routing, validator management, and restaking components.

At a high level, the system enables:

- NIBI staking with a liquid receipt token
- restaking flows for better capital efficiency
- reward collection and distribution
- validator set management
- withdrawal and unbonding handling
- protocol state tracking for slashing and exchange rate updates

## The ecosystem

The NexusFi ecosystem is designed around a few connected assets and modules:

- **NIBI** — the base asset users stake into the protocol
- **stNIBI** — the liquid staking token received when NIBI is staked
- **rstNIBI** — the restaking token used for extended protocol participation
- **Reward Dispatcher** — the component that routes and distributes rewards
- **Validator Management** — the module that manages validator operations

Together, these pieces form a composable staking system that is built to support the protocol’s long-term vision: capital that keeps working while still helping secure the network.

## Testnet Contract Addresses

*These contracts are deployed on Testnet-1 of the Nibiru blockchain.*

- **Staking Contract**: `nibi1pvyd8sku8m8uafqytuefy52vkz7utj4empkycnv3chxc4npnhpns0w629r`
- **stNIBI Token Contract**: `nibi1jwc8jufz03vmtsrcwywptzksc4t9yjgnstax3r09rm9pcrl4jy9s4vpzel`
- **rstNIBI Token Contract**: `nibi17gxmfpc6l6s79dvghs5pxgruh3spxetx0td70qwq5jkd8sa5zx7sxvjwls`
- **Reward Dispatcher Contract**: `nibi12y04ajv9fmh2n64mhtrltf8yzpqkl2a4djg8du24np5xklw5kvcq6dtsmj`
- **Validator Management Contract**: `nibi1h3rnkjxargplk88nqg9y0xrwscj5phk8jkdhc7vcre72qp8gvfdsg8xa66`

## How the protocol works

1. A user deposits NIBI into NexusFi.
2. The staking contract mints stNIBI as the liquid representation of that position.
3. The protocol manages validator delegation, reward accounting, and exchange rate updates.
4. Users can restake through the protocol to increase capital efficiency.
5. When users exit, the system handles unbonding and withdrawal flows in a controlled way.

## Core protocol modules

### Staking
- Accepts NIBI deposits
- Mints stNIBI as the liquid staking receipt
- Keeps staking state aligned with protocol rules

### Unstaking
- Starts the unbonding flow for NIBI
- Tracks exchange rates and undelegation status
- Preserves user asset integrity during exit

### Withdraw Unbonded
- Releases unbonded NIBI after the waiting period
- Calculates withdrawable balances
- Completes the exit flow cleanly

### Rewards Dispatch
- Collects and distributes staking rewards
- Handles fee separation and reward allocation
- Keeps reward flows automated

### Slashing
- Records slashing-related state changes
- Updates exchange rate data when needed
- Protects protocol accounting during validator penalties

### Restake
- Accepts CW20 restake messages
- Updates bonded amounts programmatically
- Extends capital efficiency across the protocol

### Withdraw stNIBI
- Redeems stNIBI through token transfer flows
- Supports liquidity-aware withdrawals
- Keeps user exit mechanics simple

### Validator Management
- Adds and removes validators
- Helps maintain protocol governance controls
- Supports a healthy validator set

### Delegation Module
- Powers the stNIBI CW20 token
- Defines token parameters and balances
- Supports deployment and use on Nibiru

## Architecture

The architecture diagram below shows how the protocol components interact across staking, restaking, rewards, and validator operations.

![Architecture Diagram](./architecture.jpeg)

## Vision

NexusFi is being built to give Nibiru a stronger staking foundation: one where users can access liquid staking, the protocol can coordinate rewards and validator logic reliably, and capital can move through a clearer on-chain system.

In short, NexusFi aims to turn staking infrastructure into a real product layer for the ecosystem.
