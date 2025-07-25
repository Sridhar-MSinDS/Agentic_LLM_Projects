# Agentic_LLM_Project
An agentic LLM for travel advisory is an AI system that interacts with users, gathers preferences, searches real-time data (flights, hotels, attractions, etc..), and makes decisions or suggestions—mimicking a human travel agent with contextual memory and task execution capabilities.

# ✈️ AI-Powered Flight Recommendation System
An intelligent travel advisory agent built using LangChain, OpenAI's GPT-3.5, and the Amadeus Travel API, capable of parsing natural language flight queries and returning real-time flight offers.

# 🚀 Features
🧠 Agentic Reasoning via LangChain Agent

💬 Natural Language Understanding using OpenAI GPT-3.5

🌐 Real-Time Flight Search using Amadeus API

📝 Conversation Memory with LangChain BufferMemory

🔎 Airline Code Translation into full names using LLM

📅 Supports Round-Trip & One-Way Flights

✅ IATA Code Extraction & Date Parsing


# 📁 Project Structure
flight_agent/

├── main.py               # Entry point of the app (agent + tool setup)

├── requirements.txt      # Dependencies

└── README.md             # Project documentation



# 🔧 Prerequisites
Python 3.8+

Amadeus Developer Account: Get API Keys

OpenAI API Key: Get API Key


# 🔐 Environment Variables
You must set the following environment variables before running:
bash

export OPENAI_API_KEY="your-openai-api-key"

export AMADEUS_API_KEY="your-amadeus-api-key"

export AMADEUS_API_SECRET="your-amadeus-api-secret"

Or place them in a .env file and load using python-dotenv.


# 🛠️ Installation
bash
# Clone the repo
git clone https://github.com/yourusername/flight-agent.git
cd flight-agent


# Install dependencies
pip install -r requirements.txt
▶️ Usage
bash
python main.py

💬 Example Prompt:
Recommend me flights from baltimore to new york on november 23rd, 2024 and return on november 25th, 2024

The agent will:

Parse the origin, destination, and dates.

Fetch flights via the Amadeus API.

Translate airline codes to full names.

Display top 5 matching flight options.


# 🧩 How It Works
LangChain Agent: Routes parsed flight details to a custom flight search tool.

Amadeus Tool: Queries real-time flight data.

OpenAI LLM: Handles: Natural language parsing (location, dates), Airline code translation

ConversationBufferMemory: Maintains contextual memory for multi-turn interactions.

# 🧪 Sample Output
yaml

Airline: Delta Air Lines
Price: $132.00
Departure: 2024-11-23T08:15:00
Arrival: 2024-11-23T09:25:00
Duration: 1 hours 10 minutes

Return Departure: 2024-11-25T19:45:00
Return Arrival: 2024-11-25T20:55:00
Return Duration: 1 hours 10 minutes

----------------------------------------


# 📦 Dependencies
LangChain

OpenAI

Amadeus Python SDK

Python Standard Libraries: os, json, re, warnings


# 🚏 Local Public Transportation Recommendation Agent
An intelligent agent built with LangChain, GPT-4, and Geoapify Places API that provides nearby public transportation options (bus stops, train stations, etc.) based on user-input locations. It uses natural language input, geocodes locations, and returns transport hubs within a defined radius.

# 🧠 Features
🌍 Natural language input (e.g., "Show me transport near Central Park, NYC")

📍 Location geocoding via Geoapify

🚉 Fetches nearby public transport hubs (bus, train, tram, etc.)

🧠 Memory-enabled agent using LangChain

# 🗂️ Project Structure
transport_agent/
│

├── main.py               # Agent code

├── requirements.txt      # Dependencies

└── README.md             # Project documentation

# 🔧 Prerequisites
Python 3.8+

API Keys:

OpenAI API

Geoapify API

# 🔐 Environment Variables
Make sure to set the following in your environment or .env file:

export OPENAI_API_KEY="your-openai-api-key"

export GEOAPIFY_API_KEY="your-geoapify-api-key"

# 🛠️ Installation
# Clone the repository
git clone https://github.com/yourusername/transport-agent.git
cd transport-agent

# Install dependencies
pip install -r requirements.txt

# 🧾 Sample Output

Transport Hub: Panama
Categories: public_transport, public_transport.bus
Address: Panama, National highway 65, Ward 15 Vanasthalipuram, Hyderabad - 500963, Telangana, India
----------------------------------------

Transport Hub: Vanasthalipuram
Categories: public_transport, public_transport.bus
Address: Vanasthalipuram, NH65, Ward 12 Mansoorabad, Hyderabad - 500070, Telangana, India
----------------------------------------

# 🛡️ Disclaimer
This project is for educational and prototyping purposes. Always validate final travel plans with the airline or provider directly.


# 📜 License
MIT License. See LICENSE for details.


# 🙌 Acknowledgments
OpenAI

Amadeus for Developers

LangChain
