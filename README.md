# Airport City Population Pipeline

An Alteryx workflow designed to match airport records with city and population data through cleaning, standardization, validation, and join logic.

---

# Project Overview

Inspired from a real task I got from a company, this project focuses on building a clean and structured data preparation pipeline in Alteryx, capable of:

- matching airport records with city and population datasets
- handling unmatched records separately
- standardizing inconsistent location naming
- extracting and structuring latitude and longitude information
- improving final dataset readability and usability

The workflow separates matched and unmatched outputs in order to support both successful integrations and further manual validation.

---

# Workflow Overview

## Full Workflow

![Workflow Overview](screenshots/workflow_overview.png)

---

# Join and Matching Logic

![Join Logic](screenshots/join_logic_section.png)

---

# Output Examples

## Matched Output

![Matched Output](screenshots/matched_output_preview.png)

## Unmatched Output

![Unmatched Output](screenshots/unmatched_output_preview.png)

---

# Repository Structure

```text
airport-city-population-pipeline
│
├── data
│   ├── sample_input
│   └── sample_output
│
├── workflow
│   └── airport_city_population_match.yxmd
│
├── screenshots
│
└── README.md
```

---

# Workflow Process

The workflow follows these main steps:

1. Import airport and city datasets
2. Clean and standardize location fields, in order to create keys for the matching
3. Normalize naming inconsistencies
4. Extract latitude and longitude information
5. Join airport records with city information
6. Separate matched and unmatched results, and count them
7. Export structured final datasets

---

# Sample Files Included

The repository includes small sample datasets and outputs to demonstrate the workflow logic without requiring large raw datasets nor giving out datasets provided to me by the company.

Included:
- sample airport input data
- sample city input data
- sample matched output
- sample unmatched output

---

# Tools Used

- Alteryx Designer
- Join Tool
- Formula Tool
- Select Tool
- Data Cleansing Tool
- Output Data Tool

---

# Purpose

This project is inspired by a real-world task given to me by a European company active in the field of Aviation Financial Data Analysis. I built as a portfolio-ready data preparation and reconciliation workflow demonstrating practical data cleaning, transformation, matching, and validation techniques using Alteryx.
