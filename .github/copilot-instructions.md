# Copilot instructions (Project-Leafstack)

## Product + audience (do not drift)

- This repo is a **mobile-first, conversion-focused** mini-site for a teaching program: **Python + Django for freshers**.
- Audience: freshers/recent grads (any branch), often anxious about placements; keep copy **beginner-friendly**, clear, slightly trendy, no corporate jargon.
- Primary CTA goal: **convert to WhatsApp/Telegram leads**.
- Teaching philosophy: confidence + shipping real projects; avoid over-engineering and advanced topics too early.

## What exists today (ground truth)

- Landing page: [index.html](../index.html) (inline CSS, WhatsApp CTA placeholders).
- Roadmap page: [roadmap.html](../roadmap.html) (linked from the landing page).
- Project brief / continuation rules live in [instructions-readme.md](../instructions-readme.md).

## Conventions to follow when editing/adding pages

- Keep pages as **plain static HTML** with **inline `<style>`** (no build tools/frameworks in repo right now).
- Use the existing look-and-feel:
  - Dark theme with CSS variables in `:root` (see [index.html](../index.html)).
  - Mobile-first container widths (~720–760px), large tappable CTAs, minimal clutter.
- CTAs:
  - Use `https://wa.me/YOUR_NUMBER_HERE?text=...` with **URL-encoded** text.
  - Keep placeholder phone handles (`YOUR_NUMBER_HERE`, `+91-XXXXXXXXXX`, `@leafstacked`) unless explicitly asked to replace.
- Copy style:
  - Short sections, simple words, outcome-oriented (“projects”, “resume”, “earn”).
  - Prefer clarity over cleverness; keep anxiety-reducing tone.

## Workflow (local preview)

- There’s no build step. Open HTML directly or serve locally.
- If you need a local server, use Python (repo has [.python-version](../.python-version) set):
  - `python -m http.server 8000` then open `http://localhost:8000/`.

## When continuing work (project-specific)

- Follow the pending tasks list in [instructions-readme.md](../instructions-readme.md) (lesson pages template, project pages, pricing/enrollment page, WhatsApp funnel copy, instructor positioning).
- Don’t rewrite the landing page or roadmap content unless the user explicitly asks.
- If you create new pages, keep naming consistent with intent (e.g., `lessons.html`, `pricing.html`, `projects/solo.html`) and link from the landing page.

## Safety + scope

- Don’t add backend/Django code here unless asked; this repo currently behaves like a static marketing site.
- Avoid adding dependencies/config that aren’t already present.
