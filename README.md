# Weather & Search AI Agent with LangChain
![banner](./images/banner.png)
An AI assistant that combines **web search** and **live weather information** using LangChain's ReAct agent. It uses OpenAI to interpret questions, Tavily to search the web, and Weatherstack to retrieve current weather conditions. A simple Streamlit interface lets users ask questions interactively.

## Features

- Answer general questions using Tavily web search.
- Retrieve current temperature, weather conditions, and humidity for a city.
- Combine search and weather tools to answer multi-step questions.
- Interact through a Streamlit web app or run a command-line example.

## Tech Stack

Python · LangChain · OpenAI (`gpt-3.5-turbo`) · Tavily Search · Weatherstack API · Streamlit

## Getting Started

1. Clone or download the project and open its directory.
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Create a `.env` file in the project root with your API keys:

   ```dotenv
   OPENAI_API_KEY=your_openai_api_key
   TAVILY_API_KEY=your_tavily_api_key
   WEATHERSTACK_API_KEY=your_weatherstack_api_key
   ```

4. Start the Streamlit app:

   ```bash
   streamlit run app.py
   ```

   Alternatively, run the command-line example:

   ```bash
   python main.py
   ```

## Example Query

> Find the capital of Nigeria and tell me its current weather.

The agent searches for the capital, then uses the weather tool to retrieve current conditions for that city.

## Project Structure

```text
├── app.py              # Streamlit interface and agent
├── main.py             # Command-line agent example
├── requirements.txt    # Python dependencies
└── research/           # Experimental notebook
```

## Notes

API keys are required, and the services may incur usage charges. Keep `.env` files out of version control. Weather data availability depends on your Weatherstack plan.
