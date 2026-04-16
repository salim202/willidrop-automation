# Willidrop Transport Order Automation

Automated email workflow that reads confirmed transport orders 
from Airtable and sends professional confirmation emails to carriers.

## Stack
- n8n (workflow automation)
- Airtable (data source)
- Gmail (email delivery)
- Ollama (local LLM)

## How it works
1. Reads confirmed orders from Airtable
2. Filters only uncontacted carriers
3. generate a formatted HTML confirmation email with the LLM
4. Sends formatted HTML confirmation email
5. Updates Airtable status to "sent"
