# 🌍 Julep AI Foodie Tour Planner

## Overview

This is a submission for the AI Engineering Intern Task at Julep AI. The goal is to build an AI-powered workflow that, for a given list of cities:

1. Checks today's weather and suggests indoor or outdoor dining.
2. Picks 3 iconic local dishes per city.
3. Finds top-rated restaurants serving these dishes.
4. Crafts a one-day foodie tour with breakfast, lunch, and dinner suggestions, factoring in weather conditions.

---

## Solution Highlights 🚀
- Built using Julep AI's visual workflow builder.
- Inspired by the Trip Planning Assistant from Julep's official examples.
- Integrated multiple tools to automate:
- Weather check (OpenWeatherMap API).
- Iconic food selection (Wikipedia API).
- Restaurant search (designed for Brave Search API, but couldn't test due to missing API key).

---

## Limitations & Roadblocks ⚠️
- Brave API Key Missing: I was unable to test the restaurant search component because I didn't have access to the Brave Search API key. The corresponding tool is implemented but not verified end-to-end.
- User-Defined Tools: I explored creating custom tools using the user-defined function feature in Julep, but couldn’t find sufficient documentation on how to execute these within the Julep Agent. As a result, I used pre-existing tools following the cookbook examples.
- As a backup, I implemented the entire workflow in LangChain (Python) as well, where I was able to test and verify the logic end-to-end.

---

## Julep Workflow Design 🛠
- **Agent Setup**: Follows Julep's agent creation guidelines.
- **Tools Used**:
    - Weather Tool
    - Wikipedia Tool
    - Brave Search Tool

All tools were chained using Julep’s built-in prompt logic and conditional execution.

---

## Alternative Implementation 🐍 (LangChain)
To ensure functionality, I also built the same workflow using LangChain in Python. This version uses:
- **OpenWeatherMap API** for weather.
- **Wikipedia API** for dish names.
- **EXA Search** for internet search.
- **ChatGroq** for narratives.

✅ This LangChain implementation is fully tested.

