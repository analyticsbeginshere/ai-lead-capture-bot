# AI Lead Capture & Qualification Bot

An n8n workflow that takes leads from a Google Form, classifies them as hot or cold using AI, stores them in Airtable, and sends instant Telegram alerts for hot leads.

## How it works
1. Lead fills Google Form, which saves to Google Sheets
2. n8n picks up each new row automatically
3. AI Agent (OpenAI) classifies the lead as hot or cold and returns structured JSON
4. IF node routes hot and cold leads to different paths
5. Hot leads trigger an instant Telegram alert, then are saved to Airtable
6. Cold leads are saved to Airtable without an alert

## Tools Used
- n8n
- OpenAI
- Google Forms and Google Sheets
- Airtable
- Telegram Bot API

## Screenshots
See the `Screenshots` folder for the form, sheet, workflow canvas, AI output, Telegram alert and Airtable.
