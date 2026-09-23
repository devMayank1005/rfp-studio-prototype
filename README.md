# RFP Studio prototype

A clickable design prototype of **Kognoz RFP Studio**. It's one static HTML file with no build step and no dependencies apart from Google Fonts.

It has 23 screens, grouped the way the product flows:

- **Sign in & access:** desktop sign-in, phone sign-in with the domain error, no-workspace page
- **Pipeline:** dashboard table and board views, ⌘K command palette
- **RFP setup wizard:** client, upload, extraction running, review extracted questions, confirm
- **Review workspace:** the three-pane grid (click rows, switch panel tabs, tick checkboxes for the bulk bar), the dark "late shift" theme, the keyboard sheet
- **After review:** CHRO discovery questions, exports
- **Knowledge base & Quick Q&A:** entry list, entry editor, new session, session results
- **Settings:** team, brand, voice guide

Move between screens with the links inside the mockups, or with the ← → buttons and the **All screens** menu at the bottom. Every screen has its own URL fragment (for example `/#workspace`), so you can link straight to one.

## Data

The Apex Manufacturing RFP, its 24 questions and answers, the knowledge-base entries and the voice guide come from the RFP Studio seed data. The other pipeline clients (Meridian Telecom, Harbourview Properties, Northwind Metals, Crestline Auto), the Quick Q&A sessions and the CHRO questions are made-up samples. Team members other than the admin are placeholders.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Deploy

Import the repo at vercel.com/new. Leave the framework preset as **Other**, with no build command and the output directory set to the repo root. `vercel.json` adds a `noindex` header so search engines skip the site.
