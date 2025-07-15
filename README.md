# Isro-Bot
# 🌐 GeoAssist – AI-Powered Help Bot for Satellite Data Access

GeoAssist is an intelligent virtual assistant that simplifies information discovery on [MOSDAC (Meteorological and Oceanographic Satellite Data Archival Centre)](https://www.mosdac.gov.in), a public portal hosting satellite products and services. By leveraging NLP, Knowledge Graphs, and Retrieval-Augmented Generation (RAG), GeoAssist enables users to ask natural language questions and receive contextual, accurate, and instant answers.

---

## 🚀 Key Features

- ✅ **Natural Language Query Understanding** using LLMs and intent classification
- 📚 **Knowledge Graph Construction** from structured/unstructured portal content
- 🌍 **Geo-Spatial Intelligence** for region-specific questions (e.g., "rainfall over Tamil Nadu")
- 🔍 **Semantic Search** across FAQs, product manuals, satellite metadata
- 💬 **Chatbot Interface** built with Streamlit/React for real-time user interaction
- ♻️ **Modular Design** suitable for reuse on other government or public data portals

---

## 🧠 Use Case

> “Which satellite provides rainfall data over South India?”
>
> “How can I download cloud motion vectors from MOSDAC?”
>
> “Show me sea surface temperature data for March 2024.”

GeoAssist answers such questions by intelligently parsing MOSDAC's content — including web pages, PDFs, product specs, and FAQs.

---

## 🛠️ Tech Stack

| Layer           | Tools / Frameworks                                 |
|-----------------|-----------------------------------------------------|
| **Frontend**    | Streamlit / React                                   |
| **Backend**     | Python, FastAPI, LangChain                          |
| **NLP**         | spaCy, HuggingFace Transformers                     |
| **RAG Pipeline**| LangChain + ChromaDB / FAISS                        |
| **KG Builder**  | NetworkX / Neo4j                                    |
| **Scraping**    | BeautifulSoup, Selenium, PyMuPDF                    |
| **Geo Analysis**| GeoPandas, Shapely (optional)                       |

---

## 📁 Directory Structure

```plaintext
geoassist/
├── data/                      # Raw + processed portal data
│   ├── raw_html/
│   ├── parsed_text/
│   ├── documents/
├── embeddings/                # Vector DB for RAG
├── kg/                        # Knowledge graph code + outputs
├── frontend/                  # Streamlit / React UI
├── backend/                   # API + LangChain logic
├── utils/                     # PDF/HTML parsers, chunkers, extractors
├── main.py                    # Entry point
├── requirements.txt
└── README.md
