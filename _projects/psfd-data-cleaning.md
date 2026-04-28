---
layout: project
title: "Panel Study of Family Dynamics Data Harmonization"
category: "Data Engineering"
summary: "Building a consistent 2006–2024 panel from complex PSFD follow-up and initial-visit questionnaires."
---

## Project Overview

This project harmonizes Taiwan's Panel Study of Family Dynamics data across multiple waves and questionnaire types. The goal is to create a unified panel with consistent variable names, comparable marital-status categories, spouse information, education variables, and derived indicators.

## Core Challenge

The survey design skips questions that have already been asked in previous waves. As a result, spouse or cohabiting-partner information can be missing in later waves even when the partner is the same person. The project therefore requires logic for identifying same-spouse or same-partner status and carrying forward valid information.

## Methods

- Standardized yearly data with a `make_year(df, year, cfg)` workflow.
- Built year-specific recoding rules for marriage, cohabitation, education, income, working hours, and occupation.
- Designed imputation logic for respondent and spouse education.
- Audited missing values before and after filling.

## Tools

R, haven, dplyr, tidyr, purrr, plm.
