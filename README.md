# Security and Privacy Risks of AI Agent Skills for Vulnerable Users

Preliminary measurement study of AI agent skill files (instruction files and
tool permissions that tell an AI agent what it can read, run, and send).

## 1. Research question
Do AI agent skills that touch sensitive data (health, finance, location,
children's data) request risky capabilities without any user-protecting safeguards?
Vulnerable users, such as children, older adults, migrants, and survivors of
domestic violence, are the least able to notice or recover from data leakage.

## 2. Approach
- Dataset: 13,016 AI agent skill files.
- Each skill was tagged by sensitive domain (8 domains) and by indirect access to
  personal data (3 types: personal data stores, credentials and accounts, device access).
- Each skill was checked for five risky capabilities: network calls, shell execution,
  broad file access, credential handling, and instruction-injection wording.
- Each skill was checked for safeguard wording, such as confirmation, consent, or privacy.

## 3. Key findings
- 13,016 skill files analyzed.
- 46.7% of all skills show at least one risky capability, and 22% show a risky
  capability with no safeguard wording.
- 32.2% of skills with credential or account access show a risky capability and no
  safeguard wording.
- 28.3% of location-related skills show the same pattern.
- 22.0% of children and education skills show the same pattern.
- Percentages are of the skills in each group. Groups overlap, so they should not be added.

## 4. Files in this repository
- `results_summary.xlsx`: summary tables, charts, and a data dictionary explaining
  every column.
- `figures/`: charts used in the brief.

## 5. Limitations, ethics, and status
- Results are keyword-based estimates of what skill text mentions. They are not
  confirmed vulnerabilities, and many skills are developer documentation.
- Status: ongoing research. 
- Contact: [fiza kanwal], [fizakanwal99@gmail.com]
