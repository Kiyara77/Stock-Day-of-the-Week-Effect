# Stock-Day-of-the-Week-Effect
# Empirical Study on the Day-of-the-Week Effect in China's A-Share Market  
### —— Evidence from the SSE Composite Index and SPDB

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

This repository contains the empirical analysis and supporting code for a study examining the **day-of-the-week effect** in China’s A-share stock market, using the **SSE Composite Index** and **Shanghai Pudong Development Bank (SPDB, 600000.SH)** as case studies.

## 📌 Overview

The "day-of-the-week effect" is a well-known calendar anomaly in financial markets, where asset returns exhibit systematic differences across weekdays. In Western markets, a notable "Monday effect" (negative average returns on Mondays) has been widely documented. This project investigates whether such an effect persists in the Chinese A-share market during the sample period **November 27, 2025 – March 25, 2026**.

Key findings:
- The SSE Index shows a negative average return on Mondays but positive returns on other weekdays—suggesting a superficial "Monday effect".
- SPDB exhibits higher average returns on Wednesdays ("mid-week effect").
- However, **one-way ANOVA tests show no statistically significant differences** in mean returns across weekdays for either asset (p > 0.05).
- Visual analysis (boxplots) reveals that extreme outliers—especially for SPDB on Wednesday—influence the mean but do not constitute a robust, exploitable pattern.

These results suggest that the Chinese A-share market has become increasingly efficient, and simple calendar-based trading strategies are unlikely to yield consistent excess returns.

## 📂 Repository Structure
