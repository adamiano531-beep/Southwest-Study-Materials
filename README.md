# Southwest Study Board

A single-page study app for Southwest Airlines Flight Attendant training — built to help
memorize airport codes, company terminology, and scripted PA announcements before/during
initial training.

**Live demo (after enabling GitHub Pages — see below):**
`https://<your-username>.github.io/<repo-name>/`

## What's inside

One topic selector, three study areas:

- **Airport Codes** — all 120 Southwest destinations, as flashcards + multiple-choice quiz
- **Company Terms** — 111 abbreviations from the Company Terms and Abbreviations packet,
  as flashcards + multiple-choice quiz
- **PA Announcements** — all 35 scripted PAs, including the conditional boxed inserts
  (Flight Attendant Candidate Introduction, Aircraft with Recaro Seating, Raft-Equipped
  Aircraft) embedded at their exact position in the Opening and Emergency Briefing scripts.
  Three ways to drill:
  - **Build in Order** — step through each PA paragraph by paragraph, self-graded
  - **Order Shuffle** — paragraphs are scrambled; put them back in the correct order
  - **Cold Recall** — recall the whole script from just the title, then check yourself

Opening and Emergency Briefing (the two longest, highest-stakes scripts) are pinned at the
top of every PA list under a "⭐ Key PAs" heading.

## Source material

Content is transcribed from two internal training documents:
- `Company Terms and Abbreviations` (09/15/2025)
- `PA Packet` (05/01/2026)

This is a personal study aid, not an official Southwest Airlines product.

## Tech

Plain HTML, CSS, and JavaScript — no build step, no dependencies, no backend. All app data
is embedded directly in `index.html`. The only external resource is a Google Fonts
stylesheet loaded over CDN; the app still functions offline without it (fonts just fall
back to system defaults).

**Note:** there's no persistence layer — quiz scores and progress reset on page refresh.
Everything lives in browser memory for the current session only.

## Running it

**Locally:** just open `index.html` in any browser. No server required.

**Hosted (GitHub Pages):**
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Under "Source," select your main branch and `/ (root)`, then save
4. GitHub will publish it at `https://<your-username>.github.io/<repo-name>/`

**On iPhone:** open the hosted link in Safari, tap the Share icon, then
**Add to Home Screen** for an app-like icon and full-screen experience.
