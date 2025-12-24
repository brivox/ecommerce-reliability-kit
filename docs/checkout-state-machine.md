# Checkout State Machine (Baseline)

## States
- cart_created
- checkout_started
- payment_pending
- payment_confirmed
- order_finalized
- failed
- canceled

## Rules
- Only server transitions state.
- Webhook confirmation finalizes payment state.
- Client retries must be idempotent.
