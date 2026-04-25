# 💰 Money Moves — PA Financial Literacy App

An interactive, browser-based financial literacy app for students in grades 5–12, aligned to the **Pennsylvania Academic Standards for Personal Finance (17.1–17.6)**, effective July 1, 2026.

Built by a BCIT educator in the Philadelphia, PA area.

---

## 🎯 What It Does

Students choose a difficulty level, pick a real-life financial scenario, and work through **6 weeks of structured activity** — each week has three required phases that must be completed in order. Every decision is tied to a specific PA Standard and takes **20+ minutes per scenario** to complete thoughtfully.

**No accounts. No login. No data collected. No cost to run.**

---

## 📋 How Each Week Works — Three Required Phases

Every week in every scenario follows this exact structure. Students cannot skip any phase.

### Phase 1 — 📐 Math Challenge
Before any choices appear, students must solve a math problem directly related to the scenario. Examples include:
- Calculating profit (income − expenses)
- Finding hourly wage rates
- Computing percentages and discounts
- Applying simple interest formulas
- Determining opportunity cost in dollars

Students must enter the correct answer to unlock the scenario choices. After **2 failed attempts**, a hint appears. This ensures students engage with the numbers before making a decision.

### Phase 2 — 📖 Decision
Once the math is solved, the scenario situation and three choices appear. Each choice shows its financial impact (income earned or expense incurred) upfront so students can reason through the tradeoffs before clicking. The relevant PA Standard code is displayed at the bottom of each decision.

### Phase 3 — ✍️ Written Reflection
After making a choice, students see the consequence of their decision and are presented with a reflection prompt. They must write a **minimum of 80 characters** before they can advance to the next week. A live character counter shows their progress. Reflection prompts connect the scenario to real-life personal finance thinking.

---

## 📚 PA Standards Coverage

| Standard | Area | Scenarios |
|---|---|---|
| 17.1 | Personal Finance Fundamentals | All scenarios |
| 17.2 | Income | Lemonade Stand, Babysitting, Lawn Mowing |
| 17.3 | Spending | Back to School, Lemonade Stand, Emergency |
| 17.4 | Saving & Investing | Saving for Something Big, Lawn Mowing |
| 17.5 | Risk & Insurance | Unexpected Expenses, Babysitting, Lawn Mowing |
| 17.6 | Credit | Saving for Something Big, Unexpected Expenses |

Each week displays the specific standard code (e.g., `17.3.6-8.B`) so students and teachers can connect decisions directly to curriculum objectives.

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

## 📊 Budget Tracker — Spreadsheet Component

Every scenario includes a live **Budget Ledger tab** that auto-populates as students make decisions. Students can toggle to it at any time during a scenario. It shows:

- Week-by-week income and expenses
- Running balance after each decision
- Totals row (total income, total expenses, final balance)
- Net change from starting balance

This supports spreadsheet literacy alongside financial literacy — students see their financial data organized in a structured table format, similar to a real budget spreadsheet.

---

## ⏱️ Time Per Scenario

Each of the 6 weeks includes a math problem, a decision, and a written reflection. A student working carefully and thoughtfully should spend **20–30 minutes per scenario**. Faster students who rush through reflections will be slowed by the 80-character minimum requirement.

---

## 🚀 How to Use

### For Students
1. Open the app link in any browser
2. Enter your name
3. Choose a difficulty level
4. Pick a scenario
5. Solve the math challenge to unlock your choices
6. Read the situation carefully and make your decision
7. Write your reflection (minimum 80 characters) before advancing
8. Check the Budget Tracker tab anytime to see your running totals
9. Review your full decision history at the summary screen

### For Teachers
- No setup required — share the link and students are ready to go
- Works on school Chromebooks, laptops, and tablets
- Can be used as a multi-day activity, independent work, or a class discussion starter
- After playing, discussion prompts:
  - *Which decision would you make differently? Why?*
  - *How did the math challenge change the way you thought about your choice?*
  - *What did someone else's reflection teach you?*
- The PA Standard code shown each week connects directly to lesson objectives
- Student reflections can be used as written assessment evidence

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

**Privacy:** This app collects zero student data. Names entered on the welcome screen exist only in the browser's memory for that session and are never transmitted anywhere. Fully compliant with FERPA and COPPA by design — there is nothing to report because nothing is stored.

---

## 📁 Files

```
MoneyMoves/
├── index.html    ← The entire app (single file)
└── README.md     ← This file
```

---

## ✏️ Customizing Scenarios

All scenario content is written in the `SCENARIOS` array near the top of the script section in `index.html`. Each week follows this structure:

```
week: 1,
narrative: "The story students read...",
situation: "The decision they face...",
paStandard: "17.3.6-8.B",
tip: "A financial literacy tip...",
mathChallenge: {
  question: "The math problem...",
  answer: 12,         ← the correct numerical answer
  tolerance: 0.01,    ← how close the student's answer needs to be
  hint: "Shown after 2 wrong attempts..."
},
reflectionPrompt: "The writing prompt students must respond to...",
choices: [
  {
    text: "What the choice says...",
    impact: { income: 0, expense: 8, description: "Ledger entry text" },
    consequence: "What happens as a result..."
  },
  ...
]
```

No coding experience is required to edit narrative text, math questions, reflection prompts, or financial impacts — just find the relevant section and update the text.

---

## 🏗️ Future Development Ideas

- [ ] Printable summary report for student portfolios
- [ ] Teacher dashboard showing class results
- [ ] Additional scenarios (first checking account, tax filing, renting an apartment, job application)
- [ ] Adjustable reflection minimum character count for different grade levels
- [ ] Print-friendly budget ledger export
- [ ] Expanded difficulty branching with different narrative text per level

---

## 👩‍🏫 About

Created for use in a **BCIT (Business, Computer & Information Technology)** middle school classroom in Pennsylvania. Designed to be practical, standards-aligned, and deployable without any IT infrastructure beyond a web browser.

Feedback and contributions welcome.
