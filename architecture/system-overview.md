# System Architecture Overview

The Service Business Intake Automation system captures client inquiries and converts them into structured intake records using AI-powered analysis and automation workflows.

---

## High-Level Workflow

Inquiry Source  
↓  
Webhook Trigger  
↓  
AI Intake Analysis  
↓  
Lead Database  
↓  
Team Notification

---

## Step 1 — Inquiry Sources

Client inquiries can originate from multiple channels:

- Website contact forms
- Yelp messages
- Google messages
- Email inquiries

Each inquiry contains unstructured text describing a potential client's request.

---

## Step 2 — Webhook Ingestion

A webhook receives the incoming inquiry and sends the message payload into the automation workflow.

The webhook acts as the entry point into the automation system.

---

## Step 3 — AI Intake Analysis

An LLM processes the inquiry message to extract structured details including:

- service requested
- urgency or timeline
- summary of request
- recommended next action

This step converts unstructured text into operational data.

---

## Step 4 — Lead Database

The extracted data is stored in an Airtable database that acts as the intake CRM.

This creates a structured record for every inquiry.

---

## Step 5 — Team Notification

Once a lead record is created, the system sends a Slack alert containing a summary of the inquiry.

This ensures the team can respond quickly to potential clients.
