# Train the Trainer: AI Coding Assistants Training for Financial Professionals

A self-paced course that empowers students and financial professionals to become internal champions for AI coding assistants like Windsurf. Once trained, the trainer will be able to pass knowledge and best practices using agentic coding tools to others. 

## 🎯 Course Overview

| Attribute | Detail |
|-----------|--------|
| **Duration** | ~4 hours (self-paced) |
| **Format** | Mixed: conceptual + hands-on exercises |
| **Audience** | Finance leaders / executives who will train others |
| **Data Sources** | Public only (FRED, Yahoo Finance) |

## �️ What You Can Build

By the end of this course, you'll create:
- **Treasury yield dashboards** - Real-time yield curve tracking
- **Peer group analyzers** - Compare banks, tech companies, and financials
- **Automated morning briefings** - Daily Treasury reports
- **Debt analysis tools** - Company debt metrics comparison

## 🎯 The PRD-First Approach

**Why start with a PRD.md?** Planning before coding leads to better results. Here's the workflow:

1. **Chat First** - Discuss your idea with Cascade AI
2. **Build Your PRD.md** - Document requirements, data sources, and success metrics
3. **Implement** - Let Windsurf build from your clear specifications

This approach helps AI assistants understand your goals and deliver exactly what you need.

## 🔑 Setup: Get Your FRED API Key

Many assignments use Federal Reserve Economic Data (FRED). You'll need a free API key:

1. Visit [FRED API Registration](https://fred.stlouisfed.org/docs/api/api_key.html)
2. Click "Request API Key" (requires free account)
3. Copy your API key
4. **Best Practice:** Store it in your project root as `.env`:
   ```bash
   # Create .env file in project root
   FRED_API_KEY=your_api_key_here
   ```
5. Add `.env` to your `.gitignore` (never commit API keys!)

## 📝 Assignments

Complete these hands-on exercises to master AI-assisted Treasury development:

### Assignment 1: Treasury Cash Forecasting PRD

**Objective:** Create a PRD for a Treasury cash forecasting tool

**Prompt to use in Cascade:**
```
Create a folder called "Assignment1_CashForecasting" and inside it create a file called "PRD.md" for a Treasury cash forecasting tool that uses only public APIs like FRED and Yahoo Finance. Include sections for Executive Summary, Requirements, Data Sources, and Success Metrics.
```

**What you'll learn:** PRD structure, data source planning, requirement specification

---

### Assignment 2: Treasury Yield Dashboard

**Objective:** Build a live dashboard showing Treasury yields and spreads

**Prompt to use in Cascade:**
```
Create a folder called "Assignment2_YieldDashboard" and build a Python dashboard that:
1. Fetches 10-year and 2-year Treasury yields from FRED (series: DGS10, DGS2)
2. Calculates the yield curve spread
3. Displays a 12-month chart with current values
4. Uses the FRED_API_KEY from the .env file in the root directory

Make it visually clean and save all files in the Assignment2_YieldDashboard folder.
```

**What you'll learn:** API integration, data visualization, environment variables

---

### Assignment 3: Bank Peer Comparison Tool

**Objective:** Compare major banks on key financial metrics

**Prompt to use in Cascade:**
```
Create a folder called "Assignment3_BankComparison" and build a Streamlit app that compares JPM, GS, BAC, C, and WFC on Market Cap, ROE, P/E, and Dividend Yield using yfinance. Include a bar chart and CSV export. Save all code and requirements in the Assignment3_BankComparison folder.
```

**What you'll learn:** Multi-company analysis, interactive dashboards, data export

---

## 🚀 Quick Start

### View the Interactive Course

Simply open `index.html` in your browser - no server needed!

Or use a local server:
```bash
# Start local server
python -m http.server 8080

# Open http://localhost:8080 in your browser
```

### Interactive Features

- ✅ Progress tracker (saves locally)
- ✅ Copy-to-clipboard prompts
- ✅ Interactive tutorial: Build Your First PRD
- ✅ Cascade simulator for practice
- ✅ Prompt analyzer playground
- ✅ Knowledge quizzes

## 📁 Files

| File | Description |
|------|-------------|
| `PRD.md` | Full course content and exercises |
| `index.html` | Interactive web tutorial |
| `images/` | Dashboard mockups and screenshots |

## 🎓 Learning Outcomes

By completing this course, participants will:

- Navigate Windsurf (Cascade & Flows)
- Build PRD.md files using AI assistance
- Create Treasury dashboards with public data
- Automate reports and workflows
- Troubleshoot effectively (iterate vs restart)
- Train colleagues with confidence

## 📊 Sample Outputs

The course teaches you to build:

- Treasury yield dashboards
- Peer group comparison widgets
- Automated morning briefings
- Debt analysis reports

## 🔗 Resources

- [FRED API](https://fred.stlouisfed.org/) - Treasury yield data
- [Yahoo Finance](https://finance.yahoo.com/) - Stock and market data
- [Windsurf](https://codeium.com/windsurf) - AI coding assistant

## 📄 License

Public Domain - Free to use and modify 

---

*Created as part of the Train the Trainer program for Treasury AI adoption*
