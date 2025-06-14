## 🚀 SpaceX Launch Weather & Risk Analyzer
This Python tool fetches real-time information about the next scheduled SpaceX launch, retrieves live weather forecasts from OpenWeatherMap for the launch site, and uses Groq's LLaMA 3 AI model to assess the launch risk based on weather and aerospace constraints.

## 📌 Features
✅ Retrieves upcoming SpaceX launch details using the SpaceX API

✅ Fetches 3-hour interval weather forecasts using the OpenWeather API

✅ Summarizes temperature trends, wind, humidity, cloud cover, and precipitation

✅ Converts launch pad coordinates into readable formats

✅ Uses Groq + LLaMA 3 to perform a detailed launch risk assessment

✅ Outputs a comprehensive GO/NO-GO report for mission planning

## 📂 Project Structure
.
├── SpaceXLaunchAnalyzer.py   # Main analyzer class
├── .env                      # Environment variables (API keys)
├── README.md                 # Documentation

## 🔧 Requirements
Python 3.7+

requests

python-dotenv

groq (Groq client for LLaMA 3)

Install dependencies:

```bash
pip install requests python-dotenv groq
```
## 🔐 Setup Environment Variables
Create a .env file in the root directory:
```bash
OPENWEATHER_API_KEY=your_openweather_api_key
GROQ_API_KEY=your_groq_api_key
```
## Sample Output:

```bash
🚀 Starting SpaceX Launch Weather Analysis
📡 Fetching launch information...
🔭 Mission: Starlink Group 9-2
⏰ Scheduled: July 5, 2025 at 02:16 UTC
🛰️ Rocket: Falcon 9
🏁 Launch Site: LC-39A
📍 Location: 28.6081°N, -80.6043°E

🌤️ Retrieving weather forecast...

=== SPACEX LAUNCH WEATHER ANALYSIS ===
...
=== LAUNCH RISK ASSESSMENT ===
GO/NO-GO: GO
Primary concerns: Moderate wind
Delay Probability: 20%
Mitigation: ...
```

## 🤖 How AI Is Used
The script sends live launch and weather data to Groq’s LLaMA 3 model via prompt engineering. The model assesses:

Wind limits

Visibility

Precipitation

Cloud ceiling

Lightning proximity
And gives a GO/NO-GO recommendation.

## 📌 API Sources

SpaceX API (v4):
```bash 

https://github.com/r-spacex/SpaceX-API

```

OpenWeatherMap Forecast API:
```bash
https://openweathermap.org/forecast5
```

GroqCloud with LLaMA 3:
```bash
https://console.groq.com/home
```
## ✅ Example Use Cases

Pre-launch checks for aerospace engineers

Weather-informed mission planning

Teaching data-to-text generation with LLMs

Combining real-time APIs with AI inference

## Clone the repo 

```bash
git clone https://github.com/kanishk-rezol/SpaceX-Launch-Weather-Risk-Analyzer
```