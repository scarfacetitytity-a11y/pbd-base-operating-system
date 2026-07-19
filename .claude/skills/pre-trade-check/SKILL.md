---
name: pre-trade-check
description: Run Jay's pre-entry checklist before taking a trade on XAUUSD, US30, US100, GBPUSD or other forex/indices. Use when the user is about to enter a trade, wants a setup checked, asks "should I take this trade", or mentions an active or planned entry. Walks through higher-timeframe bias, premium/discount, liquidity sweep, M5/M1 confirmation, risk-to-reward, and emotional state, then gives a clear go/no-go call.
---

# Pre-Trade Check

Reference: `trading/trading_framework.md` (Sniper v1.0 model).

Walk through this checklist with the user, one question at a time or as a batch if they've already given detail. Do not let vague answers pass.

1. What is the higher timeframe (M30/M15) bias?
2. Are we in premium or discount, or stuck in the middle of the range? (Middle of range = no trade.)
3. Has liquidity been swept?
4. Is there M5 structure confirmation (break of structure / market shift)?
5. Is there M1 entry confirmation (rejection candle, liquidity grab)? Never enter on a guess before this.
6. Where is invalidation (stop)?
7. Where is the target? Is risk-to-reward at least 1:2 (A-star setup)?
8. Is the trade actually worth the risk?
9. Is the trader calm, or emotional/forcing it?

## Verdict

After going through the checklist, give a direct **GO** or **NO-GO** call — no hedging.

- If any answer is unclear or "kind of" → **NO-GO**. No-trade is a valid, winning outcome.
- If the trader admits emotion, boredom entry, or outside influence → **NO-GO**, and point them to the `emergency-reset` skill if they sound tilted.
- Only call **GO** if every item is clean and it's a genuine A-star setup.

Keep the tone direct and calm, like a disciplined big brother — not robotic, no waffle. Don't soften a NO-GO to spare feelings; protecting capital comes first.
