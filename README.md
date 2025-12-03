# 📧 Cold Mail Generator 

### **Generate Personalized Cold Emails for Service Companies Using Groq, LangChain, and Streamlit**

This project is an AI-powered cold email generator designed for service-based companies. It automates the process of analyzing job listings from a company’s careers page and generates highly personalized cold emails tailored to those roles. The system also pulls relevant portfolio links from a vector database to enhance the credibility of the outreach.

---

## 🚀 **Features**

* **URL Input for Careers Pages:**
  Provide any company’s careers page URL to fetch open job positions automatically.

* **Job Listing Extraction:**
  Scrapes job titles and descriptions using LangChain tools.

* **Personalized Cold Email Generation:**
  Uses Groq LLM models to craft role-specific outreach emails.

* **Portfolio Retrieval via Vector DB:**
  The system fetches matching portfolio/project links based on job description similarity.

* **Streamlit UI:**
  Clean, interactive interface for business development teams.

* **Real-World Use-Case Example:**

  * Nike is hiring a *Principal Software Engineer*.
  * Atliq (a software services company) wants to offer dedicated engineers.
  * Mohan (BD Executive) uses this tool to send a personalized email with relevant past project links.

---

## 🏗️ **Architecture**

```
Careers Page URL → Job Scraper → JD Embeddings → Vector DB Search
           ↓                             ↓
        LangChain Pipeline ——→ Groq LLM ——→ Personalized Email

---

## 📦 **Tech Stack**

* **Groq LLMs**
* **LangChain**
* **Streamlit**
* **FAISS / Pinecone / Chroma** (depending on your vector DB)
* **Python**

---

## ⚙️ **Setup Instructions**

### **1. Install Dependencies**

```bash
pip install -r requirements.txt
```

### **2. Add Your API Key**

Get a Groq API key here:
[https://console.groq.com/keys](https://console.groq.com/keys)

Create an `.env` file inside the `app/` directory:

```
GROQ_API_KEY=your_api_key_here
```

### **3. Run the Streamlit App**

```bash
streamlit run app/main.py
```

---

## 📁 **Project Structure**

```
├── app/
│   ├── main.py
│   ├── utils/
│   ├── components/
│   ├── .env
├── vectorstore/
├── requirements.txt
├── README.md
```

---


> **AI-powered cold email generator using Groq, LangChain, and Streamlit. Extracts job listings from careers pages and generates personalized outreach emails with relevant portfolio links. Built for service companies to supercharge lead generation.**
