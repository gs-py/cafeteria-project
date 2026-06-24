# CampusCafé — Cashless Cafeteria & Lunch Management

Interactive, high-fidelity prototype for a school cafeteria platform. Single self-contained HTML file — no build, no install, no internet required (one optional web font). Open it and demo.

```
open campuscafe-demo.html      # macOS
# or just double-click the file
```

## What it demonstrates

Three connected personas in one app, sharing **one live state store** — an action in one instantly reflects in the others.

| Persona | Highlights |
|---|---|
| **Admin Dashboard** (web) | KPI cards, weekly sales chart (hand-drawn SVG), category donut, grade-wise student table, add-balance flow, menu management (stock/availability toggles), reports + export, notification log |
| **Cafeteria POS** | Category tabs, tap-to-add menu grid, scan student by QR/ID, live wallet card with allergy flag, cart, balance check → **confirm or decline** with receipt |
| **Parent Mobile App** | Phone mockup: wallet + recharge (UPI/card/netbanking), transaction history, real-time push notifications, two-way cafeteria messaging, multi-child switch |

## The "wow" moment (use this in the demo)

1. Open **Cafeteria POS** → scan `STU-01` (Aarav) → add items → **Confirm & charge**.
2. Switch to the **Parent App** (top bar) → the purchase, new balance, and a **push notification** are already there.
3. Drain a wallet below ₹100 → next order is **declined** and an auto **low-balance alert** fires.

Everything maps to the requirement flowchart: login → role → add balance → POS billing → check balance → deduct/decline → SMS/push → parent.

## Notes

- All data is mock and in-memory. **Reset data** (top bar) restores defaults.
- Currency ₹ (INR). Payments, exports, and SMS are simulated.
- Built as a vanilla HTML/CSS/JS prototype — design system via CSS variables, no framework.
