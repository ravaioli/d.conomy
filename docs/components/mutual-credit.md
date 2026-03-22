# Mutual Credit Circles

## Description

A **closed‑loop credit system** where members extend credit to one another without interest. Transactions are recorded as credits/debits within the circle, enabling debt‑free exchange.

## Governance

- Circles are typically Guild‑based or neighborhood‑based.
- Rules (e.g., maximum debit limits, membership requirements) are set via CivicNotes proposals.
- A circle may have a “clearing house” that reconciles accounts periodically.

## Economic Integration

- Surplus credits can be transferred to other circles via bioregional clearing houses, creating a mesh of mutual credit.
- Active circles increase the “Relational Density” sub‑metric of the Φ‑Score.

## Example User Flow

1. A Guild creates a mutual credit circle for its members.
2. Members list services (e.g., carpentry, gardening) and set prices in circle credits.
3. Alice does carpentry for Bob; Bob’s debit increases, Alice’s credit increases.
4. Bob later does gardening for Carol; his debit decreases, Carol’s credit increases.
5. The circle’s ledger remains balanced without interest.

## Technical Implementation

- **Ledger database** tracking credits/debits per member.
- **API** for transactions and balance checks.
- **Integration** with CivicNotes to display circle activity in Guild dashboards.
