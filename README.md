# 💰 Money Moves — PA Financial Literacy App

An interactive, browser-based financial literacy app for students in grades 5–12, aligned to the **Pennsylvania Academic Standards for Personal Finance (17.1–17.6)**, effective July 1, 2026.

Built by a BCIT educator in the Levittown, PA area.

---

## 🎯 What It Does

Students choose a difficulty level, pick a real-life financial scenario, and work through **6 weeks of decisions** — each one tied to a specific PA Standard. Every choice has real financial consequences tracked in a live budget ledger.

**No accounts. No login. No data collected. No cost to run.**

---

## 📚 PA Standards Coverage

| Standard | Area | Scenarios |
|---|---|---|
| 17.1 | Personal Finance Fundamentals | All scenarios |
| 17.2 | Income | Lemonade Stand, Babysitting, Lawn Mowing |
| 17.3 | Spending | Back to School, Lemonade Stand, Emergency |
| 17.4 | Saving & Investing | Saving for Something Big, Lawn Mowing |
| 17.5 | Risk & Insurance | Unexpected Expenses, Babysitting, Lawn Mowing |
| 17.6 | Credit | Saving for Something Big |

Each scenario week displays the specific standard code (e.g., `17.3.6-8.B`) so students and teachers can connect decisions to curriculum.

---

## 🗂️ Scenarios Included

| Scenario | Starting Balance | Primary Standards | Focus |
|---|---|---|---|
| 🍋 Lemonade Stand | $20 | 17.2, 17.3 | Entrepreneurship, pricing, competition |
| 👶 Babysitting Business | $15 | 17.2, 17.3, 17.5 | Service business, rates, reputation |
| 🌿 Lawn Mowing Service | $25 | 17.2, 17.4, 17.5 | Equipment, risk, seasonal saving |
| 🎒 Back to School Budget | $100 | 17.3 | Comparison shopping, peer pressure |
| 🎯 Saving for Something Big | $30 | 17.4, 17.1 | Goal setting, delayed gratification |
| ⚡ Unexpected Expenses | $80 | 17.5, 17.4, 17.3 | Emergency funds, real-life surprises |

---

## 🏫 Difficulty Levels

| Level | Grade Band | PA Standards Tier |
|---|---|---|
| Just Starting Out | Grades 3–5 | 17.x.3-5 |
| Getting the Hang of It | Grades 6–8 | 17.x.6-8 |
| Money Pro | Grades 9–12 | 17.x.9-12 |

Students self-select their level. A motivated 5th grader can challenge themselves with a harder level; a struggling 9th grader can rebuild confidence at a lower tier.

---

## 📊 Budget Tracker (Spreadsheet Component)

Every scenario includes a live **Budget Ledger tab** that auto-populates as students make decisions. It shows:

- Week-by-week income and expenses
- Running balance after each decision
- Total income, total expenses, and net change
- Starting balance vs. final balance comparison

This supports spreadsheet literacy alongside financial literacy — students can see their data in a structured table format in real time.

---

## 🚀 How to Use

### For Students
1. Open the app link in any browser
2. Enter your name
3. Choose a difficulty level
4. Pick a scenario
5. Read each week's situation and make a decision
6. Watch your budget update — check the Budget Tracker tab anytime
7. Review your full decision history at the summary screen

### For Teachers
- No setup required — share the link and students are ready to go
- Works on school Chromebooks, laptops, and tablets
- Can be used as a warm-up, independent activity, or class discussion prompt
- After playing, discuss: *Which choice would you make differently? Why?*
- The PA Standard code shown each week connects directly to lesson objectives

---

## 🛠️ Technical Details

| Property | Value |
|---|---|
| File type | Single HTML file (`index.html`) |
| Framework | React 18 (loaded via CDN) |
| Backend | None |
| Database | None |
| Student data stored | None |
| Internet required | Only to first load the page |
| API keys required | None |
| Cost to host | Free (GitHub Pages) |

**Privacy:** This app collects zero student data. Names entered on the welcome screen exist only in the browser's memory for that session and are never transmitted anywhere. Compliant with FERPA and COPPA by design.

---

## 📁 Files

```
money-moves/
├── index.html    ← The entire app (single file)
└── README.md     ← This file
```

---

## ✏️ Customizing Scenarios

All scenario content is written directly in `index.html` in a clearly labeled `SCENARIOS` data array near the top of the script section. To edit a scenario or add a new one, find the relevant section and update the text — no coding experience required beyond basic copy/paste.

Each week follows this structure:
- `narrative` — the story text students read
- `situation` — the decision they face
- `choices` — three options, each with a financial impact and consequence text
- `paStandard` — the PA Standard code for that decision
- `tip` — a brief financial literacy tip

---

## 🏗️ Future Development Ideas

- [ ] Printable summary report for student portfolios
- [ ] Teacher dashboard showing class results
- [ ] Additional scenarios (first checking account, tax filing, renting an apartment)
- [ ] Editable spreadsheet component where students manually enter their own budgets
- [ ] Expanded difficulty branching with different narrative text per level

---

## 👩‍🏫 About

Created for use in a **BCIT (Business, Computer & Information Technology)** middle school classroom in Pennsylvania. Designed to be practical, standards-aligned, and deployable without any IT infrastructure beyond a web browser.

Feedback and contributions welcome.
