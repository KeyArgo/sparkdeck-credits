# sparkdeck-credits

A small, private co-share of the operator's home AI hardware among friends,
family and a few invited contributors. **This is not a public or commercial
service:** nothing is sold, there's no open sign-up, and access is by personal
invitation only.

> **Alpha.** Private, invite-only test. Rewards, rates, limits and logging are
> experimental and may change at any time — see `TERMS.md`.

If you've been invited:

1. **Find work** — bugs, features, docs, regressions in the operator's
   public repos. Quality is the only bar that matters; Claude and Codex
   pre-review, a human approves.
2. **Sign** — PR adding yourself to `CONTRIBUTORS.md` (accepts `TERMS.md`).
3. **Get a key** — once your signature PR merges, the operator sends your
   personal API key to you privately. Keys are never posted publicly.
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

5. **Burn** — usage costs credits per token, with separate input and
   output rates per model. Current rates are shown on your account page and
   may change during the alpha. Credits are points, not money.
   Empty balance = key pauses (HTTP 402) until your next grant.
6. **Check** — sign in at the account page with your key to see your
   balance, usage and history; the ledger is the record of truth.

Credits are a barter for contributions, not payment — see `TERMS.md` §6.

## Endpoint

    base URL + personal key + model list: posted on your signature PR, after it merges.
