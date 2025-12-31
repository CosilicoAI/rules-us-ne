# rules-us-ne

Nebraska tax and benefit rules encoded in Cosilico DSL.

## Structure

```
rules-us-ne/
├── statutes/       # Nebraska Revised Statutes
│   └── 77/         # Chapter 77: Revenue and Taxation
└── regulations/    # Nebraska Administrative Code
    └── 316/        # Title 316: Department of Revenue
```

## Overview

This repository contains machine-readable encodings of Nebraska state tax and benefit law, structured according to the official Nebraska Revised Statutes and Nebraska Administrative Code.

### Statutes

Nebraska Revised Statutes are organized by chapter. Key chapters for tax/benefit rules:

- **Chapter 68**: Public Assistance (SNAP, TANF, Medicaid)
- **Chapter 77**: Revenue and Taxation (income tax, property tax, sales tax)
- **Chapter 79**: Schools (education funding)

### Regulations

Nebraska Administrative Code Title 316 contains Department of Revenue regulations implementing tax statutes.

## Usage

```python
from cosilico import load_rules

# Load Nebraska income tax rules
ne_rules = load_rules("rules-us-ne/statutes/77")
```

## Sources

- [Nebraska Revised Statutes](https://nebraskalegislature.gov/laws/browse-statutes.php)
- [Nebraska Administrative Code](https://www.nebraska.gov/rules-and-regs/)
- [Nebraska Department of Revenue](https://revenue.nebraska.gov/)

## License

The encoded rules are derived from public Nebraska law. See individual files for source citations.
