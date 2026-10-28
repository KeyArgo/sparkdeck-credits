# sparkdeck-credits

Self-hosted LLM inference, paid in contribution-credits.

1. **Find work** — bugs, features, docs, regressions in the operator's
   public repos. Quality is the only bar that matters; Claude and Codex
   pre-review, a human approves.
2. **Sign** — PR adding yourself to `CONTRIBUTORS.md` (accepts `TERMS.md`).
3. **Get a key** — automatic: once your signature PR merges, your personal
   API key is posted as a comment on that PR. No manual step, no waiting.
4. **Earn** — merged work lands credits in the ledger, automatically
   (`autogrant` runs every 5 minutes):

   | merged PR size            | credits |
   |---------------------------|--------:|
   | 20 lines or fewer         |      50 |
   | 200 lines or fewer        |     250 |
   | 1000 lines or fewer       |     500 |
   | more than 1000 lines      |    1000 |
   | includes tests            |    +250 |

   Cap: 1250 credits per PR. Exceptional work: ask the operator for a
   manual top-up (`grant`).

5. **Burn** — inference costs credits per token. Rates (credits per 1M
   tokens, input/output):

       GLM-5.3-Flash-EXL3   30 / 30
       spark-e              15 / 15

   1 credit = $0.01 of table value; cached input tokens count half.
   Empty balance = key pauses (HTTP 402) until your next grant.
6. **Check** — your live balance page (linked from your key-delivery
   comment) shows balance and the last 10 ledger events; the ledger is
   the record of truth.

Credits are a barter for contributions, not payment — see `TERMS.md` §6.

## Endpoint

    base URL + personal key + model list: posted on your signature PR, after it merges.
