# 🌍 CityGenie

**CityGenie** is an AI-powered City Assistant built using **LangChain**, **Mistral AI**, **Tavily Search**, and the **OpenWeather API**.

It can intelligently answer city-related queries by using external tools for real-time information.

## ✨ Features

- 🌦️ Get the current weather of a city
- 📰 Fetch the latest news about a city
- 🤖 Powered by Mistral AI through LangChain
- 🔒 Human approval before every tool execution
- 💬 Interactive command-line interface

---

## 🛠️ Tech Stack

- Python
- LangChain
- Mistral AI
- Tavily Search API
- OpenWeather API
- Rich
- python-dotenv
- Requests

---

## 📂 Project Structure

```text
CityGenie/
│── main.py
│── .env
│── requirements.txt
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd CityGenie
```

### 2. Create a virtual environment (Optional)

```bash
python -m venv venv
```

Activate the environment:

**Windows**

```bash
venv\Scripts\activate
```

**Linux / macOS**

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the project root.

```env
OPENWEATHER_API_KEY=your_openweather_api_key
TAVILY_API_KEY=your_tavily_api_key
MISTRAL_API_KEY=your_mistral_api_key
```

---

## ▶️ Running the Project

```bash
python main.py
```

Example:

```text
City Agent | type exit to quit

You : What's the weather in Delhi?

Agent wants to call 'get_weather'. Approve? (yes/no):
yes

Bot :
Weather in Delhi: scattered clouds, 32°C
```

---

## 🧰 Available Tools

### 🌦️ Weather Tool

Uses the **OpenWeather API** to fetch the current weather of a city.

Example:

```text
Weather in Mumbai: clear sky, 29°C
```

---

### 📰 News Tool

Uses **Tavily Search API** to retrieve the latest news related to a city.

Example:

```text
Latest news in Delhi

- Metro expansion approved
- Air quality improves
- New infrastructure projects announced
```

---

## 🔒 Human Approval Middleware

Before executing any tool, the agent asks for user confirmation.

Example:

```text
Agent wants to call 'get_news'. Approve? (yes/no):
```

- Type **yes** → Tool executes.
- Type **no** → Tool execution is cancelled.

---

## 💬 Sample Conversation

```text
You : Tell me today's weather in Jaipur.

Agent wants to call 'get_weather'. Approve? (yes/no):
yes

Bot :
Weather in Jaipur: few clouds, 34°C
```

```text
You : Latest news in Bangalore

Agent wants to call 'get_news'. Approve? (yes/no):
yes

Bot :
Latest news in Bangalore:
...
```

---

## 📦 Dependencies

- langchain
- langchain-mistralai
- tavily-python
- python-dotenv
- requests
- rich

Install them using:

```bash
pip install -r requirements.txt
```

---

## 🚀 Future Improvements

- 🌍 Support international cities
- 📅 7-day weather forecast
- 📝 AI-powered news summarization
- 🧠 Conversation memory
- 🌐 Streamlit/Gradio web interface
- 🛠️ More city-related tools

---

## 👨‍💻 Author

**Amam Jain**

🔗 LinkedIn: www.linkedin.com/in/amam-jain-216082386

---

## 📄 License

This project is licensed under the **MIT License**.

---

⭐ If you found this project helpful, consider giving it a **Star** on GitHub!