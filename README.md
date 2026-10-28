# How it works

Self-hosted LLM inference, paid in contribution-credits.

1. **Find work** — bugs, features, docs, regressions in the operator's
   public repos. Quality is the only bar that matters; Claude and Codex
   pre-review, a human approves.
2. **Sign** — PR adding yourself to `CONTRIBUTORS.md` (accepts `TERMS.md`).
3. **Get a key** — after your first merged contribution, the operator
   provisions a personal API key scoped to specific models.
4. **Earn** — merged work lands credits in the ledger:

   | contribution                        | credits (typical) |
   |-------------------------------------|------------------:|
   | typo / doc fix                      |               50  |
   | confirmed bug fix (with test)       |              250  |
   | regression fix in owned area        |             1500  |
   | new feature, accepted               |             1000  |
   | security report (valid, actionable)|              500  |
   | exceptional / large                 |          negotiable|

5. **Burn** — inference costs credits per token; some models are premium
   (frontier) and burn faster. Empty balance = paused until your next grant.
6. **Check** — ask the operator for your balance anytime; the ledger is
   the record of truth.

Credits are a barter for contributions, not payment — see `TERMS.md` §6.

## Endpoint

    base URL + personal key + model list: from the operator, after signing.
