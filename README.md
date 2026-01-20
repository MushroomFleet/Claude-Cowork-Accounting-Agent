# Claude Cowork Accounting Agent

An experimental system prompt for [Claude Cowork](https://www.anthropic.com) designed to assist with company accounts analysis using CSV and PDF document processing.

> ⚠️ **EXPERIMENTAL PROJECT** — This repository explores the new Claude Cowork feature. It is provided for evaluation and testing purposes only.

---

## 🚨 Important Disclaimer

**THIS IS NOT A FINANCIAL TOOL**

This project is an experimental prompt template for testing Claude Cowork's document processing capabilities. It should **not** be used for:

- Official company filings
- Tax submissions
- Regulatory compliance
- Audited financial statements
- Any binding financial decisions

Always consult a qualified accountant or financial professional for actual business accounting needs.

---

## Overview

Claude Cowork is Anthropic's new desktop automation tool enabling Claude to work with local files and manage tasks. This repository provides a system prompt that configures Claude as a company accounts analyst, capable of:

- Processing bank statements (CSV) and invoices (PDF)
- Summarizing costs vs revenue for a specified financial year
- Tracking Director Loan Account balances
- Categorizing purchasing and campaign costs
- Flagging missing documentation
- Generating discrepancy reports and action plans

## System Prompt

The core of this project is `cowork_financial_analysis_prompt.md` — a structured system prompt that defines:

| Section | Purpose |
|---------|---------|
| **Role Definition** | Establishes Claude as a financial analysis assistant |
| **Document Processing** | Rules for CSV/PDF extraction and cross-referencing |
| **Analysis Scope** | Revenue, costs, purchasing, campaigns, Director Loans |
| **Output Templates** | Financial summary, documentation audit, action plans |
| **Interaction Protocol** | Step-by-step workflow for document intake |
| **Constraints** | Guardrails to prevent fabrication and ensure transparency |

### Key Features

**Cost & Revenue Analysis**
- Operating expenses, staff costs, professional fees
- Purchasing costs (inventory, equipment, supplies)
- Campaign costs (marketing, advertising, promotional spend)
- Revenue streams and gross/net position calculation

**Director Loan Tracking**
- Opening/closing balances per director
- Funds introduced and withdrawn
- S455 tax implication flags

**Documentation Audit**
- Checklist verification for all required documents
- Missing document flagging
- Unmatched transaction identification

**Action Plan Generation**
- Priority 1: Blocking items (required for filing)
- Priority 2: Important items (material to accuracy)
- Priority 3: Advisory items (best practice)

## Usage

1. Copy the contents of `cowork_financial_analysis_prompt.md`
2. Use as a system prompt or project instructions in Claude Cowork
3. Confirm your accounting period when prompted
4. Upload relevant CSV/PDF financial documents
5. Review the generated analysis and action items

## File Structure

```
├── README.md
└── cowork_financial_analysis_prompt.md
```

## Requirements

- Access to [Claude Cowork](https://www.anthropic.com) (beta)
- Financial documents in CSV or PDF format

## Limitations

- Experimental feature — outputs require verification
- No direct integration with accounting software
- Cannot replace professional financial advice
- Results depend on quality/completeness of uploaded documents

## Contributing

This is an experimental project. Feedback and suggestions are welcome via issues or pull requests.

## License

MIT License — See LICENSE file for details.

---

## 📚 Citation

### Academic Citation

If you use this codebase in your research or project, please cite:

```bibtex
@software{claude_cowork_accounting_agent,
  title = {Claude Cowork Accounting Agent: Experimental system prompt for company accounts analysis},
  author = {Drift Johnson},
  year = {2025},
  url = {https://github.com/MushroomFleet/Claude-Cowork-Accounting-Agent},
  version = {1.0.0}
}
```

### Donate

[![Ko-Fi](https://cdn.ko-fi.com/cdn/kofi3.png?v=3)](https://ko-fi.com/driftjohnson)
