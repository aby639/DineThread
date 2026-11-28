# NVDA observations

NVDA 2026.3.1 portable, Chrome on Windows; desktop keyboard layout. Downloaded
from NV Access, with a valid NV Access Limited Authenticode signature. Installer
SHA-256: `6f80a5b0ca720a7d0d314b5be212f37388bbe81a1107ac3298c1821a1cd3f052`.
The native keyboard and pointer checks in the recorded NVDA sessions used AI
assistance. Playwright prepared the synthetic fixtures. The speech observations
below come from NVDA’s own IO log. These sessions were technical inspections
without study participants.

Bibek Rai’s [personal keyboard check](RESULTS.md) covered the dish dialog. He
reached the dish with Tab, opened it with Enter, then pressed Escape and checked
that focus returned to the dish.

First session: `screenreader-1794595153110`. A uses build
`m83pPGcb6p2ZgPs9s0OoB`; B uses `Tr08L6Iuyz9VH_OifDqm1`.

| Journey | A observation | B observation |
|---|---|---|
| Customisation | Dialog announced without an item name; Tab initially reached the unnamed background Share button. Large was announced as a button without selected state; quantity controls were unnamed. | Dialog named Test soup; Large announced as a pressed toggle button, Bread as not pressed. Quantity names are exposed. Escape returned speech to View Test soup. |
| Validation | Submitting without a table announced the alert and instruction. | Shift+Tab reached Place Order; Enter announced the same instruction. The table choices have a named group. |
| Status | No new Preparing/Ready announcement was recorded during the observation intervals. A repeat with explicit DOM-version verification is required before treating absence as confirmed. | Preparing and Ready changes were announced by the persistent status region. |

The additional bill-request check **failed** on the first B build: the visible
confirmation was not announced. Its newly inserted live region was replaced by
an update to the existing order-status region. This requires a new build and
NVDA retest. The failure and first-run speech are retained.

Only task-related speech excerpts are included in the evidence. Unrelated
desktop speech and the complete local NVDA log are excluded from the repository.
The Windows UI Automation focus field sometimes remained on the address bar
while actual NVDA speech followed page controls; conclusions use the speech log,
native key events and the browser's rendered state, not that stale field.

## Retest

Session `screenreader-1794595717603` used B build `q6nMds_BQKnZGtsMjQFeu`.
The baseline status check was repeated with independent DOM-version checks:
versions 1 and 2 rendered after Preparing and Ready, but no corresponding live
speech followed. Both states still appeared together as static step labels.
In B, NVDA announced Preparing and Ready as each version rendered. After
Shift+Tab and Enter on Request Bill, it announced: “Order status: Ready. Bill
requested - your server is on the way.” This resolves the first-run bill defect.
The action log includes the rendered versions and actual visible status text.
Both native test sessions were closed, and the portable NVDA process was stopped.

## Speech Viewer retest on 28 November 2026

Bibek tested checkout with a Lemon Tart. At 0:20 Speech Viewer displayed the instruction to select a table. After checkout it displayed Preparing (0:50), Ready (1:01) and Served (1:08). The bill acknowledgement was visible at 1:19 and Paid at 1:35. The [Speech Viewer excerpts](retest-2026-11-28/nvda-speech.png) preserve the announced text. The installed NVDA version for this recording was not captured.
