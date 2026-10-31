<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=25&pause=900&color=2563EB&center=true&vCenter=true&width=880&height=64&lines=Arpita+Tiwari;Finance+Analyst+%C2%B7+FP%26A+and+record+to+report;I+build+the+tooling+for+the+work+I+do+by+hand;rules+first%2C+a+model+only+where+it+belongs" alt="Arpita Tiwari" />

<p>
<a href="https://www.linkedin.com/in/arpita-tiwari-5b955a307"><img src="https://img.shields.io/badge/FP%26A-record__to__report-2563EB?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0F172A" alt="FP&A" /></a>
<img src="https://img.shields.io/badge/Bengaluru-open__from__16__Nov__2026-16A34A?style=for-the-badge&labelColor=0F172A" alt="Availability" />
<img src="https://komarev.com/ghpvc/?username=arpita-at&style=for-the-badge&color=2563EB&labelColor=0F172A&label=profile+views" alt="views" />
</p>

</div>

---

I am a **Finance Analyst** at a global shared services centre in Bengaluru. Month-end
close, balance sheet reconciliations, budget versus actual, and the commentary that
goes with it.

I also write the tooling for the parts of that job I kept doing by hand. Not because
automation is interesting, but because the fourth time you reconcile the same file the
same way, it stops being analysis.

```text
  by day ──►  record to report      close, reconciliations, accruals, intercompany
              FP&A                  budget vs actual, flux and variance commentary
              systems               SAP (FB03, FAGLL03, FS10N), Ariba, TM1, Excel

  by night ─► finance agents        deterministic rules, a model only for ambiguity
              controls              audit trail on every decision, human approval gate
              stack                 Python, FastAPI, pandas, pytest, Anthropic
```

### What I believe about AI in finance

Most of it aims at the wrong bottleneck. Close is not slow because the arithmetic is
hard. It is slow because data arrives late, nobody owns the cost line, and the answer
lives in the head of someone on leave. Those are structural problems, not compute
problems.

So everything here follows the same shape:

| | |
|---|---|
| **Rules** | Matching, totalling, thresholds, FX, anything that must tie to the penny |
| **Model** | Naming a cause, classifying an exception, drafting a sentence |
| **Human** | Signing. That does not move to software |

If it must tie exactly, it is a rule. You can regression test a rule. You cannot
regression test a vibe.

### Finance tooling

| Repo | What it does |
|---|---|
| **[margin-model](https://github.com/arpita-at/margin-model)** | Overhead absorption and product profitability. Allocates one pool two ways, a plantwide machine-hour rate and activity-based driver rates, and reports which products change sign. On the sample all six look profitable under the blanket rate; two, carrying 12.2% of revenue, are loss-making under the drivers. Splits over and under absorption into expenditure and volume variance. Excel workbook with live formulas |
| **[flux-agent](https://github.com/arpita-at/flux-agent)** | Month-end flux commentary. Deterministic variance, materiality and evidence retrieval; a model drafts the sentence, and only from postings it was handed. A line with no evidence comes back as a gap, never a guess |
| **[grir-agent](https://github.com/arpita-at/grir-agent)** | GR/IR open item triage for SAP. Groups every posting by PO line, nets it, names the mechanical cause and sizes the exposure. On the sample 45% of the aged account already balances and carries no exposure at all |
| **[dupe-agent](https://github.com/arpita-at/dupe-agent)** | Duplicate supplier payments the ERP's own check never sees. Normalises invoice numbers and vendor names, scores six near-duplicate patterns, and asks a model one question only: is there an innocent explanation |
| **[reconcile-studio](https://github.com/arpita-at/reconcile-studio)** | Settlement reconciliation. Match a gateway file against the ledger, label every discrepancy, report a match rate with an audit trail |
| **[reconcile](https://github.com/arpita-at/reconcile)** | The gateway-agnostic engine underneath. Deterministic matcher plus a Claude agent for the fuzzy cases |
| **[dispute-agent](https://github.com/arpita-at/dispute-agent)** | Chargebacks. Triages by reason code, lists the missing evidence, drafts the representment |
| **[risk-triage](https://github.com/arpita-at/risk-triage)** | Transaction risk scoring. Deterministic engine, Claude only on the borderline cases. Advisory only |

### Stack

<p>
<img src="https://img.shields.io/badge/Excel-0F172A?style=for-the-badge&logo=microsoftexcel&logoColor=16A34A" alt="Excel" />
<img src="https://img.shields.io/badge/SAP-0F172A?style=for-the-badge&logo=sap&logoColor=2563EB" alt="SAP" />
<img src="https://img.shields.io/badge/Python-0F172A?style=for-the-badge&logo=python&logoColor=2563EB" alt="Python" />
<img src="https://img.shields.io/badge/pandas-0F172A?style=for-the-badge&logo=pandas&logoColor=2563EB" alt="pandas" />
<img src="https://img.shields.io/badge/FastAPI-0F172A?style=for-the-badge&logo=fastapi&logoColor=2563EB" alt="FastAPI" />
<img src="https://img.shields.io/badge/pytest-0F172A?style=for-the-badge&logo=pytest&logoColor=2563EB" alt="pytest" />
<img src="https://img.shields.io/badge/Anthropic-0F172A?style=for-the-badge&logo=anthropic&logoColor=7C3AED" alt="Anthropic" />
</p>

### Still learning

Consolidation across many entities at scale. Statutory and audit workflow end to end.
Power BI beyond the basics.

Costing is the honest caveat on margin-model: I have built the allocation and the
absorption variance and I can defend every formula in it, but I have not yet run
product costing inside a live ERP. CO-PA, standard cost rolls and the month-end
revaluation are next. I would rather write that here than guess in an interview.

### Reach me

Open to **Finance Analyst, FP&A Analyst and R2R Analyst** roles in Bengaluru or hybrid,
available from **16 November 2026**.

[LinkedIn](https://www.linkedin.com/in/arpita-tiwari-5b955a307) · sktarpita@gmail.com ·
or open an issue on any repo and tell me where the logic breaks.
