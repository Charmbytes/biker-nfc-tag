# 🏍️ RideSafe ID — Emergency Medical Identity for Riders

**When a rider goes down, the first 10 minutes decide everything. RideSafe ID makes sure first responders know who they're helping — instantly.**

🔗 **Live demo:** https://charmbytes.github.io/biker-nfc-tag/

---

## The Problem

Road accidents are a leading cause of death for two-wheeler riders, and in the critical minutes after a crash, bystanders and paramedics usually know **nothing** about the victim:

- No name, no blood group, no allergy information
- No way to reach family — phones are locked or damaged
- Medical history (diabetes, epilepsy, heart conditions) stays invisible exactly when it matters most

Wrong or delayed treatment in this window costs lives.

## The Solution

RideSafe ID turns a helmet or bike into a **scannable medical identity**.

1. A rider fills a one-time form: name, age, blood group, allergies, medical history, surgeries, and an emergency contact.
2. The app instantly generates a **unique link and QR code** for that record.
3. The QR is printed as a sticker or written to an **NFC tag** on the helmet.
4. Anyone at an accident scene taps or scans it — the rider's medical ID card opens in any browser, with a **one-tap CALL button** to reach family immediately.

No app download. No login. No internet dependency on our side. It works on every smartphone made in the last decade.

## Why This Approach Wins

- **Zero friction for responders** — scan → see → call. Three seconds.
- **Self-contained records** — each ID lives in its own link, so there's no server to go down at the worst possible moment.
- **Privacy by design** — riders choose exactly what to share; nothing is collected beyond what they type.
- **Near-zero infrastructure cost** — the current architecture runs on static hosting, so unit economics stay lean while we scale.

## Product Status

✅ Working prototype — live and testable today at the demo link above
✅ Record creation, unique links, QR generation, tap-to-call — all functional
✅ Mobile-first UI designed around real emergency use

## Roadmap

| Phase | Milestone |
|-------|-----------|
| Now | Web prototype with QR + NFC-ready links |
| Next | Editable records with permanent IDs, multilingual support, printed sticker + NFC tag kits |
| Then | Partnerships with helmet brands, riding clubs, and insurers; fleet/delivery-rider dashboards |
| Vision | The default safety layer shipped with every helmet sold |

## Business Model (Proposed)

- **B2C:** one-time NFC tag + sticker kits; optional premium subscription for editable/managed profiles
- **B2B:** bulk programs for delivery fleets, riding clubs, and motorcycle manufacturers
- **Insurance:** partnerships where verified safety measures earn riders premium discounts

## Tech Notes (for the curious)

- Single static page (HTML/CSS/JS), hosted free on GitHub Pages
- Records are encoded directly into each unique URL — no database required for v1
- QR codes generated client-side; call button uses the native `tel:` protocol
- Planned v2: lightweight backend (Node.js + SQLite/Postgres) for editable records with permanent short links

## Run It Yourself

```
1. Fork this repo
2. Enable GitHub Pages (Settings → Pages → main branch)
3. Open your live URL and create a record
```

---

*Built with the belief that no rider should be a stranger in an emergency.*
