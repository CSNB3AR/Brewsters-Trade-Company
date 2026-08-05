# Dispatch Board & Economy Rules

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

## The Workshop (Crafting)

The guild's crafting engine. The guild supplies materials, a crafter supplies the skill/spec to make the item, and profit splits on sale.

**Split:**
- Guild supplies materials, crafter supplies skill/spec to craft the item, profit is split 50/50 on sale.
- Buying cheap materials specifically to convert into finished goods and flip is considered the "true trade merchant" move.
- If materials are already gathered in-house, there's no cost to recoup, so the split logic changes, there's no material cost to net out first.

**Order Board Posting Template** (for `#order-board`, members requesting a crafted item):

```
ITEM NEEDED:
QUANTITY:
MATERIALS PROVIDED: Yes or No
TIER/ENCHANT:
DEADLINE:
NOTES:
```

**Workshop rules:**
1. One request per thread.
2. Crafters claim a request by replying "claiming." First claim locks it, no double-claiming.
3. If materials aren't provided by the requester, the guild-supplies-materials split applies (50/50). If the requester provides their own materials, negotiate the labor cost directly, that's outside the guild split.
4. Workshop Warden confirms material allocation before a request is tagged Open.
5. Completed orders get confirmed by both the requester and the crafter before the thread closes.

## Guild Auction House

Rare gank/PvP loot only. Never guild-bought stock. Priced below market. Runs weekly, members-only.

**Auction Night:** the live-bidding format. The leader or officers seed rare items at a cheap starting price, then run a live call-out auction in voice or text: "going once, going twice, sold." Members-first.

**Item Submission Template** (for a member putting an item up for the guild auction):

```
ITEM:
QUALITY/ENCHANT:
STARTING BID:
REASON (loot drop, contribution, etc.):
```

Submit this in advance of Auction Night so officers can queue it.

**Anti-Flip Rule:** items bought through the guild auction can't be resold for personal profit on the open market. Enforcement is two-strike: warning first, market ban second.
