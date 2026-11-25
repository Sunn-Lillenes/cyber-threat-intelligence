# Cyber Threat Intelligence — ArcticBank Case Study

An MC102 academic case study following the intelligence lifecycle for a fictional
Norwegian bank, from stakeholder requirements to collection, analysis and feedback.

[Read the submitted case study](reports/cti_case_study.pdf)

## What the project demonstrates

- Stakeholder mapping and intelligence requirements.
- A collection management plan covering internal telemetry and public OSINT sources.
- Indicator processing, correlation and confidence assessment.
- STIX 2.1 representation and MITRE ATT&CK mapping.
- Analysis of competing hypotheses and documentation of intelligence gaps.
- Reporting adapted to technical, operational and strategic stakeholders.

## Portfolio artifacts

| Artifact | Purpose |
| --- | --- |
| [Collection management plan](data/CMP_snapshot.csv) | Sources, coverage, frequency and responsibility |
| [Collection log](data/Collection_Log.csv) | Traceability from questions to collected material |
| [ACH matrix](data/ACH_matrix.csv) | Competing hypotheses and evidence |
| [Illustrative STIX bundle](data/stix_bundle_example.json) | Structured intelligence objects and relationships |

## Scenario scope

ArcticBank is fictional. The TLP labels, internal sources, incident descriptions,
and example identifiers in the submitted report belong to the exam scenario.
Illustrative CVE and IOC entries require independent validation before operational use.
The standalone STIX example uses `example.org` in place of the original example domain.

The repository is a research and reporting case study. It contains structured
artifacts and a PDF report, with no requirement to contact external targets.

## Inspect the artifacts

CSV files can be opened in a spreadsheet editor. The STIX example is JSON.

```bash
python3 -m json.tool data/stix_bundle_example.json
```

JSON parsing checks the file's syntax. Full STIX semantic validation would require
a STIX validator and review of the scenario assumptions.
