# AI Customer Support FAQ Agent

An AI-powered customer support automation built with **n8n, OpenAI GPT-4o-mini, and Airtable**. This workflow enables customers to ask questions through a webhook and receive responses based on verified company information stored in Airtable.

## Overview

The AI agent acts as a virtual customer support assistant for MNM. Before answering a customer query, it uses Airtable to search the company's FAQ database and retrieves relevant information.

If the requested information is available, the agent responds using the data retrieved from Airtable. If the information is not available, it informs the customer rather than generating an unsupported answer.

## Key Features

- **AI-Powered Customer Support:** Handles customer questions using OpenAI GPT-4o-mini.
- **Airtable Knowledge Base:** Retrieves company information directly from Airtable.
- **Grounded Responses:** Uses company FAQ data to provide accurate answers.
- **Fallback Handling:** Informs customers when requested information is not available in the knowledge base.
- **Webhook Integration:** Accepts incoming customer queries through an HTTP POST webhook.
- **Automated Responses:** Returns AI-generated answers through the webhook response node.

## Technology Stack

- **n8n:** Workflow automation and orchestration.
- **OpenAI GPT-4o-mini:** AI language model.
- **Airtable:** Company FAQ database and knowledge source.
- **Webhook:** Incoming request handling and integration endpoint.

## Workflow Architecture

1. **Webhook Trigger:** Receives incoming customer questions through an HTTP POST request.
2. **AI Agent:** Processes the customer's latest message and determines the required information.
3. **Airtable Search:** Searches the company FAQ database for relevant information.
4. **OpenAI Chat Model:** Generates a response based on the retrieved information.
5. **Webhook Response:** Returns the final answer to the requesting application.

## Supported FAQ Categories

- Company office hours
- Pricing information
- Refund policies

## Use Cases

- Automated FAQ handling
- Customer support chatbots
- Company information assistants
- Website customer support integrations
- Reducing repetitive customer support inquiries

## Setup Requirements

- An active n8n instance
- OpenAI API credentials
- Airtable account and FAQ database
- Webhook integration with a client application

## Project Type

AI Agent | Customer Support Automation | n8n Workflow

---

**Note:** Configure your own API credentials and Airtable database before activating the workflow. Do not commit API keys, access tokens, or private credentials to GitHub.
