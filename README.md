# AEC Resume Building & Scoring Toolkit

A free, browser-based resume builder and scorer built specifically for
architects, civil/structural engineers, and MEP engineers.

**Live site:** _add your GitHub Pages URL here once deployed_

Built by **Ar. Neeraj**.

## What it does

- **Build** — a guided editor with a live preview, six visual presets, and
  fine-tuning knobs (typeface, heading style, density, bullets, colour).
- **Score** — grades an existing resume section-by-section against the
  vocabulary of your specific discipline (Architecture / Civil & Structural
  / MEP).
- **Job match** — paste a job description and see exactly which
  requirements aren't yet covered, matched by meaning using an AEC synonym
  map, not just literal keywords.
- **Import** — paste or upload an existing resume (PDF, .txt, .md) and it's
  split into editable fields.
- **Bullet coach** — flags weak openers, missing numbers, and bloated
  bullets, one at a time.
- **Versions** — save one version per application and track its status.
- **Export** — a real, text-based PDF (selectable text, ATS-readable) or a
  Word file.

## Why

Generic resume advice is written for software and consulting roles. AEC is
a portfolio-led discipline with its own vocabulary (Revit, ASHRAE, IS
codes, BOQ, clash detection), and design-trained candidates tend to build
exactly the resumes that applicant tracking systems reject — columns,
icons, skill bars — usually without ever finding out why they heard
nothing back.

## Privacy

Everything runs client-side, in your browser. No resume text, file, or
personal data is ever sent to a server or stored anywhere but your own
device (via `localStorage`, for drafts and saved versions only). See
[PRIVACY.md](PRIVACY.md) for the full explanation.

The one optional exception: if you add your own Anthropic API key in Score
mode or the Bullet Coach, your resume text is sent directly from your
browser to Anthropic's API for AI-generated feedback. This is entirely
optional and off by default.

## Running it locally

This is a single self-contained HTML file. Clone the repo and open
`index.html` in any modern browser — no build step, no server, no
dependencies to install.

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
open index.html   # or just double-click it
```

## Tech

Plain HTML/CSS/JS. No framework, no bundler. Two CDN libraries load only
when needed: [jsPDF](https://github.com/parallax/jsPDF) for PDF export,
and [pdf.js](https://mozilla.github.io/pdf.js/) for reading uploaded PDFs.

## License

MIT — see [LICENSE](LICENSE). Use it, fork it, adapt it.

## Feedback

This is an early build. If something breaks, parses your resume oddly, or
scores something in a way that doesn't make sense, feel free to open an
issue.
