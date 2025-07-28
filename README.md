# 📚 Semantic Book Recommender using LLMs

This repository contains all the code and assets required to build a **Semantic Book Recommender** powered by **Large Language Models (LLMs)** and deployed with **Gradio**.

this project takes you through a modern GenAI pipeline—from vector search to LLM-based classification—all wrapped in an interactive UI.

---

## 🧠 Core Components

1. **Text Data Cleaning**
   - Notebook: `data-exploration.ipynb`
   - Preprocesses book metadata and descriptions.

2. **Semantic Search / Vector Database**
   - Notebook: `vector-search.ipynb`
   - Uses embeddings to store books and retrieve similar ones based on natural language queries.

3. **Zero-shot Text Classification**
   - Notebook: `text-classification.ipynb`
   - Classifies books into `Fiction` or `Non-Fiction` using an LLM without training.

4. **Sentiment & Emotion Analysis**
   - Notebook: `sentiment-analysis.ipynb`
   - Extracts the tone (e.g., suspenseful, joyful, dark) of each book.

5. **Gradio Web App**
   - File: `gradio-dashboard.py`
   - Allows users to get book recommendations based on natural queries and filter via classification or sentiment.

---

## 🚀 Live Demo (Locally)

To run the Gradio app:

```bash
conda activate your_env_name  # Activate your environment
python gradio-dashboard.py    # Launch the web UI
```

---

## 📁 Directory Structure

```
📦semantic-book-recommender/
├── data-exploration.ipynb
├── vector-search.ipynb
├── text-classification.ipynb
├── sentiment-analysis.ipynb
├── gradio-dashboard.py
├── requirements.txt
├── .env
└── README.md
```

---

## 🔧 Installation

This project was built with `Python 3.11`

### 1. Clone the repository

```bash
git clone https://github.com/mohitbansal25082006/NovelNexus.git
cd NovelNexus
```

### 2. Create and activate environment

```bash
conda create -n bookai python=3.11
conda activate bookai
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the root directory and add your **OpenAI API key**:

```
OPENAI_API_KEY=your_openai_key_here

HUGGINGFACEHUB_API_TOKEN=your_huggingfacehub_token_here

```

---

## 📦 Dependencies

Key libraries used in this project:

- `kagglehub`
- `pandas`, `matplotlib`, `seaborn`
- `python-dotenv`
- `langchain`, `langchain-community`, `langchain-chroma`
- `transformers`, `openai`
- `gradio`
- `ipywidgets`, `notebook`

Install all via:

```bash
pip install -r requirements.txt
```

---

## 📊 Dataset

The book metadata and descriptions used in this project can be downloaded from **Kaggle**. Follow the instructions in the notebooks to link your Kaggle API key and fetch the dataset automatically.

---

## ✨ Features

- Semantic search for books using sentence embeddings
- LLM-based classification: Fiction vs Non-Fiction
- Emotional tone detection with AI
- Fully interactive **Gradio interface**
- Easy to extend for any type of semantic recommender

---

## 🙌 Credits

Inspired by the course: [Build a Semantic Book Recommender with LLMs – Full Course (freeCodeCamp)](https://www.youtube.com/watch?v=Q7mS1VHm3Yw&t=2512s)
