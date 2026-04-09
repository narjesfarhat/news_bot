📰 Intelligent News Summarization Bot with Topic Tagging & Relevance Insights

A lightweight, AI‑powered news assistant that aggregates current headlines, generates concise summaries, and highlights why each story matters.
Built to demonstrate practical NLP techniques for information filtering, topic understanding, and content prioritization.

🚀 Key Features
🔎 1. Automatic Topic Classification
Automatically assigns categories such as:

Technology

Politics

Economy

World News

Science

Sports

This helps users instantly understand the domain of each article.

🧹 2. Duplicate Article Filtering
Removes repeated or near‑duplicate stories across sources, reducing noise and improving clarity.

🧠 3. “Why This Matters” Insights
For every article, the bot generates a short contextual explanation that answers:

Why is this news important?

This transforms raw headlines into meaningful, digestible insights.

🧼 4. Clean, Structured Output
Each processed article includes:

Title

Summary

Topic tag

Relevance insight

Source

Perfect for dashboards, newsletters, or automated reporting.

🧰 Tech Stack
Component	Technology
LLM	phi‑3 via Ollama
NLP Framework	LangChain
Document Parsing	PyMuPDF
Vector Store	ChromaDB
Frontend	Gradio
Language	Python

📁 Project Structure
Code
📦 Intelligent News Summarization Bot
 ┣ 📂 news_articles/          # Raw input articles
 ┣ 📂 chroma_news_db/         # Vector database
 ┣ 📜 News_bot.py             # Main application
 ┣ 📜 requirements.txt        # Dependencies
 ┣ 📜 README.md               # Project documentation
⚙️ How It Works
Load Articles  
PDFs or text files are parsed and cleaned.

Chunk & Embed  
Articles are split into semantic chunks and embedded using an LLM‑compatible embedding model.

Store in ChromaDB  
Embeddings are indexed for fast retrieval.

Generate Summaries & Insights  
The LLM produces:

A concise summary

A topic classification

A “why this matters” explanation

Serve via Gradio UI  
Users can query, browse, and interact with the processed news.

🧪 Use Cases
Daily news briefings

Automated newsletters

Research assistants

Media monitoring tools

Content recommendation engines

📦 Installation
bash
pip install -r requirements.txt
Make sure Ollama is installed and running:

bash
ollama serve
ollama pull phi3
▶️ Run the App
bash
python News_bot.py
