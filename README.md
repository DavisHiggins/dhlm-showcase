<p align="center">
  <a href="https://dhlm.davishiggins.com"><img src="assets/hero.svg" width="100%" alt="DHLM: my digital life, one intelligence layer. Animated cover with the LM mark beside mail, calendar, files, and notes nodes routing light into a central core, followed by a cited answer streaming in." /></a>
</p>

<h1 align="center">DHLM</h1>

<p align="center"><strong>A private AI workspace that answers from my email, calendar, files, and personal notes, with sources cited and every change confirmed.</strong></p>

<p align="center">
  <a href="https://dhlm.davishiggins.com"><img src="assets/btn-open.svg" height="44" alt="Read the case study" /></a>&nbsp;
  <a href="https://www.higginsd.com/work/dhlm"><img src="assets/btn-case.svg" height="44" alt="Studio write-up" /></a>&nbsp;
  <a href="https://davishiggins.com"><img src="assets/btn-dh.svg" height="44" alt="Davis Higgins" /></a>
</p>

<p align="center"><sub>Private application · Public case study with synthetic data · Designed and built by Davis Higgins</sub></p>

---

## See it in motion

<p align="center">
  <img src="assets/demo.gif" width="800" alt="Screen recording of the DHLM case study: scrolling through synthetic workflow previews for email context, calendar clarity, and file discovery, each showing a plain request, the sources it touched, and a cited answer." />
</p>

<p align="center"><sub>Real capture of the public case study's workflow section. Every preview uses synthetic data. <a href="assets/demo.png">Static frame</a></sub></p>

## What it does

- **One question, the right sources.** Ask about the week and DHLM works out which of my notes, email, calendar, or files it needs, then answers with every source cited.
- **Drafts, never sends.** It can prepare an email draft or a calendar event, show a preview, and act only after I confirm.
- **Memory I approve.** When a conversation surfaces something worth remembering, DHLM proposes the update and saves it only after I say yes.

## Why I built it

The context behind a decision is usually split three ways. One email holds a detail, a calendar event holds the time, and a document holds the rest. Answering a simple question about my week meant opening three apps and stitching the answer together by hand.

Handing a general assistant full access to all of it would trade a searching problem for a trust problem. So I built one private workspace that reads only what a question needs, cites it, and changes nothing without confirmation.

## What I built

I designed and built DHLM end to end:

- The chat and command workspace, with streamed answers and citations beside every response
- The intelligence layer that decides which sources a request needs
- Integrations with my email, calendar, and files
- Confirmed drafts and events, approval-gated memory, and a full activity record
- A career workspace for job discovery and application tracking
- The public case study, with synthetic previews of six workflows

<details>
<summary><strong>How it's put together</strong></summary>

<br />

```mermaid
flowchart TB
    Q[Request] --> L[DHLM intelligence layer]
    L --> K[Personal notes]
    L --> S[Email · Calendar · Files]
    K --> A[Answer with citations]
    S --> A
    A -.->|optional| D[Prepared draft or event] --> C{I confirm} --> X[Action + activity record]
```

| Decision | Why |
|---|---|
| **Only what the question needs** | Each request reaches only the sources it actually requires, which keeps answers focused and limits what any single answer can see. |
| **Access is deliberate** | Signing in and connecting data are separate steps, and anything beyond reading is opt-in. |
| **Every action is confirmed** | Nothing is sent, scheduled, or remembered until I've reviewed exactly what will happen, and every action is recorded. |

</details>

## Screens

<table>
  <tr>
    <td width="62%"><img src="assets/screenshot-home.png" alt="DHLM case study hero: 'My digital life. One intelligence layer.' beside a synthetic chat preview routing a calendar question." /></td>
    <td rowspan="2" width="38%" align="center"><img src="assets/screenshot-mobile.png" width="300" alt="DHLM case study on a phone with the hero headline and the synthetic chat preview." /></td>
  </tr>
  <tr>
    <td><img src="assets/screenshot-control.png" alt="DHLM 'Access is intentional. Actions are explicit.' section on the case study." /></td>
  </tr>
</table>

<sub>Case study hero (synthetic preview) · Access and control · Case study on mobile</sub>

## Technology

| Layer | Technology |
|---|---|
| App and case study | Next.js, React, TypeScript |
| Data | Supabase |
| Motion | GSAP, Lenis |
| Hosting | Vercel |

---

<p align="center">
  <a href="https://dhlm.davishiggins.com"><img src="assets/btn-open.svg" height="44" alt="Read the case study" /></a>&nbsp;
  <a href="https://github.com/DavisHiggins"><img src="assets/btn-more.svg" height="44" alt="More of my work" /></a>
</p>

<p align="center"><sub>© 2026 Davis Higgins. All rights reserved. The DHLM, LM, and DH marks belong to Davis Higgins.</sub></p>
