# Train the Trainer: AI Coding Assistants Training for Financial Professionals

## Product Requirements Document (PRD)

**Version:** 1.0  
**Date:** February 4, 2026  
**Author:** Treasury Innovation Team  
**Repository:** github.com/jimkliew/buildBestPracticesStartsInWindsurf

---

## 1. Executive Summary

This self-paced course empowers Treasury professionals to become internal champions for AI coding assistants. Participants will learn to use Windsurf (Cascade and Flows) to build dashboards, automate reports, analyze peer companies, and create their own PRD.md files—skills they can then teach to colleagues across the organization.

**Target Audience:** Treasury executives and senior analysts who will train others  
**Business Outcome:** Accelerate AI adoption, reduce manual work, improve decision-making speed  
**ROI Drivers:** Time savings, error reduction, faster insights, scalable training

---

## 2. Course Overview

| Attribute | Detail |
|-----------|--------|
| **Course Title** | Train the Trainer: AI Coding Assistants Training for Financial Professionals |
| **Duration** | ~4 hours (self-paced, variable by module) |
| **Format** | Mixed: conceptual explanations + hands-on exercises |
| **Prerequisites** | Basic Excel/data familiarity; no coding required |
| **Data Sources** | Public only (FRED, SEC EDGAR, Yahoo Finance, Wikipedia) |
| **Compliance** | Simulation environment; no proprietary data used |
| **Vendor Neutral** | Concepts apply to multiple AI assistants |

---

## 3. Learning Objectives

By completing this course, participants will be able to:

1. **Navigate Windsurf** — Understand Cascade (AI chat) and Flows (automated workflows)
2. **Build PRD.md Files** — Use AI to draft, iterate, and refine product requirements
3. **Create Dashboards** — Build Treasury-focused visualizations with public data
4. **Automate Reports** — Generate scripts for recurring Treasury tasks
5. **Analyze Peer Groups** — Compare banks, financials, and tech companies
6. **Troubleshoot Effectively** — Recognize when to iterate vs. restart
7. **Train Others** — Teach these skills to colleagues with confidence

---

## 4. Module Structure

### Module Overview Table

| Module | Topic | Duration | Complexity | Key Deliverable |
|--------|-------|----------|------------|-----------------|
| 1 | Windsurf Fundamentals | 30 min | ⭐ | First PRD.md file |
| 2 | Cash Management Dashboard | 45 min | ⭐⭐ | Cash position tracker |
| 3 | Debt Management Analysis | 45 min | ⭐⭐ | Debt schedule comparison |
| 4 | Investments & Peer Analysis | 60 min | ⭐⭐⭐ | Peer group widget |
| 5 | Automation & Reporting | 50 min | ⭐⭐⭐ | Automated report script |
| 6 | Troubleshooting & Best Practices | 30 min | ⭐⭐ | Decision tree for restarts |

**Total:** ~4 hours 20 minutes

---

### Module 1: Windsurf Fundamentals (30 min) ⭐

#### What You'll Learn
- Windsurf interface overview
- **Cascade** — The AI chat assistant for coding and analysis
- **Flows** — Automated multi-step workflows
- When to use each tool

#### Cascade vs. Flows Decision Chart

```
┌─────────────────────────────────────────────────────────────┐
│                    WHAT ARE YOU DOING?                      │
└─────────────────────────────────────────────────────────────┘
                            │
            ┌───────────────┴───────────────┐
            ▼                               ▼
    ┌───────────────┐               ┌───────────────┐
    │  One-time or  │               │   Repeatable  │
    │  exploratory  │               │   multi-step  │
    │     task?     │               │    process?   │
    └───────────────┘               └───────────────┘
            │                               │
            ▼                               ▼
    ┌───────────────┐               ┌───────────────┐
    │  USE CASCADE  │               │   USE FLOWS   │
    │               │               │               │
    │ • Chat-based  │               │ • Automated   │
    │ • Interactive │               │ • Scheduled   │
    │ • Iterative   │               │ • Consistent  │
    └───────────────┘               └───────────────┘
```

#### Hands-On Exercise 1.1: Your First PRD.md

**Objective:** Create a simple PRD.md file using Cascade

**Steps:**
1. Open Windsurf and start a new Cascade session
2. Type: *"Help me create a PRD.md for a Treasury cash forecasting tool"*
3. Review the AI's response
4. Iterate: *"Add a section for data sources using only public APIs"*
5. Save the file as `my-first-prd.md`

**Success Criteria:**
- [ ] PRD contains at least 5 sections
- [ ] Data sources section lists public APIs
- [ ] File saved in your workspace

---

### Module 2: Cash Management Dashboard (45 min) ⭐⭐

#### What You'll Learn
- Fetching public Treasury data (FRED API)
- Building a cash position visualization
- Dashboard layout best practices

#### Public Data Sources for Cash Management

| Source | Data Available | URL |
|--------|---------------|-----|
| **FRED** | Interest rates, Treasury yields, money supply | fred.stlouisfed.org |
| **Treasury.gov** | Daily Treasury statements, debt data | fiscaldata.treasury.gov |
| **Yahoo Finance** | Stock prices, company financials | finance.yahoo.com |

#### Hands-On Exercise 2.1: Cash Position Dashboard

**Objective:** Build a dashboard showing Treasury yields and cash metrics

**Prompt to Use:**
```
Create a Python dashboard that:
1. Fetches 10-year Treasury yield from FRED (series: DGS10)
2. Fetches 2-year Treasury yield (series: DGS2)
3. Calculates the yield curve spread
4. Displays a chart showing the last 12 months
5. Shows current values in a summary table

Use only public data. Make it visually clean.
```

**Expected Output:**
- Line chart with yield curves
- Summary table with current rates
- Yield spread indicator (positive/negative)

#### Sample Dashboard Layout

```
┌─────────────────────────────────────────────────────────────┐
│                 TREASURY YIELD DASHBOARD                    │
├─────────────────────────────────────────────────────────────┤
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐      │
│  │  10Y Yield   │  │   2Y Yield   │  │   Spread     │      │
│  │    4.25%     │  │    4.10%     │  │   +0.15%     │      │
│  │     ▲ +5bp   │  │     ▼ -3bp   │  │   NORMAL     │      │
│  └──────────────┘  └──────────────┘  └──────────────┘      │
│                                                             │
│  ┌─────────────────────────────────────────────────────┐   │
│  │                                                     │   │
│  │          [12-Month Yield Curve Chart]              │   │
│  │                                                     │   │
│  │    ────── 10Y    ────── 2Y    ────── Spread        │   │
│  │                                                     │   │
│  └─────────────────────────────────────────────────────┘   │
└─────────────────────────────────────────────────────────────┘
```

---

### Module 3: Debt Management Analysis (45 min) ⭐⭐

#### What You'll Learn
- Analyzing public company debt schedules
- Comparing debt metrics across companies
- Building debt maturity visualizations

#### Companies for Analysis (Public Data)

| Company | Ticker | Sector | Why Include |
|---------|--------|--------|-------------|
| Apple | AAPL | Technology | Large cash/debt position |
| Microsoft | MSFT | Technology | Investment grade issuer |
| JPMorgan Chase | JPM | Banking | Major bank, complex debt |
| Goldman Sachs | GS | Banking | Investment bank focus |
| Berkshire Hathaway | BRK.B | Financials | Unique capital structure |

#### Hands-On Exercise 3.1: Debt Comparison Table

**Objective:** Create a debt metrics comparison for 3 companies

**Prompt to Use:**
```
Create a Python script that:
1. Fetches financial data for AAPL, MSFT, and JPM from Yahoo Finance
2. Extracts: Total Debt, Cash, Debt-to-Equity, Interest Coverage
3. Displays a formatted comparison table
4. Highlights the company with the strongest balance sheet

Use yfinance library. Format numbers clearly (billions, ratios).
```

**Expected Output Table:**

| Metric | Apple | Microsoft | JPMorgan |
|--------|-------|-----------|----------|
| Total Debt | $111B | $79B | $298B |
| Cash & Equivalents | $62B | $81B | $45B |
| Net Debt | $49B | -$2B | $253B |
| Debt/Equity | 1.8x | 0.4x | 1.2x |
| **Strongest** | | ✓ | |

---

### Module 4: Investments & Peer Analysis (60 min) ⭐⭐⭐

#### What You'll Learn
- Building peer group comparisons
- Creating interactive widgets
- Analyzing banks vs. tech companies

#### Peer Group Framework

```
┌─────────────────────────────────────────────────────────────┐
│                    PEER GROUP ANALYSIS                      │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│   BANKS              TECH               DIVERSIFIED         │
│   ─────              ────               ───────────         │
│   • JPMorgan         • Apple            • Berkshire         │
│   • Goldman Sachs    • Microsoft        • GE                │
│   • Bank of America  • Google           • 3M                │
│   • Citigroup        • Amazon           • Johnson & Johnson │
│   • Wells Fargo      • Meta             • Procter & Gamble  │
│                                                             │
│   Key Metrics:       Key Metrics:       Key Metrics:        │
│   • NIM              • Cash/Revenue     • Debt/EBITDA       │
│   • CET1 Ratio       • R&D Spend        • Dividend Yield    │
│   • ROE              • FCF Margin       • Credit Rating     │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

#### Hands-On Exercise 4.1: Peer Group Widget

**Objective:** Build an interactive peer comparison widget

**Prompt to Use:**
```
Create a Python Streamlit app that:
1. Lets user select a peer group (Banks, Tech, or Diversified)
2. Fetches key metrics for 5 companies in that group
3. Displays a comparison table with conditional formatting
4. Shows a bar chart comparing a selected metric
5. Exports results to CSV

Companies:
- Banks: JPM, GS, BAC, C, WFC
- Tech: AAPL, MSFT, GOOGL, AMZN, META
- Diversified: BRK.B, GE, MMM, JNJ, PG

Use yfinance for data. Make it visually professional.
```

**Widget Layout:**

```
┌─────────────────────────────────────────────────────────────┐
│  PEER GROUP ANALYZER                          [Refresh] [Export]│
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  Select Peer Group: [Banks ▼]    Select Metric: [ROE ▼]    │
│                                                             │
│  ┌─────────────────────────────────────────────────────┐   │
│  │  Company  │ Market Cap │  ROE   │  P/E  │ Div Yield │   │
│  ├───────────┼────────────┼────────┼───────┼───────────┤   │
│  │  JPM      │   $580B    │ 15.2%  │ 12.1  │   2.4%    │   │
│  │  GS       │   $145B    │ 12.8%  │ 14.3  │   2.1%    │   │
│  │  BAC      │   $310B    │ 10.5%  │ 11.8  │   2.6%    │   │
│  │  C        │   $120B    │  8.2%  │  9.5  │   3.1%    │   │
│  │  WFC      │   $195B    │ 11.1%  │ 12.0  │   2.8%    │   │
│  └─────────────────────────────────────────────────────┘   │
│                                                             │
│  ┌─────────────────────────────────────────────────────┐   │
│  │  ROE Comparison                                     │   │
│  │  JPM  ████████████████ 15.2%                       │   │
│  │  GS   █████████████ 12.8%                          │   │
│  │  WFC  ███████████ 11.1%                            │   │
│  │  BAC  ██████████ 10.5%                             │   │
│  │  C    ████████ 8.2%                                │   │
│  └─────────────────────────────────────────────────────┘   │
└─────────────────────────────────────────────────────────────┘
```

---

### Module 5: Automation & Reporting (50 min) ⭐⭐⭐

#### What You'll Learn
- Creating automated data refresh scripts
- Building recurring reports
- Using Flows for scheduled tasks

#### Automation Use Cases for Treasury

| Use Case | Frequency | Complexity | ROI Impact |
|----------|-----------|------------|------------|
| Daily rate monitoring | Daily | Low | High |
| Weekly peer comparison | Weekly | Medium | Medium |
| Monthly debt analysis | Monthly | Medium | High |
| Quarterly board report | Quarterly | High | Very High |

#### Hands-On Exercise 5.1: Automated Morning Report

**Objective:** Create a script that generates a daily Treasury briefing

**Prompt to Use:**
```
Create a Python script that generates a daily Treasury morning report:

1. Fetch today's data:
   - 10Y and 2Y Treasury yields from FRED
   - S&P 500 level from Yahoo Finance
   - Top 5 bank stock prices (JPM, GS, BAC, C, WFC)

2. Calculate:
   - Yield curve spread
   - Daily changes for all metrics

3. Generate a formatted report with:
   - Executive summary (3 bullet points)
   - Key metrics table
   - Notable moves (anything >1% change)

4. Save as both .txt and .html files

Make it suitable for executive distribution.
```

**Sample Output:**

```
═══════════════════════════════════════════════════════════════
              TREASURY MORNING BRIEFING
              February 4, 2026
═══════════════════════════════════════════════════════════════

EXECUTIVE SUMMARY
─────────────────
• Yield curve remains normal with +15bp spread (10Y-2Y)
• Bank stocks mixed; JPM +1.2%, C -0.8%
• S&P 500 flat at 5,890 (+0.1%)

KEY METRICS
───────────────────────────────────────────────────────────────
Metric                  Value           Change      Status
───────────────────────────────────────────────────────────────
10Y Treasury            4.25%           +5bp        ▲
2Y Treasury             4.10%           -3bp        ▼
Yield Spread            +0.15%          +8bp        NORMAL
S&P 500                 5,890           +0.1%       ─
───────────────────────────────────────────────────────────────

BANK STOCKS
───────────────────────────────────────────────────────────────
Ticker    Price       Change      52W Range
───────────────────────────────────────────────────────────────
JPM       $198.50     +1.2%       $145 - $205
GS        $425.30     +0.5%       $320 - $440
BAC       $38.20      -0.3%       $28 - $42
C         $62.10      -0.8%       $45 - $68
WFC       $58.90      +0.2%       $42 - $62
───────────────────────────────────────────────────────────────

NOTABLE MOVES (>1% change)
─────────────────────────
• JPM: +1.2% — Strong earnings expectations

═══════════════════════════════════════════════════════════════
Report generated: 2026-02-04 07:00:00 EST
═══════════════════════════════════════════════════════════════
```

#### Using Flows for Automation

**Flow Setup Steps:**
1. Create the Python script (Exercise 5.1)
2. Open Windsurf Flows
3. Create new Flow: "Daily Treasury Briefing"
4. Set trigger: Daily at 7:00 AM
5. Add action: Run Python script
6. Add action: Save output to designated folder
7. (Optional) Add action: Email notification

---

### Module 6: Troubleshooting & Best Practices (30 min) ⭐⭐

#### What You'll Learn
- Common pitfalls that get you stuck
- When to iterate vs. restart
- Best practices for AI-assisted development

---

## 5. Best Practices

### Top 5 Do's ✅

| # | Do This | Why It Matters |
|---|---------|----------------|
| 1 | **Start with a clear PRD.md** | AI performs better with structured requirements |
| 2 | **Use specific, measurable requests** | "Create a table with 5 columns" beats "make a table" |
| 3 | **Iterate in small steps** | Build incrementally; validate each piece |
| 4 | **Provide context about your data** | Tell AI the source, format, and constraints |
| 5 | **Save working versions frequently** | Create checkpoints before major changes |

### Top 5 Don'ts ❌

| # | Don't Do This | What Happens |
|---|---------------|--------------|
| 1 | **Don't ask for everything at once** | AI gets confused; output is unfocused |
| 2 | **Don't ignore error messages** | Errors contain clues; read them carefully |
| 3 | **Don't keep iterating on broken code** | After 3 failed attempts, restart fresh |
| 4 | **Don't use vague language** | "Make it better" gives unpredictable results |
| 5 | **Don't skip the PRD step** | No PRD = no shared understanding = rework |

---

## 6. Troubleshooting Guide

### Decision Tree: Iterate or Restart?

```
┌─────────────────────────────────────────────────────────────┐
│                 IS YOUR CODE WORKING?                       │
└─────────────────────────────────────────────────────────────┘
                            │
                ┌───────────┴───────────┐
                ▼                       ▼
            YES, but                    NO
            needs tweaks                │
                │                       │
                ▼                       ▼
        ┌─────────────┐         ┌─────────────────┐
        │  ITERATE    │         │ How many times  │
        │             │         │ have you tried? │
        │ • Small fix │         └─────────────────┘
        │ • Add feature│                │
        │ • Refine UI │         ┌───────┴───────┐
        └─────────────┘         ▼               ▼
                            1-2 times       3+ times
                                │               │
                                ▼               ▼
                        ┌─────────────┐  ┌─────────────┐
                        │  ITERATE    │  │  RESTART    │
                        │             │  │             │
                        │ • Read error│  │ • New chat  │
                        │ • Fix issue │  │ • Rephrase  │
                        │ • Try again │  │ • Simplify  │
                        └─────────────┘  └─────────────┘
```

### Common "Holes" That Get You Stuck

| Problem | Symptom | Solution |
|---------|---------|----------|
| **Vague requirements** | AI asks clarifying questions repeatedly | Write a PRD.md first |
| **Missing dependencies** | Import errors, module not found | Ask AI to list all required packages |
| **Wrong data format** | Type errors, parsing failures | Specify exact format in your prompt |
| **Scope creep** | Code gets complex, hard to debug | Break into smaller tasks |
| **Conflicting instructions** | AI produces inconsistent output | Start fresh with clear, single goal |

### When to Restart: Warning Signs

1. **Error loops** — Same error appears 3+ times despite fixes
2. **Code bloat** — File has grown beyond what you can understand
3. **Lost context** — AI seems to have forgotten earlier requirements
4. **Fundamental flaw** — Architecture is wrong, not just details
5. **Frustration threshold** — You've spent 15+ minutes on one issue

### Restart Checklist

- [ ] Save any working code snippets
- [ ] Note what worked and what didn't
- [ ] Simplify your requirements
- [ ] Start a new Cascade session
- [ ] Begin with your PRD.md

---

## 7. Charts & Widgets Gallery

### Treasury Dashboard Templates

#### Template 1: Executive Summary Dashboard

```
┌─────────────────────────────────────────────────────────────┐
│                    TREASURY EXECUTIVE DASHBOARD             │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  KEY METRICS                           ALERTS               │
│  ┌────────┐ ┌────────┐ ┌────────┐     ┌─────────────────┐  │
│  │ Cash   │ │ Debt   │ │ Yield  │     │ ⚠ Rate spike    │  │
│  │ $2.1B  │ │ $850M  │ │ 4.25%  │     │ ⚠ Maturity due  │  │
│  │ ▲ +5%  │ │ ─ flat │ │ ▲ +10bp│     │ ✓ All clear     │  │
│  └────────┘ └────────┘ └────────┘     └─────────────────┘  │
│                                                             │
│  TREND CHARTS                                               │
│  ┌─────────────────────────────────────────────────────┐   │
│  │     Cash Position (12 months)                       │   │
│  │  $2.5B ┤                              ╭─────        │   │
│  │  $2.0B ┤              ╭───────────────╯             │   │
│  │  $1.5B ┤─────────────╯                              │   │
│  │        └────────────────────────────────────────    │   │
│  │         Mar  Apr  May  Jun  Jul  Aug  Sep  Oct      │   │
│  └─────────────────────────────────────────────────────┘   │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

#### Template 2: Peer Comparison Widget

```
┌─────────────────────────────────────────────────────────────┐
│  PEER COMPARISON: BANKS                    [Refresh] [Export]│
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  ┌─────────────────────────────────────────────────────┐   │
│  │ Metric      │ JPM   │ GS    │ BAC   │ C     │ WFC   │   │
│  ├─────────────┼───────┼───────┼───────┼───────┼───────┤   │
│  │ Market Cap  │ $580B │ $145B │ $310B │ $120B │ $195B │   │
│  │ P/E Ratio   │ 12.1  │ 14.3  │ 11.8  │  9.5  │ 12.0  │   │
│  │ ROE         │ 15.2% │ 12.8% │ 10.5% │  8.2% │ 11.1% │   │
│  │ Div Yield   │  2.4% │  2.1% │  2.6% │  3.1% │  2.8% │   │
│  │ YTD Return  │ +8.5% │ +6.2% │ +4.1% │ -2.3% │ +5.8% │   │
│  └─────────────────────────────────────────────────────┘   │
│                                                             │
│  RANKING BY ROE                                             │
│  1. JPM  ████████████████████████████████ 15.2%            │
│  2. GS   ██████████████████████████ 12.8%                  │
│  3. WFC  ██████████████████████ 11.1%                      │
│  4. BAC  ████████████████████ 10.5%                        │
│  5. C    ████████████████ 8.2%                             │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Table Formatting Standards

| Element | Format | Example |
|---------|--------|---------|
| Currency (Billions) | $XXX.XB | $125.5B |
| Currency (Millions) | $XXX.XM | $45.2M |
| Percentages | XX.X% | 12.5% |
| Ratios | X.Xx | 1.25x |
| Basis Points | +/-XXbp | +15bp |
| Dates | MMM DD, YYYY | Feb 04, 2026 |

---

## 8. Appendices

### Appendix A: Public Data Sources

| Source | URL | Data Types | API Available |
|--------|-----|------------|---------------|
| **FRED** | fred.stlouisfed.org | Economic data, rates | Yes (free) |
| **SEC EDGAR** | sec.gov/edgar | Company filings | Yes (free) |
| **Yahoo Finance** | finance.yahoo.com | Stock data, financials | Yes (yfinance) |
| **Treasury.gov** | fiscaldata.treasury.gov | Government debt data | Yes (free) |
| **Wikipedia** | wikipedia.org | Company info, lists | Yes (free) |

### Appendix B: Python Libraries Used

```python
# Data fetching
import yfinance as yf          # Stock and financial data
from fredapi import Fred       # FRED economic data

# Data manipulation
import pandas as pd            # DataFrames
import numpy as np             # Numerical operations

# Visualization
import matplotlib.pyplot as plt  # Charts
import plotly.express as px      # Interactive charts

# Web apps
import streamlit as st         # Dashboard apps

# Utilities
from datetime import datetime  # Date handling
import requests                # API calls
```

### Appendix C: Glossary of Treasury Terms

| Term | Definition |
|------|------------|
| **Yield Curve** | Graph showing interest rates across different maturities |
| **Spread** | Difference between two interest rates |
| **NIM** | Net Interest Margin — bank profitability metric |
| **CET1** | Common Equity Tier 1 — bank capital ratio |
| **ROE** | Return on Equity — profitability measure |
| **FCF** | Free Cash Flow — cash after capital expenditures |
| **Debt/EBITDA** | Leverage ratio comparing debt to earnings |

### Appendix D: Windsurf Quick Reference

| Action | How To |
|--------|--------|
| Start Cascade chat | Click Cascade icon or Cmd/Ctrl + L |
| Create new file | Ask: "Create a new file called X.py" |
| Edit existing file | Ask: "Edit line 25 to change X to Y" |
| Run code | Ask: "Run this script" or use terminal |
| Start new session | Click "New Chat" to reset context |
| Use Flows | Click Flows tab → Create New Flow |

---

## 9. Course Completion Checklist

### Module Completion Tracker

| Module | Exercise | Completed | Notes |
|--------|----------|-----------|-------|
| 1 | First PRD.md | ☐ | |
| 2 | Cash Dashboard | ☐ | |
| 3 | Debt Comparison | ☐ | |
| 4 | Peer Widget | ☐ | |
| 5 | Morning Report | ☐ | |
| 6 | Troubleshooting | ☐ | |

### Skills Self-Assessment

Rate yourself 1-5 after completing the course:

| Skill | Before | After |
|-------|--------|-------|
| Using Cascade effectively | ___ | ___ |
| Writing clear prompts | ___ | ___ |
| Building dashboards | ___ | ___ |
| Automating reports | ___ | ___ |
| Troubleshooting AI issues | ___ | ___ |
| Teaching others | ___ | ___ |

---

## 10. Next Steps for Trainers

After completing this course, you are ready to:

1. **Run a pilot session** — Train 2-3 colleagues using this material
2. **Customize exercises** — Adapt to your organization's specific needs
3. **Build a library** — Save successful prompts and templates
4. **Measure ROI** — Track time saved and quality improvements
5. **Scale training** — Roll out to broader Treasury team

---

**Congratulations!** You are now equipped to train others in AI coding assistants for Treasury.

*Questions? Issues? Open an issue on the GitHub repository.*

---

© 2026 | Train the Trainer Program | Public Domain — Free to use and modify
