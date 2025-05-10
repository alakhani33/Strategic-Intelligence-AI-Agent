<<<<<<< HEAD

# 🕵️ AI Agent for Strategic Intelligence

This project implements a deployable AI agent that extracts **strategic intelligence** from company websites and public data sources. The agent is designed to:

- Scrape and ingest content from a list of provided company URLs.
- Build a **retrieval-based QA chain** using Gemini embeddings and a FAISS vector store.
- Integrate with external tools like **Wikipedia** and **OpenWeatherMap** using LangChain.
- Prioritize answering queries from internal company data first, with external fallbacks if needed.
- Deploy via a **Gradio app** for user-friendly interaction.

We use **Kaiser Permanente** as a case study example.

---

## 🚀 Features

- **Custom Website Retrieval Tool:** Scrapes and embeds content from specified URLs, enabling domain-specific question answering.
- **Smart Query Handling:** Prioritizes company data and falls back to external tools when internal data is insufficient.
- **LangChain Agent Framework:** Combines custom tools with pre-built tools (Wikipedia, OpenWeatherMap).
- **Gradio Interface:** Lets users input queries and view responses in a simple web interface.
- **Optimized for Performance:** Saves and reloads FAISS indexes to avoid repeated embedding.

---

## 🛠 Technologies Used

- Python 🐍
- LangChain
- Gemini (Google Generative AI)
- FAISS (Vector Store)
- Gradio (Web Interface)
- BeautifulSoup & Requests (Web Scraping)

---

## ⚙️ How It Works

1. **Web Crawling (Optional):** Crawl a top-level URL to discover embedded links.
2. **Web Content Loading:** Load web pages using `WebBaseLoader`.
3. **Chunk & Embed:** Split content into chunks and embed using Gemini embeddings.
4. **Vector Store:** Store embeddings in FAISS (with `save_local` and `load_local` for performance).
5. **Retrieval QA:** Set up a retrieval-based QA chain to answer questions from ingested web content.
6. **Tool Wrapping:** Wrap the retrieval chain as a custom LangChain tool.
7. **Agent Assembly:** Combine the custom tool with Wikipedia and OpenWeatherMap tools.
8. **Smart Query Execution:** First attempt to answer using website data; if insufficient, fall back to external sources.
9. **Gradio Deployment:** Deploy as a web app where users input queries and receive answers.

---

**Gradio App:**
   The Gradio interface lets users input questions interactively.

---

## 💡 Example Queries

- "What is Kaiser Permanente's mission?"
- "How many doctors work for Kaiser Permanente?"
- "Who is the CEO of Kaiser Permanente?"
- "What is the current weather in the city where Kaiser was founded?"

---

=======
# Strategic-Intelligence-AI-Agent
This project implements a deployable AI agent that extracts strategic intelligence from company websites and public data sources. Using Kaiser Permanente as a case study, the agent scrapes and embeds web content, builds a retrieval-based QA system, and integrates with external tools (Wikipedia) via LangChain. The agent prioritizes answers from company data first, falling back to external sources only if needed. The solution is wrapped in a Gradio app for easy user interaction.
>>>>>>> 9349923f337f85c4bb4d342e840c5889f66e1a5c
