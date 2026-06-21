# Caiyun Weather / 彩云天气 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/caiyun-weather)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/caiyun-weather-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/caiyun-weather-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

China's leading high-precision weather service — get minute-level precipitation and air quality via AI.

## Description
Empower your AI agent to orchestrate your environmental monitoring and high-precision weather forecasting with **Caiyun Weather** (彩云天气), the pioneer of minute-level precipitation forecasting in China. By connecting Caiyun to your agent, you transform complex meteorological data, air quality auditing, and long-term forecasts into a natural conversation. Your agent can instantly retrieve real-time conditions for any coordinate, provide hyper-local rain alerts for the next two hours, and audit historical or forecast trends without you ever needing to navigate a weather map. Whether you are planning outdoor logistics or monitoring air quality for retail branches, your agent acts as a real-time environmental coordinator, providing accurate and fast results from a single, authorized source.

### What you can do

- **Minute-Precision Rain** — Access hyper-local precipitation forecasts for the next 120 minutes with high resolution.
- **Real-time Auditing** — Retrieve current temperature, humidity, visibility, and wind conditions for specific coordinates.
- **Air Quality Monitoring** — Access real-time AQI and pollutant data (PM2.5, PM10) across mainland China.
- **Long-term Forecasting** — Retrieve detailed hourly and daily weather trends for up to 15 days.
- **Geographic Flexibility** — Query any location using Longitude,Latitude (GCJ-02) or administrative codes.

### How it works

1. Subscribe to this server
2. Enter your Caiyun Weather Token (天气令牌)
3. Start monitoring your environmental data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Operations** — coordinate deliveries and outdoor activities with minute-level rain precision.
- **Health & Wellness Services** — monitor real-time air quality data to provide timely advice to users.
- **Developers** — integrate professional-grade meteorological APIs into your AI-driven daily routines.
- **Caiyun Power Users** — integrate your existing weather workflows into your AI-driven daily routines.


## Available Tools
- **get_aqi_info**: Get air quality index
- **get_daily_forecast**: Get daily weather forecast
- **get_hourly_forecast**: Get hourly weather forecast
- **get_minutely_rain**: Get minute-precision rain
- **get_precipitation_probability**: Check rain probability
- **get_realtime_weather**: Get real-time weather
- **get_visibility_data**: Get visibility distance
- **get_wind_conditions**: Get wind speed and direction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Caiyun Weather / 彩云天气** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the real-time weather at coordinates 121.47,31.23 (Shanghai)?"

**🤖 AI Agent:**
> The current weather in Shanghai is 22 °C with clear skies. The humidity is 65% and visibility is excellent at 15 km. Should I also check if there's any rain forecast for the next hour?

---

**👤 You:**
> "Will it rain in the next 2 hours at 116.40,39.90 (Beijing)?"

**🤖 AI Agent:**
> According to Caiyun's minutely forecast, there is no rain expected in your area for the next 120 minutes. It will remain cloudy. Would you like me to check the daily forecast for the rest of the week?

---

**👤 You:**
> "Check the air quality index for coordinates 113.26,23.12 (Guangzhou)."

**🤖 AI Agent:**
> I've retrieved the AQI for Guangzhou. The current index is 45, which is 'Good'. Pollutant levels are low, with PM2.5 at 12 μg/m³. Is there anything else you'd like to know about the environmental conditions there?


## Installation & Usage

To install and use the **Caiyun Weather / 彩云天气** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/caiyun-weather](https://vinkius.com/mcp/caiyun-weather)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
