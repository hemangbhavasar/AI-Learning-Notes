---
title: >-
  Model Context Protocol (MCP) Explained for Beginners: AI Flight Booking Demo!
  - YouTube
description: >-
  🆓Access to MCP Lab: https://kode.wiki/3IxxdBGCurious about how AI agents
  function and their impact on technology? 🤖✨ In this video, we explore AI
  agents an...
author: YouTube
source: https://www.youtube.com/watch?v=E2DEHOEbzks&ab_channel=KodeKloud
created: "2025-08-19"
tags:
  - web-notes
  - hover-notes
  - webpage
---

### Introduction to AI Agents and Model Context Protocol (MCP)
- Goal: To explain these concepts using visualizations for easy understanding.
- No prior AI, coding, or programming knowledge needed.
- Part 1: Explain the "why" and "what" behind the concepts.
- Part 2: Dive into code to understand the "how" of implementation.
- Access to a hands-on lab for practice.
### What is ChatGPT?
- Two components:
- A chat application.
- A GPT (Generative Pre-trained Transformer) model.
- The chat part is simply an application.
- The **GPT part** is the *Large Language Model (LLM)*, which is the AI component.
- Other examples of LLMs include:
    - Claude (from Anthropic)
    - DeepSeek
    - Gemini
    - Llama
- **How ChatGPT works:**

    1.  User asks a question in the ChatGPT application.
    2.  The application sends a *request* to the LLM (GPT).
    3.  The LLM processes the request.
- After the LLM processes the request, it sends a response back to the application, which displays the results.
- Let's say we're building an application called FlyGPT, similar to ChatGPT, that books flights.
- User asks: "I would like to fly to North London."
- Ideally, it should book a flight.
- We need something that the application can interact with, that understands the request and does as I say.
- That 'magical thing' is AI in the form of an LLM.
- The response is just instructions in the form of text. It doesn't actually book the flight.
### LLMs and Taking Action
- LLMs can generate responses in the form of text, pictures, or videos.
- **Limitations:** LLMs cannot, by themselves, take actions.
- **Example of taking action:**
    - Interacting with third-party flight services like Joyair, DracAir, or AeroGo.
    - Retrieving flight details.
    - Comparing flight options against user preferences (cheap vs. luxury, seat preferences, meals).
### AI Agents
- AI agents can interact with third-party platforms or websites.
- They gather information and combine it with memory from previous conversations.
- They interact with an LLM (which is the real AI) to make decisions.
- AI agents enable goal-driven behavior.
### AI Agents (continued)
- An AI agent acts as an intermediary, interacting with:
    - **Third-party tools/services** (like flight booking sites: Joyair, DracAir, AeroGo).
    - Its **own memory** (from previous conversations/tasks).
    - An **LLM** (the core AI for decision-making).
- This interaction is a continuous loop: the agent goes back and forth, gathering information, making decisions, and taking actions until a goal is achieved (e.g., booking a flight).
- Agents enable true *goal-driven behavior* by translating LLM responses into executable actions.
### AI Agents in Everyday Tools
- Many modern *Integrated Development Environments (IDEs)* are starting to function as AI agents.
- Examples include:
    - Cursor
    - Warp
    - VS Code (with extensions like GitHub Copilot)
- These IDEs have an "agent mode" that allows them to interact with tools and execute tasks, not just provide code suggestions.
- **Agent vs. Non-Agent Era:**
    - **Non-Agent Era:** If you asked a question, an LLM would just *give you a response* (e.g., text, code snippet).
    - **Agent Era:** An agent can *take action* based on that response, like modifying code, running tests, or performing system operations, without you needing to manually execute each step. It works to *complete* the task.
### AI Agents vs. Chatbots
- **AI Agent:**
    - Can be given a big task (e.g., build an entire app or troubleshoot an issue).
    - Goes through a sequence of multiple AI calls.
    - Interacts with the codebase and the terminal (if needed).
    - Doesn't stop until the task is completed.
- **Chatbot:**
    - Calls a single LLM.
### Real-World Use Cases: Troubleshooting
- Software development is a key area.
- Example: "We recently noticed that a button was missing on the UI. Help me identify when and how this changed and share a plan to revert."
    - An AI agent can help with this type of task by checking:
        - Git changes.
        - Backend code.
        - Frontend code.
### Real-World Use Cases: Troubleshooting (continued)
- AI agents can scan through codebases, including:
    - Frontend code.
    - Backend code.
    - Git history.
- Agents can identify the specific commit that caused a change and suggest how to revert or fix it.
### Getting Started with AI Agents
- **Pre-built Agents:**
    - Platforms like [agents.ai](https://agents.ai) offer pre-built agents.
    - These agents can perform various tasks, such as video script generation or web design grading.
    - They can be integrated into applications by invoking them remotely.
- **Building Your Own Agents:**
    - Tools like n8n allow you to build your own agents without coding.
    - n8n provides the capability to...
### Building Your Own Agents
- **n8n (No Code):**
    - Allows drag-and-drop agent creation.
    - Offers example workflows for tasks like:
        - Generating AI videos for YouTube.
        - Intelligent email organization with AI-powered content classification.
- **LangChain and LangGraph:**
    - Platforms for building agents from scratch with code.
    - Full courses available for in-depth learning.
### Agent Interaction with Third-Party Platforms
- Agents interact with third-party platforms through **tools**.
### Agent Interaction with Airlines
- Agents use **tools** to interact with third-party platforms (e.g., airlines).
- The video uses airline booking as an example.
- **Human User Interaction (without agents):**
    - A user goes to an airline's website (e.g., emirates.com).
    - The website returns a webpage.
    - The user clicks around to find a flight according to their preferences and books the flight.
### Agent Interaction with Airlines (continued)
- **User Interface (UI):**
    - The airline's website or mobile app (e.g., emirates.com).
    - Used by human users to search and book flights.
- **Application Interaction (without agents):**
    - Third-party websites (e.g., MakeMyTrip, Booking.com, Cheapflights) interact with airline websites.
    - In the past, these applications would *scrape* the airline websites.
        - Scraping means saving the website as a text file (HTML).
        - Complex algorithms were used to extract flight details from the scraped HTML.
### APIs (Application Programming Interfaces)
- Airlines realized it's beneficial to be on third-party platforms.
- Airlines provide an API, so third-party platforms can access flight information in a structured format.
- Example: `emirates.com/api/flights` returns flight details in JSON format, so applications don't have to scrape the website.
- An API lets other applications *retrieve* flight details.
- An API can also *book* flights. Example: `emirates.com/api/book-flights?flightNumber=EK502`.
### APIs (Application Programming Interfaces) (continued)
- **User Interface (UI)**: What a human user interacts with (e.g., a website).
- **Application Programming Interface (API)**: What an application interacts with.
-  Airlines use APIs so third-party platforms can access flight information in a structured format.
### Agent Interaction with Third-Party Platforms (via APIs)
- Tools interact with airlines through APIs.
- Each tool is a piece of code that interacts with an API.
### Agent Interaction with Third-Party Platforms (via APIs) (continued)
- Tools interact with APIs of airlines to retrieve flight information.
- This information is shared with LLMs for decision-making.
- The agent uses tools again to make another API call to book the flight on the respective airline.
- Example API calls:
    - `curl [https://www.joyair.com/api/flights](https://www.joyair.com/api/flights)`
    - `curl [https://www.dracair.com/api/flights-list](https://www.dracair.com/api/flights-list)`
    - `curl [https://www.aerogo.com/api/list-flights](https://www.aerogo.com/api/list-flights)`
- Each API call is different, and so are the responses.
### The Problem with Diverse APIs
- Each airline (and other third-party services) has its *own standard* for their APIs.
- **Example:**
    - Joyair's API returns flight information with keys like `flightNumber`, `origin`, `destination`.
    - DracAir's API uses `flightNum`, `from`, `to`.
    - AeroGo's API uses `detail-flights`, `start`, `finish`.
- There are hundreds of airlines and millions of other third-party sites.
- **Challenge:** If an application needs to interact with all of them, writing specific "adapter codes" for each unique API standard is inefficient and time-consuming.
- **AI Solution:** In the AI world, we want AI to handle this complexity directly, eliminating the need for developers to write endless custom integration code.
### Model Context Protocol (MCP)
- MCP acts as a guide for AIs to choose the right APIs and interact with third-party platforms.
- MCP provides agents the context needed to make the right API calls.
- Example: MCP tells the agent that Joyair has `searchFlights` and `bookFlight` capabilities.
- MCP also provides the input structure and output structure that are needed to interact with Joyair.
### Model Context Protocol (MCP) (continued)
- MCP was introduced by Anthropic and has since been open-sourced.
- It's now a default standard for building AI agents.
- MCP servers can be found for many applications at [https://github.com/modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers)
- Every agent has an MCP configuration file named `mcp.conf`.
- The `mcp.conf` file specifies:
    - The name of the MCP (e.g., MongoDB).
    - The command and arguments associated with running the MCP server (e.g., MongoDB's connection string).
### Model Context Protocol (MCP) Configuration
- Each agent has an `mcp.conf` file.
    - Specifies the name of the MCP (e.g., MongoDB).
    - Includes the command and arguments to run the MCP server (e.g., MongoDB's connection string).
- The location of the `mcp.conf` file depends on the tool being used.
    - Cursor: `~/.cursor/mcp.js`
    - Windsurf: `~/.codeium/windsurf/mcp_config.json`
    - Claude: `/Library/Application Support/Claude/claude_desktop_config.json`
### MCP Server
- MCP server works in a *client-server model*.
- Instead of interacting with the API directly, the agent interacts with the MCP server.
### MCP Client and Servers
- The agent interacts with MCP servers through an MCP client.
### Expanding Agent Capabilities
- Current agent can only book flights.
- To expand the agent's capabilities to include booking hotels, more MCP servers can be added to connect to hotel booking services (e.g., Marriott, Holiday Inn, Accor).
### Expanding Agent Capabilities
- Instead of one agent handling everything, it's better to have specialized agents for specific tasks, like:
    - A **Flight Agent** for finding and booking flights.
    - A **Hotel Agent** for finding and booking hotels.
- Each specialized agent should:
    - Be excellent at its specific task.
    - Have its own integration with relevant MCP servers.
    - Maintain its own memory and preferences (e.g., flight preferences vs. hotel preferences like amenities, bed type, check-in/out).
- Agents can call other agents (e.g., the Flight Agent could call the Hotel Agent) to complete a multi-faceted task. This is an **agent-to-agent call**.
### Agent2Agent Protocol (A2A)
- Addresses how agents communicate and understand each other's capabilities.
- Developed by Google to enable collaboration in a multi-agent ecosystem.
- Allows agents to discover the capabilities of other agents.
- Example: Flight agent asks hotel agent, "What can you do?"
- Hotel agent responds: "I can search and book hotels."
- **Agent2Agent (A2A) Protocol:**
    - Defines standards for agents to discover each other's capabilities.
    - Defines standards to assign tasks to other agents and check their status.
    - Defines standards for how agents communicate.
    - Defines how context and results are shared between agents.
### Real-World Use Cases: Backend Development
- AI agents and MCPs are used to build backend applications.
- AI agents can identify the specific commit that caused a change.
- APIs are developed using AI agents and MCP.
### Real-World Use Cases: Backend Development (continued)
- AI Agents can test APIs during development.
- They can also ensure data is available in MongoDB.
### Real-World Use Cases: Data Engineering
- Agents use SQL queries and MCP to interact with:
    - Stripe
    - Google BigQuery
    - Metabase
- Example Prompt: "We seem to be missing invoice details from stripe records. Identify when this started and provide a fix please."
### Real-World Use Cases: Data Engineering
- **Example Scenario:** Missing invoice details from Stripe records.
- **Agent's Task:** Identify when the issue started and provide a fix.
- **Agent's Action:** The AI agent was given access to Stripe, Google BigQuery, and Metabase through MCP servers.
- It performed a 5-10 minute troubleshooting process.
- **Agent's Output (Example):**
    - Identified a specific transaction ID, date, amount, status, product type (`KODEKLOUD STANDARD`), and interval (`year`).
    - **Conclusion:** The product details were correctly retrieved, and the charge was for KodeKloud STANDARD (type: standard) with a yearly interval.
    - **Key Fix:** Always join invoices using both `charges.invoice_id = invoices.id` and `invoices.charge_id = charges.id` to catch all cases.
    - Suggested updating main queries to include this logic or checking for more charges.
- This demonstrates how AI agents with MCP can troubleshoot and resolve complex data issues across multiple platforms.