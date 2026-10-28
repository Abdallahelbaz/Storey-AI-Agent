# Multi-Agent Procurement & Market Intelligence System

An automated multi-agent workflow built using **CrewAI**, **AgentOps**, **Tavily Search API**, and **ScrapeGraphAI**. This system acts as an intelligent procurement assistant that formulates optimal search strategies, discovers and scrapes product listings across e-commerce platforms (e.g., Amazon, Jumia, Noon), evaluates product specifications and pricing, and generates a clean, executive HTML report.

---

## 🚀 Key Features

* **Search Strategy Generation:** Dynamically generates optimized search queries tailored for specific e-commerce platforms and regions.
* **Intelligent Product Discovery:** Leverages Tavily API to locate relevant product listings and filter high-confidence URLs.
* **Deep Web Scraping:** Employs ScrapeGraphAI to extract structured product data (prices, specifications, discounts, images, links).
* **Automated Executive Reporting:** Synthesizes scraped product data into a fully styled Bootstrap HTML procurement report.
* **Observability & Analytics:** Integrated with AgentOps to track agent steps, latency, execution traces, and costs.

---

## 🛠️ Prerequisites & Installation

### 1. Clone the Repository
```bash
git clone https://github.com/Abdallahelbaz/Storey-AI-Agent.git
cd your-repository-name
```

### 2. Create a Virtual Environment (Optional but Recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

---

## ⚙️ Environment Configuration

Create a `.env` file in the root directory by copying `.env.example` or setting the following variables:

```bash
cp .env.example .env
```

Add your credentials inside `.env`:

---

## 🏃 Usage

Run the main pipeline or execute the notebook cells to start the research agent crew:

---

## 📂 Output Structure

All intermediate outputs and final artifacts are stored under the `./ai_agent_output` directory:

```text
ai_agent_output/
├── step_1_suggested_search_queries.json  # Recommended regional search queries
├── step_2_search_results.json             # Aggregated store links & search results
├── step_3_scraped_products_info.json     # Extracted product details & prices
└── step_4_procurement_report.html        # Interactive Bootstrap HTML report
```

