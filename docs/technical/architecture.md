# Technical Architecture

## Overview

d.conomy is a **set of loosely coupled services** that integrate with CivicNotes and the Φ‑Grid. It can be implemented on traditional web infrastructure or on a blockchain, depending on community preference.

## Core Services

- **LoT Service** – Inventory management, reservations, usage tracking.
- **Mutual Credit Ledger** – Account balances, transaction history.
- **CLT Service** – Lease management, bond issuance.
- **Φ‑Currency Ledger** – Balances, transfers, demurrage deductions.
- **PoR Oracle** – Detects events, triggers minting.

## Integration with CivicNotes

- **Authentication** – Uses same user accounts (OAuth).
- **Data Models** – Extends CivicNotes database with d.conomy tables.
- **API** – Exposes endpoints for CivicNotes frontend to display balances, usage stats, etc.

## Example Data Flow

1. A user borrows a tool from the LoT.
2. LoT service logs the transaction and updates usage count.
3. Usage count reaches a PoR threshold → PoR oracle triggers.
4. PoR oracle calls Φ‑currency ledger to mint new Φ to the LoT Guild.
5. Φ‑currency ledger updates balances.
6. CivicNotes frontend displays the new balance on the Guild’s dashboard.
