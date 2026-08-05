# Dispatch Board: Forum Channel Rules

## What Route Running Is

The company's core income stream. A runner buys an item in one city, transports it across the map (often through dangerous zones), and sells it for profit in another city or through the Caerleon Black Market. It takes market knowledge, planning, and a willingness to risk the goods in transit.

## Splits

The split isn't just about who owns the capital, it's about what the guild is actually providing on that specific run.

| Arrangement | Runner Gets | Guild Gets |
|---|---|---|
| **Guild-Funded** (guild supplies the mount for the run) | 25% | 75% |
| **Self-Funded with Escort** (runner brings their own goods, guild provides protection/escort during the run) | 50% | 50% |

If a runner wants to go fully solo with their own goods and no guild escort, there's no guild cut to negotiate since the guild isn't providing anything on that run, they're just running on their own. The 50/50 tier prices in the value of the guild's protection, the 75/25 tier prices in the value of the guild's mount.

## Sales Outlet

**Caerleon Black Market:** the primary channel for crafted gear and gank loot moved through route running.

## Required Posting Template

```
ITEM:
BUY LOCATION:
SELL/DESTINATION LOCATION:
FUNDING TYPE: Self-Funded or Guild-Funded
ESTIMATED PROFIT:
NOTES:
```

## Tags

Three tags, in order:

1. **Open:** a new job has been posted, unclaimed.
2. **Delivered:** the runner delivered the goods and the payout is confirmed. The thread closes and gets removed once tagged.
3. **Lost Goods:** the run failed, the order and its goods are gone.

## Rules

1. One job per thread.
2. Every post must use the full template. No incomplete threads.
3. Funding type sets the split and is locked in at posting (see Splits above). Guild-Funded jobs need Route Master confirmation of capital before the thread is tagged Open.
4. Only the Route Master assigns tags. Runners don't self-tag.
5. First reply of "claiming" locks the job. No double-claiming, no reserving jobs you're not ready to run.
6. Runner and Route Master both confirm the payout amount before a thread is tagged Delivered. The thread itself, plus the ledger entry, is the record, this is the primary tracking mechanism until a bot exists to automate it (see `operations/ledger-log.md`).
7. If a run goes bad, tag it Lost Goods immediately, don't leave it hanging as Open. Self-Funded losses are the runner's own risk. Guild-Funded losses come out of company capital and get logged as a loss.
8. Stale claims (48 hours, no update) get released by the Route Master.
9. No side deals outside the board. Everything gets logged.
