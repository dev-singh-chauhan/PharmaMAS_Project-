# 💊 PharmaMAS — AI-Powered Multi-Agent System for Drug Repurposing  
*A CrewAI-based innovation engine for pharmaceutical research.*

---

## 🚀 Overview

PharmaMAS is a **Multi-Agent AI System** built using **CrewAI** that automates pharmaceutical molecule research and identifies potential **drug repurposing opportunities**.

Instead of spending **2–3 months** manually analyzing market data, patents, clinical trials, scientific papers, and internal documents, PharmaMAS performs the entire workflow in **under 3 minutes** using coordinated AI agents.

This project was developed for a **pharmaceutical innovation hackathon challenge** to demonstrate the power of Agentic AI in streamlining early-stage product evaluation.

---

## 🎯 Problem Statement

Pharma companies operating in the competitive generics market must innovate to stay profitable.  
One effective strategy is **drug repurposing**—finding new uses, new dosage forms, or new patient segments for existing approved molecules.

However, discovering these opportunities requires:

- Market research  
- Patent landscape analysis  
- Clinical trial exploration  
- Scientific literature review  
- API trade analysis  
- Internal knowledge extraction  

This process is **slow, repetitive, and performed manually**.

PharmaMAS solves this bottleneck.

---

## 🧠 Solution Summary

PharmaMAS automates repurposing research using a **Multi-Agent Architecture**:

- The **Master Agent** interprets user queries, breaks them into tasks, and coordinates Worker Agents.
- **Worker Agents** analyze mock datasets for market, patents, clinical trials, EXIM trends, web intelligence, and internal insights.
- A **Report Generator Agent** produces a professional PDF + Excel output summarizing all findings.

This enables rapid, scalable, and consistent molecule evaluation.

---

## 🏗️ Architecture (Simple Version)

                 User (Streamlit UI)
                          │
                          ▼
                  Master Agent (CrewAI)
                          │
         ┌──────────────────────────────────────┐
         │         Worker Agents Group           │
         │                                        │
         │  • Market Insights Agent               │
         │  • Patent Landscape Agent              │
         │  • Clinical Trials Agent               │
         │  • EXIM Trade Agent                    │
         │  • Web Intelligence Agent              │
         │  • Internal Knowledge Agent            │
         └──────────────────────────────────────┘
                          │
                          ▼
                 Report Generator Agent
                          │
                          ▼
                PDF Report + Excel Summary
                 User (Streamlit UI)
                          │
                          ▼
                  Master Agent (CrewAI)
                          │
         ┌──────────────────────────────────────┐
         │         Worker Agents Group           │
         │                                        │
         │  • Market Insights Agent               │
         │  • Patent Landscape Agent              │
         │  • Clinical Trials Agent               │
         │  • EXIM Trade Agent                    │
         │  • Web Intelligence Agent              │
         │  • Internal Knowledge Agent            │
         └──────────────────────────────────────┘
                          │
                          ▼
                 Report Generator Agent
                          │
                          ▼
                PDF Report + Excel Summary

---

## 🗂️ Project Structure

pharma_mas/
│
├── agents/ # Agent definitions
├── crew/ # Task and crew setup
├── mock_data/ # Mock datasets (JSON, CSV)
├── reports/ # Generated PDF & Excel files
├── app.py # Streamlit UI
└── PharmaMAS.ipynb # Google Colab notebook


---

## 📊 Mock Data Used

PharmaMAS uses high-quality mock datasets to simulate:

- **IQVIA Market Data**  
- **Patent Database (USPTO mock)**  
- **Clinical Trials Pipeline**  
- **EXIM Import/Export API**  
- **Scientific Web Articles**  
- **Internal Strategy Insights**

These are stored in `/mock_data/`.

---

## 🧩 Multi-Agent System Components

### **1. Master Agent**
- Interprets user query  
- Breaks tasks  
- Orchestrates Worker Agents  
- Synthesizes results  
- Applies repurposing heuristics  

### **2. Worker Agents**
- Market Insights Agent  
- Patent Landscape Agent  
- Clinical Trials Agent  
- EXIM Trade Agent  
- Web Intelligence Agent  
- Internal Knowledge Agent  

### **3. Report Generator Agent**
Outputs:
- **PDF Report**
- **Excel Workbook**

---

## 🖥️ Frontend (Optional)

A lightweight **Streamlit** UI is included:

- Molecule input field  
- “Run Analysis” button  
- Access to generated reports  
- Hosted via **Cloudflared Tunnel** on Google Colab  

---

## 🧪 How to Run (Google Colab Recommended)

1. Clone the repository  
2. Open the Colab notebook  
3. Run all cells  
4. Enter a molecule (e.g., `"Metformin"` or `"Aspirin"`)  
5. Download the generated PDF + Excel files

---

📦 Requirements

Python 3.10+

CrewAI

Pandas

ReportLab

Streamlit (optional)

cloudflared (for UI tunneling)

openpyxl

python-dotenv

📈 Output Example

PharmaMAS generates:

Market Summary

Patent Expiry Tables

Clinical Trials Overview

EXIM Import/Export Trends

Scientific Literature Summary

Internal Insights

Repurposing Opportunity Flags

Final PDF + Excel

🌟 Key Impact

90% faster repurposing research

Enables rapid evaluation of dozens of molecules

Produces standardized decision-ready reports

Reduces human effort dramatically

Improves innovation pipeline quality

👥 Team & Credits

Developed by:
[Dev Singh Chauhan & Team Members]
Built for: EY Techathon 6.0
Pharmaceutical Innovation Hackathon 

🙌 Acknowledgements

CrewAI multi-agent framework

OpenAI

Google Colab

Streamlit
