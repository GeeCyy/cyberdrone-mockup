# Cyberdrone35 + Cyberlux Watch Lab — Project Blueprint

> Living document. Status: **Phase 1 — static UI mockup** (`design/index.html`). Last updated: 2026-11-22.

## 1. Overview

| | |
|---|---|
| **Client** | Friend's two businesses, shown as one site |
| **Business 1** | **Cyberdrone35** — "Shoes and Lux Items". We BUY · SELL · TRADE · RESTORE sneakers, cars and luxury items. "100% Legit", "Affordable Price". IG: [@cyberdrone35](https://www.instagram.com/cyberdrone35) (296 followers). Deals also posted on Facebook and Carousell. |
| **Business 2** | **Cyberlux Watch Lab** — Service · Buff · Repair for watches (Rolex, Omega, Tag Heuer seen in posts; "Watches SOLD" archive). IG: [@watch_repair_maintenance](https://www.instagram.com/watch_repair_maintenance) (30 followers). Facebook: https://www.facebook.com/share/19mhU6JAJJ/ |
| **Audience** | Local buyers/sellers arriving from Instagram, Facebook or Carousell on **mobile**; they need trust fast. |
| **Mode** | Persuade (visitor decides to message). |

**Goal:** one branded home that proves legitimacy, shows what's available and what can be fixed, and funnels people to a DM.

## 2. Design direction

- **Concept:** every item leaves with a *service tag* — the appraisal ticket is the page's signature object (hero tag, deal tickets, "sold" tags).
- **Scene:** someone on their phone at night, deciding whether to trust a seller with a ₱-thousands purchase. Needs proof and an obvious next step.
- **Color (palette C, "Concrete & Cherry", chosen by the user 2026-11-22):** charcoal `#1B1B1D` field · concrete `#DCD9D3` paper and tickets · cherry `#D12A25` actions and bands (`#FF625A` for red text on dark) · black `#0D0D0E` + silver `#C9CDD3` for the Watch Lab. Replaced the first cobalt/orange palette; options A (violet), B (racing green) and D (obsidian/brass) were declined.
- **Type:** Unbounded (display, wide/techy) + Hanken Grotesk (body).
- **Motion:** one authored moment — the hero tag swings in; the Watch Lab's second hand ticks. Respects `prefers-reduced-motion`.
- **Assets:** all illustration is authored SVG (sneaker, car, watch). **No real photos yet** — see content inventory.

## 3. Sitemap (single page)

1. Header (wordmark, two section links, Message CTA)
2. Hero — Buy / Sell / Trade / Restore + service-tag
3. Four verbs
4. Cyberdrone35 deals (sample tickets) + sample reviews
5. Cyberlux Watch Lab — service, buff, repair, brands, sold tags
6. Legit promise band
7. Contact + footer

## 4. Content inventory (to collect from client)

| Item | Status |
|---|---|
| Logos (both brands) | needed — wordmarks are placeholders |
| Real deal photos, watch before/after photos | **interim:** 10 photos saved from the two Instagram feeds into `design/assets/` (640px, Nov 2026). Get originals from the owner, confirm he's happy with their use, and replace; watch photos look like dealer/stock shots, so use his own bench photos. |
| Real reviews (from the "Reviews" highlight) | needed — sample copy is flagged |
| Facebook page link for Cyberdrone35, Carousell link | needed |
| Location / meet-up policy, hours | needed — not shown |
| Services list + turnaround/pricing for watch work | needed — wording is generic, confirm |
| Currency and real prices | confirm — samples use ₱ |

## 5. Tech

Static HTML/CSS (no build step, no `package.json`), deploy-ready via `design/vercel.json`. Decide on a framework only if a CMS/ordering is requested.

## 6. Open questions
1. Keep one combined site, or add a separate page per brand later?
2. Messenger vs Instagram DM as the primary contact?
3. Does the client want live listings (CMS) or a "see Facebook/Carousell" link-out?
4. Domain and who maintains content?

## 7. Decision log
| Date | Decision |
|---|---|
| 2026-11-22 | Both businesses on one site (user decision). |
| 2026-11-22 | Static HTML mockup first; skills used: impeccable + ui-ux-pro-max. |
