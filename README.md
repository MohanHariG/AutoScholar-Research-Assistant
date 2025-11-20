AutoScholar Research Assistant

A multi-agent system that automates online research using search, extraction, summarization, and citations.

⭐ Overview

AutoScholar Research Assistant is a project that turns any topic into a clean, easy-to-understand research summary.
Instead of searching the web manually and reading multiple articles, this tool does the entire workflow for you using AI agents.

You enter a topic.
The system searches the web, collects information, extracts useful text, generates a summary, lists citations, and saves everything for later.

It works like a small research team inside a single notebook.

🎯 Key Features
- Automated Web Search using SerpAPI
- Parallel Page Fetching for faster processing
- Smart Text Extraction from webpages
- Top Passage Selection
- Citation Ranking based on relevance
- Summarization (fallback summarizer for stable output)
- 5-Bullet Outline Generation
- Session Memory stored in JSON
- Observability Tools (logs, event timeline, metrics)
- Human Evaluation CSV Export

🧠 Why I Built This

Research takes a lot of time:
searching → reading → filtering → summarizing → citing.
Most people repeat this every day.
I wanted to build an agent system that:
saves time
organizes the workflow
automates repetitive steps
produces a clear, helpful output
AutoScholar does all of this with one command.

🏗️ System Architecture

The project uses a multi-agent pipeline:

* Orchestrator Agent
Controls the workflow and links all agents together.

* Search Agent
Uses SerpAPI to find relevant webpages.

* Fetch Agents (Parallel)
Download and extract text from web pages.

* Extraction Agent
Picks the most meaningful passages.

* Citation Agent
Ranks sources by relevance.

* Summarizer Agent
Creates a summary + outline + citations.

* Memory System
Stores past research sessions in JSON.

* Observability Tools
Logging, tracing, latency checks, usage counts.

🔧 Tech Stack

* Python
* SerpAPI (web search)
* BeautifulSoup (HTML parsing)
* ThreadPoolExecutor (parallel fetching)
* Matplotlib (charts and timeline)
* JSON (memory + logs)
* Kaggle Notebook environment

🚀 How It Works

- Enter any topic in the notebook cell
- The orchestrator starts the pipeline
- Search results are collected
- Pages are fetched and text extracted
- Important passages are selected
- Summary + outline are generated
- Citations are added
- Memory is updated
- Logs are written for observability
- The output is clean, readable, and backed by real sources.

🧪 Observability

The notebook includes:
* JSON event logs
* A timeline plot of agent events
* Tool usage count
* Latency calculations
* Recent session viewer
This makes debugging and evaluation easy.

📊 Human Evaluation:

The system automatically exports:

topic | summary | outline | citations | relevance | coherence | correctness | notes


🌟 Value

AutoScholar reduces hours of research into seconds.
It keeps everything:
- simple
- clear
- repeatable
- reliable
It is helpful for:
- students
- developers
- analysts
- content creators
- anyone learning something new

🔮 Future Improvements

* Add Gemini summarizer (full version)
* Add UI interface
* Add persistent memory database
* Improve citation checking
* Add topic clustering for multi-topic research

🙌 Acknowledgements

This project was built as part of the 5-Day Kaggle Agents Intensive.
Thanks to Google, Kaggle, and the teaching team for the course content and examples that inspired this project.
