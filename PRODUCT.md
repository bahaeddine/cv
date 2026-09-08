# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Primary audience is recruiters and hiring managers evaluating Baha Eddine Boukhzar for Cloud & Platform Engineer roles. The site currently supports an active job search — it should read as a pitch, not just a passive reference page, though it also functions as the standing professional profile linked from LinkedIn/GitHub/email.

## Product Purpose

A personal single-page CV/portfolio site that presents ~8 years of cloud and platform engineering experience (Renault Group, Ingenico, Paris-Dauphine, Sofrecom) in a way that gets a hiring manager to reach out. Success is a recruiter or hiring manager coming away with a clear, credible picture of scope and impact, and using the contact section to get in touch.

## Positioning

A single continuous throughline, not three disconnected jobs: migrated 1,000+ applications to GCP/Kubernetes → built Renault's central GKE platform from the ground up → now owns the Software Factory the engineering org runs on daily. The mechanism a neighboring candidate couldn't truthfully copy is that continuity — one person who has lived the full lifecycle (migration → platform build → platform ownership) inside the same organization. This throughline is confirmed and must be preserved as the lead narrative in any future redesign.

## Operating Context

Static site hosted on GitHub Pages (gh-pages branch), served at the custom domain in `CNAME` (bahaeddine.boukhzar.com). Self-contained `index.html` (inline CSS/JS, Google Fonts + Font Awesome via CDN) — no build step, no framework, no dependencies to install. The `README.md` still describes the old Jekyll/markdown-cv template this project has since moved away from (per commit "Replace Jekyll CV site with self-contained index.html redesign") and is stale documentation, not product truth.

## Capabilities and Constraints

- Single HTML file (`index.html`), edited and deployed directly on `gh-pages` — no CI/build pipeline.
- Assets live under `media/images/`.
- Sections: Hero, About, Experience (expandable per-company rows), Skills, Certifications, Contact.
- No CMS, no analytics mentioned, no contact form — contact is direct mailto/tel links plus social links (GitHub, Twitter, LinkedIn).

## Brand Commitments

- Name: Baha Eddine Boukhzar.
- Title: Cloud & Platform Engineer @ Renault Group.
- Location: Paris, France.
- Certifications to keep visible: CKA, CKAD (both verifiable via Credly/Acclaim links), LFS158x (edX), RHCSA, LPIC-2, LPIC-1.

## Evidence on Hand

All content currently on the page (roles, dates, responsibilities, certifications, contact details, social links) is confirmed accurate by the user and is binding fact, not placeholder copy — future work must preserve it as-is rather than treating it as sample content to rewrite. No additional testimonials, press, or case studies exist and none should be fabricated.

## Product Principles

1. Lead with the migration → platform-build → platform-ownership throughline; never fragment it back into three unrelated jobs.
2. Every claim on the page must be truthful and traceable to the user's actual history — no invented metrics, testimonials, or employers.
3. Optimize for a hiring manager's first-scan credibility: scope (1,000+ apps, ~8 years), continuity (one org, three roles), and verifiability (linked certifications).
4. Keep the site a single dependency-free HTML file deployable straight to GitHub Pages — no build step required to ship an edit.
5. Contact must stay frictionless: direct email/phone, not a form.
