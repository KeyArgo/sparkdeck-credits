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

   | merged PR size                         | credits |
   |----------------------------------------|--------:|
   | 20 lines or fewer                      |      25 |
   | 200 lines or fewer                     |     100 |
   | 1000 lines or fewer                    |     250 |
   | more than 1000 lines                   |     400 |
   | includes tests                         |     +50 |
   | your first merged PR in that repo      |    +100 |

   Caps: 500 credits per PR (before the first-PR bonus) and 750 per person
   per week; a PR over the weekly cap is paid the following week. Line count
   is only a rough size: exceptional work gets a manual top-up (`grant`).

   Credits expire 6 months after you earn them (oldest first), and a balance
   tops out at 3,000; see `TERMS.md` §6.

   These rewards apply to PRs merged from 2026-11-03. Earlier merges were
   paid on the previous table (50 / 250 / 500 / 1000, +250 for tests, cap
   1250), and that pay stands.

5. **Burn** — usage costs credits per token, with separate input and
   output rates per model. Current rates are shown on your account page and
   may change during the alpha. Credits are points, not money.
   Empty balance = key pauses (HTTP 402) until your next grant.
6. **Check** — sign in at the account page with your key to see your
   balance, usage and history; the ledger is the record of truth.

Credits are a barter for contributions, not payment — see `TERMS.md` §6.

## Endpoint

    base URL + personal key + model list: posted on your signature PR, after it merges.
