# 🌍 AI Trip Planner

**AI Trip Planner** is an intelligent, agentic application that helps users plan trips to any destination worldwide. It leverages real-time data, advanced language models, and a suite of tools to generate detailed, actionable travel plans, including itineraries, cost breakdowns, weather forecasts, and more.

---

## 🚀 Features

- **Conversational Trip Planning**: Chat-based interface for users to request custom travel plans.
- **Day-by-Day Itinerary**: Generates detailed itineraries for both popular and off-beat locations.
- **Hotel & Restaurant Recommendations**: Suggests hotels (with price estimates) and top restaurants.
- **Attractions & Activities**: Lists must-see places and activities with details.
- **Weather Integration**: Provides current and forecasted weather for your destination.
- **Expense & Currency Tools**: Calculates total and daily expenses, and converts currencies.
- **Transportation Info**: Details available modes of transport at your destination.
- **Markdown Export**: Save your travel plan as a well-formatted Markdown document.

---

## 🏗️ Project Structure

```
.
├── agent/                # Core agent workflow and orchestration
├── config/               # Configuration files (e.g., LLM providers)
├── exception/            # Custom exception handling
├── logger/               # Logging utilities
├── notebook/             # Experimentation and prototyping notebooks
├── prompt_library/       # System and tool prompts
├── tools/                # Tool wrappers (weather, places, expenses, currency)
├── utils/                # Utility modules (API wrappers, calculators, config loaders)
├── env/                  # Environment and secrets (not tracked)
├── main.py               # Simple CLI entry point
├── streamlit_app.py      # Main Streamlit web application
├── requirements.txt      # Python dependencies
├── setup.py              # Packaging and installation
├── pyproject.toml        # Project metadata
└── README.md             # Project documentation
```

---

## 🖥️ Quick Start

### 1. **Clone the Repository**
```bash
git clone <your-repo-url>
cd AI_Trip_Planner
```

### 2. **Install Dependencies**
```bash
pip install -r requirements.txt
```

### 3. **Set Up Environment Variables**
Create a `.env` file in the root directory with the following keys (get API keys from respective providers):

```
OPENWEATHERMAP_API_KEY=your_openweathermap_key
GPLACES_API_KEY=your_google_places_key
EXCHANGE_RATE_API_KEY=your_exchangerate_key
ALPHAVANTAGE_API_KEY=your_alphavantage_key
```

### 4. **Run the Streamlit App**
```bash
streamlit run streamlit_app.py
```
Open the provided local URL in your browser.

---

## 🧠 How It Works

- **Frontend**: Built with Streamlit, provides a chat interface for user queries.
- **Backend/Agent**: Orchestrates LLMs (OpenAI, Groq, etc.) and tools for weather, places, expenses, and currency.
- **Tools**: Modular Python classes for fetching weather, searching places, calculating expenses, and converting currencies.
- **Prompt Engineering**: Uses a system prompt to ensure comprehensive, actionable, and well-formatted travel plans.

---

## 🛠️ Key Technologies

- **Python 3.12+**
- **Streamlit** (UI)
- **LangChain** (LLM orchestration)
- **OpenAI, Groq** (LLM providers)
- **Google Places, OpenWeatherMap, ExchangeRate APIs** (data sources)
- **FastAPI** (for backend endpoints, if extended)
- **Pydantic, dotenv, requests** (utilities)

---

## 📦 Installation (Development)

- Install in editable mode:
  ```bash
  pip install -e .
  ```

- Run tests and experiments in the `notebook/` directory.

---

## 📄 Example Usage

1. **Ask:**  
   _"Plan a trip to Paris for 7 days with a moderate budget."_

2. **Get:**  
   - Two detailed itineraries (mainstream & off-beat)
   - Hotel and restaurant suggestions with prices
   - Attractions, activities, and transportation info
   - Weather forecast and daily expense breakdown
   - Option to export the plan as a Markdown file



## 🙏 Acknowledgements

- [LangChain](https://github.com/langchain-ai/langchain)
- [Streamlit](https://streamlit.io/)
- [OpenWeatherMap](https://openweathermap.org/)
- [Google Places API](https://developers.google.com/maps/documentation/places/web-service/overview)
- [ExchangeRate-API](https://www.exchangerate-api.com/)

---

**Created by Raju Baddela**  
Contact: rajubaddela1234@gmail.com

---
