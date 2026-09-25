# Monolith

Monolith is a Solana orderbook built for efficient trading across multiple market types. One interface brings together order placement, cancellation, repricing, execution and settlement.

### Built for active liquidity

Market makers can refresh hundreds of quotes in one transaction. Flip orders automatically place the opposite leg after a full fill, without a separate maker transaction. Shared settlement within a market lets trading proceeds fund subsequent actions.

For takers, efficient matching leaves more compute available for routing and transaction composition. Minimum-output checks, fill limits and self-trade controls provide execution safeguards. Lower quote-maintenance costs can help makers offer tighter spreads.

### Technical capabilities

- Capacity for **551,882 orders in one market**.
- Measured standalone batches of **2,790 placements**, **385 cancellations** or **374 reprices** in a v0 transaction
- Selected batch averages of **458 CU per placement** and **698 CU per reprice**.
- GTC limit, post-only, immediate-or-cancel, timed and repeating flip orders.
- Atomic composition of deposits, cancellations, repricing, placements and settlement.

### One interface, multiple markets

**Phase 1:** Spot markets for compatible tokenized assets.

**Phase 2:** Release options and binary prediction-market functionality, scheduled to be used through the same orderbook interface.
