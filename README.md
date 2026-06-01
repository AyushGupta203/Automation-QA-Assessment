# Automation & QA Developer Assessment

## Candidate

Ayush Gupta

## Task 1 - QA Testing

The Conduit (Real World OSS Project) application was tested using manual functional testing techniques.

### Bugs Identified

* Registration accepts whitespace-only credentials
* Registration accepts invalid email formats
* Article creation accepts whitespace-only content
* Invalid image URLs accepted in profile settings
* Technical validation messages exposed to users
* Missing Forgot Password functionality

Detailed bug reports, screenshots, and root cause analysis are available in the attached PDF report.

---

## Task 2 - Cryptocurrency Price Alert Workflow

### APIs Used

* CoinGecko Simple Price API
* CoinGecko Coin Details API

### Workflow Logic

1. Manual Trigger starts workflow execution.
2. HTTP Request fetches Bitcoin price.
3. IF node validates whether Bitcoin price is greater than 70000 USD.
4. Second HTTP Request retrieves detailed cryptocurrency information.
5. Edit Fields formats the required output.
6. Gmail sends an email notification.

### Transformation

The workflow extracts:

* Cryptocurrency Name
* Symbol
* Current Price
* Alert Status

### Error Handling

Continue On Fail was enabled on HTTP Request nodes to prevent silent workflow failures.

### Output

An email alert is generated whenever the configured threshold condition is satisfied.

---

## Files Included

* Task1,2_QA_Report_Ayush_Gupta.pdf
* Task2_Workflow_AyushGupta.json
