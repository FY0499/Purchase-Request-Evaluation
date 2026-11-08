# Purchase Request Evaluation

I built this n8n workflow to evaluate employee purchase requests using AI, review the reason and estimated price, and identify the approval level required for each request.

<img width="726" height="247" alt="image" src="https://github.com/user-attachments/assets/d141855a-a3c1-464e-90ab-01980b8dbe36" />

## How it works

1. An employee submits their name, email, requested item or service, estimated price, and reason through a form.
2. The AI agent evaluates the request based on the justification, price reasonableness, and priority.
3. The AI also identifies whether the request requires approval from a direct manager or the financial manager.
4. JavaScript processes the result and the request is saved to Google Sheets with a Pending Approval status.
5. The workflow sends an email notification according to the approval path.

## Main features

- Employee purchase request form.
- AI assessment of the request and price.
- Priority classification.
- Recommended approval level.
- Google Sheets request tracking and email notifications.

## Technologies

n8n, Google Gemini, Google Sheets, Gmail, JavaScript, AI Agent, and n8n Forms.

## Setup

Import [workflow.json](./workflow.json) into n8n, configure your Gemini, Google Sheets, and Gmail credentials, then connect your purchase request sheet and review the approver email address before testing.
