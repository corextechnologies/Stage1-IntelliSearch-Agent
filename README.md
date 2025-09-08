IntelliSearch Agent

IntelliSearch Agent is an AI-powered automation workflow built with n8n
.
It leverages OpenAI (GPT-4.1), memory, and a browser automation toolkit (Airtop) to perform autonomous web interactions, extract information, and respond intelligently to chat-based inputs.

🚀 Features

Chat-triggered automation → Starts when a chat message is received.

AI-powered reasoning → Uses GPT-4.1 with memory for context-aware actions.

Browser automation → Create and control browsing sessions with Airtop tools:

Start/terminate browser sessions

Load URLs

Type into input fields

Click elements

Query/extract data from pages

Reflection ability → Includes a "Think" step for planning before actions.

Structured workflow in n8n → Fully modular and extendable.

🛠️ Components

Trigger:

When chat message received → Activates workflow on new chat input.

AI Core:

OpenAI Chat Model (GPT-4.1) → Powers decision-making and natural language understanding.

Simple Memory → Maintains conversation context.

AI Agent → Orchestrates tools and system prompts.

Browser Tools (via Airtop):

createbrowser → Starts a browser session.

typing tool → Types into input fields (e.g., search bars).

clicking tool → Clicks buttons or elements.

Load a page in Airtop → Navigates to a URL.

Query tool → Extracts structured info from web pages.

Terminate a session in Airtop → Closes the browser session.

Utility:

Think → Used by the agent for internal reasoning before next steps.

⚙️ Setup

Clone or import the workflow into your n8n instance.

Configure the following credentials:

OpenAI API key (for GPT-4.1).

Airtop API credentials (for browser automation).

Adjust workflow IDs (e.g., create browser) if needed.

Save and activate the workflow.

📌 Usage

Send a chat message (the workflow trigger).

The agent will:

Interpret the request

Decide on a browsing strategy

Open a session and navigate accordingly

Interact with the web page (type, click, query)

Return the extracted results

Properly terminate the session

🔒 Notes & Best Practices

Always ensure the session is terminated (Terminate a session in Airtop) to avoid resource leaks.

Use descriptive element selectors/placeholders for typing/clicking tools.

Extend the workflow by adding more n8n tools if needed (APIs, storage, notifications).

📄 License

This project is licensed under the MIT License.
