# 🌤️ Event & Weather Daily Briefing (n8n Automation)

An automated intelligence briefing workflow built in **n8n**. It aggregates multi-location weather forecasts and historical "This Day in History" events, processes the data using **Groq LLM**, and delivers a smart daily digest straight to **Telegram**.

## 🏗 Workflow Architecture
1. **Schedule Trigger:** Automatically initiates the daily briefing process.
2. **Parallel Weather Fetching:** Simultaneously pulls 5-day weather forecasts for Lutsk, Kyiv, and Spain via HTTP Request nodes.
3. **Historical Data:** Fetches significant events for the current day.
4. **Data Grouping & Normalization:** Groups raw JSON data by type and normalizes the payload.
5. **AI Processing (Groq Chat Model):** Synthesizes the weather and historical data into a coherent, engaging summary using an LLM chain.
6. **Telegram Delivery:** Sends the final automated message to your Telegram chat.

## 🛠 Tech Stack
- **Automation:** n8n
- **AI Engine:** Groq Chat Model (LLM)
- **Data APIs:** Weather Forecast APIs, Historical Events API
- **Output:** Telegram Bot API

## 🚀 How to Use
1. Import the `workflow.json` file into your n8n instance.
2. Connect your **Groq API** credentials.
3. Set up your **Telegram Bot** token and destination chat ID.

📩 **Contact & Custom Solutions:** [My Telegram Channel - Workflow & Scripts](https://t.me/vladiksonchik)
