---
id: 23a7a0d8-1548-4967-8423-14e94f0376c8
type: skill
title: Finance Domain Pedagogy
tags:
  - domain-pedagogy
  - finance
  - blocks
  - lyceum-core
references: []
created: '2026-03-03'
updated: '2026-03-03'
---
FINANCE-SPECIFIC BLOCKS (use these for investing/finance/trading courses):

- stock-simulator: A stock purchase card showing a real company, price, mini chart, and share selector. Learner picks how many shares and taps Buy. Uses real company names and realistic prices.
  { "type": "stock-simulator", "company": "Apple Inc.", "ticker": "AAPL", "price": 178.52, "change": "+2.34 (1.3%)", "changePositive": true, "shareOptions": [1, 5, 10, 25], "instruction": "Your first investment. Pick how many shares to buy.", "successMessage": "You just bought {n} shares of Apple. You're an investor." }

- fund-card: An ETF/fund analysis card with tappable metrics. Learner reveals each metric to understand what makes a good fund, then decides whether to invest.
  { "type": "fund-card", "fundName": "Vanguard FTSE All-World UCITS ETF", "ticker": "VWCE", "isin": "IE00BK5BQT80", "metrics": [{"label": "Expense Ratio (TER)", "value": "0.22%", "good": true, "tip": "Below 0.5% is great for a passive ETF."}, {"label": "Assets Under Management", "value": "$12.4B", "good": true, "tip": "Large AUM means the fund is liquid and well-established."}, {"label": "Diversification", "value": "3,700+ stocks", "good": true, "tip": "More holdings = more diversification = less risk from any single company."}, {"label": "Tracking Error", "value": "0.15%", "good": true, "tip": "Low tracking error means the fund closely follows its index."}], "instruction": "Tap each metric to learn what it means.", "successMessage": "You just evaluated a real ETF like an investor. These metrics help you compare funds." }

- spreadsheet-formula: Use this for financial calculations — budgeting, compound interest, portfolio allocation. The Excel-style grid makes financial math tangible.
  { "type": "spreadsheet-formula", "fileName": "Portfolio.xlsx", "cells": [{"label": "Stocks", "value": "$6,000"}, {"label": "Bonds", "value": "$3,000"}, {"label": "Cash", "value": "$1,000"}], "resultLabel": "Total", "formulaOptions": [{"formula": "SUM", "result": "$10,000", "correct": true, "explanation": "SUM adds up all your holdings to show your total portfolio value."}], "instruction": "What's the total value of this portfolio?" }

FIRST-TOUCH SEQUENCE FOR INVESTING (Beginner, Module 1, Blocks 1-3):
  Block 1: stock-simulator — buy shares of a well-known company (Apple, Tesla, etc.)
  Block 2: fund-card — evaluate a simple ETF with 3-4 metrics
  Block 3: quick-quiz — "What did buying a share actually give you?" (tests comprehension)

FIRST-TOUCH SEQUENCE FOR INVESTING (Intermediate, Module 1, Blocks 1-3):
  Block 1: fund-card — evaluate an ETF with 5 metrics including TER, AUM, replication
  Block 2: stock-simulator — compare buying individual stock vs ETF cost
  Block 3: fill-in-blank — "An ETF with a TER of {{0}} means you pay that percentage annually"

FIRST-TOUCH SEQUENCE FOR INVESTING (Advanced, Module 1, Blocks 1-3):
  Block 1: fund-card — evaluate a complex ETF with 5-6 metrics (synthetic replication, securities lending, tracking difference)
  Block 2: spreadsheet-formula — calculate portfolio allocation percentages
  Block 3: claim-judge — challenge a common advanced investing myth

TIER AWARENESS: Adjust content complexity to match the module's position in the course.
  Beginner: simple stock purchases, basic fund metrics (TER, diversification), one-concept interactions.
  Intermediate: compound concepts (comparing stocks vs ETFs), comparison tasks, multiple metrics.
  Advanced: real-world scenario evaluation (synthetic vs physical replication, tax-loss harvesting), portfolio construction.

IMPORTANT: Finance lessons should be at least 50% interactive. The learner should FEEL like an investor from block 1 — buying stocks, evaluating funds, making decisions. Use real company names and realistic prices. Never give actual financial advice — frame everything as educational simulation.
