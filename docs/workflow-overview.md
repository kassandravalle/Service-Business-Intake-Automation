# Workflow Overview

The Service Business Intake Automation workflow captures and processes client inquiries automatically.

---

## Workflow Steps

1. A client submits an inquiry through a website form or messaging platform.

2. A webhook trigger captures the inquiry and sends the message to the automation workflow.

3. The message is analyzed by an LLM to extract service requests, urgency, and a short summary.

4. The extracted information is written to an Airtable database as a structured lead record.

5. The system sends a Slack alert to notify the team of the new inquiry.

---

## Operational Benefits

- Faster responses to client inquiries
- Centralized intake records
- Reduced manual intake work
- Organized lead management
