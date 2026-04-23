---
name: Pale Horse Driver App PWA
description: PWA for CDL driver employment applications — Isabel (HR) sends link, applicant fills out and submits, Vercel function generates merged PDF and emails HR
type: project
originSessionId: ac615905-3e82-4b56-86c5-f9dafdf5d572
---
Live URL: https://pale-horse-driver-app.vercel.app/
Repo: https://github.com/Jatt5abi/pale-horse-driver-app
Vercel project: pale-horse-driver-app (foodandbooze-2074s-projects)
HR email: isabel@palehorseae.com (hardcoded in api/submit.js line 4)
Stack: Vercel serverless (ESM), pdf-lib, Resend, vanilla JS PWA

**Why:** Isabel (HR) sends link to driver applicants. They fill all tabs, hit Submit → merged PDF emailed to Isabel. DOT-compliant driver file.

**How to apply:** Read /tmp/pale-horse-driver-app/public/index.html and api/submit.js — source of truth.

## Current state (2026-04-23) — v15

9 tabs: Personal(0) → License(1) → Employment(2) → Experience(3) → Emergency(4) → Tax(5) → Docs & Sig(6) → Submit(7)

Service worker: v15 (public/sw.js)
Company address: 19256 California Hwy 99, Acampo CA 95220
Logo: public/logo.png

## PDF pages generated (in order)
1. Application (multi-page)
2. W-4
3. DE-4
4. I-9
5. Direct Deposit
6. ID Photos (DL front/back + second ID)
7. Medical card — own page(s), raw PDF merge if PDF uploaded
8. Clearinghouse consent (Class A/B only, if consented)

## Key features
- Upload: Camera OR File buttons per field (no capture=environment lock)
- PDF uploads supported for medCard and id2 — stored with isPdf flag
- Signature pad: strokes persist on finger lift, only Clear button wipes it
- Phone numbers formatted 916-479-5590 everywhere via fmtPhone()

## Class A/B conditional fields
- Clearinghouse consent: shown on Experience tab (A or B) — MANDATORY, must say yes
- HOS 7-day cert: shown on Docs & Sig tab (A only) — grid auto-built from dateAvail, one row/day, Off Duty checkbox or hours 0-24
- DOT medical card upload: shown on Docs & Sig tab (A only)

## I-9 section (Docs & Sig tab)
- Citizenship status radio: citizen / national / lpr / alien
- Alien Reg # field: shown for lpr or alien
- Work auth expiry: shown for alien only
- Document type: US Passport, Green Card, SS Card+ID, Birth Cert+ID, Citizenship Cert+ID
- PDF marks correct [X] checkbox and fills Section 2 doc info

## Signature blocks (all forms)
- Date shown at top of sig block (filled in)
- 54pt space reserved above sign line for sig image
- Image bottom touches sign line, extends upward
- Single sign line full width — no floating second date line

## Key implementation notes
- "type": "module" in package.json (ESM)
- Body size limit: 12mb
- Client-side image compression: max 900px, 78% JPEG
- Canvas sig pad: init() only on setup, not on each stroke start
- SSN formatter strips non-digits first
- Employment history must cover 3 years
- Per-tab validation blocks navigation
- Vehicles rendered full-width (not in twoCol — too long)
- HOS log: one line per day in PDF
- DE-4 allowances: fixed x=520 for all values
- Med card PDF: copied directly into merge (full size, all pages)
