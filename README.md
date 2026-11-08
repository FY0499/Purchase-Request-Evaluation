# Purchase Request Evaluation

An n8n workflow that receives employee purchase requests and uses AI to assess the justification, price reasonableness, priority, and required approval level.

## How it works

1. An employee submits the requested item or service, estimated price, and reason through a form.
2. A Gemini-powered AI agent assesses the request and returns a category, priority, price assessment, and recommended approval level.
3. JavaScript parses and structures the AI result.
4. The request is recorded in Google Sheets with a pending-approval status.
5. The workflow sends an email notification based on the approval path.

## Technologies

- n8n
- Google Gemini / Gemma
- Google Sheets
- Gmail
- JavaScript
- n8n Forms

## Setup

1. Import workflow.json into n8n.
2. Configure Gemini, Google Sheets, and Gmail credentials.
3. Connect your purchase requests sheet and set the approver email address.
4. Review the approval routing and test with sample requests before using it.

## Notes

This repository contains the exported n8n workflow. Configure your own credentials and integrations in n8n before running it.
