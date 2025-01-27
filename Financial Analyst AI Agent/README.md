# Financial Analyst AI Agent

## Overview

The **Financial Analyst AI Agent** is a sophisticated AI system designed to assist in financial analysis by leveraging advanced models and toolkits. This agent is capable of retrieving real-time financial data, summarizing analyst recommendations, and providing insights through a user-friendly interface. It uses the **PhiData** library for Agentic AI, which simplifies the integration and orchestration of AI agents.

---

## Features

1. **Web Search Agent**:
   - Retrieves up-to-date information from the web.
   - Provides reliable and source-cited data using the DuckDuckGo tool.
   - Uses the `Groq` model (Llama 3-based) for optimized tool utilization.

2. **Financial AI Agent**:
   - Accesses real-time financial data, including:
     - Stock prices.
     - Analyst recommendations.
     - Company fundamentals.
     - Latest company news.
   - Displays data in table format for better readability.
   - Utilizes `YFinanceTools` for seamless access to financial datasets.

3. **Multi-Agent Collaboration**:
   - Combines the capabilities of multiple agents (Web Search and Financial).
   - Provides comprehensive financial insights by integrating data from multiple sources.

4. **Interactive Playground**:
   - A web-based interface to interact with the agents dynamically.
   - Built using `Playground` from the PhiData library.

---

## Libraries Used

### 1. **PhiData**
   - A cutting-edge library for building and deploying Agentic AI systems.
   - Key components:
     - **Agent**: Orchestrates task execution using advanced models and tools.
     - **Playground**: Offers a UI for agent interaction.
     - **Models**: Supports models like `Groq` and OpenAI's GPT variants.

### 2. **YFinanceTools**
   - Retrieves financial data such as:
     - Stock prices.
     - Analyst recommendations.
     - Company fundamentals.
     - News updates.

### 3. **DuckDuckGo Tool**
   - Provides web search capabilities with source-cited results.

### 4. **Groq Model**
   - An advanced AI model optimized for tool utilization and multi-agent tasks.

### 5. **dotenv**
   - Loads environment variables securely from a `.env` file.

---

## How It Works

### 1. **Financial Agent**
- Initializes with the `Groq` model.
- Configured to use the `YFinanceTools` for financial data access.
- Displays data in markdown tables.

### 2. **Web Search Agent**
- Uses the `DuckDuckGo` tool for retrieving online information.
- Displays results with sources for transparency.

### 3. **Multi-Agent System**
- Combines multiple agents into a unified system using a team-based approach.
- Example Task: Summarizing analyst recommendations and fetching the latest company news.

### 4. **Interactive Playground**
- Provides a user interface for interacting with the agents.
- Configured and served using `Playground` from PhiData.

---

## Setup Instructions

1. Clone the Repository:
   ```bash
   git clone https://github.com/your-username/financial-analyst-ai-agent.git
   cd financial-analyst-ai-agent

2. Install Dependencies:

    `pip install -r requirements.txt`

3. Configure Environment Variables:

    - Create a .env file with the following:
        ```OPENAI_API_KEY=your_openai_key
        PHI_API_KEY=your_phi_key

4. Run the Application:

    `python playground.py`

5. Access the Playground:

    - Open your browser and navigate to `http://localhost:8000`

---

## Example Query
`multi_ai_agent.print_response("Summarize analyst recommendation and share the latest news for NVDA", stream=True)`
