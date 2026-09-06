# EquiCompare AI - Dual Annual Report Comparative Analyst

A full-stack automated investment decision and financial analysis system that compares two company annual reports (10-K, annual filings, or earnings reports) using an **n8n workflow** and a responsive **Web Frontend**.

---

## 🚀 Key Capabilities

1. **Dual Annual Report Ingestion**:
   - Upload PDF files, `.txt`, or markdown transcripts for Company A and Company B.
   - Live client-side PDF text extraction via `pdf.js`.
2. **Financial Analyst Verdict & Multi-Horizon Strategy**:
   - **Primary Investment Decision**: Quantitative conviction rating & executive synthesis.
   - **Long-Term Compounder (5–10 Years)**: Evaluates Economic Moat durability, ROIC, and capital reinvestment efficiency.
   - **Short-Term Tactical Upside (3–12 Months)**: Evaluates top-line growth acceleration, earnings catalysts, and valuation multiples (P/E).
   - **Dividend & Cash Flow Hold**: Analyzes dividend yield, payout sustainability, and free cash flow coverage.
   - **When to Sell & Risk Management**: Specific margin compression thresholds, leverage limits, and trailing stop-loss guidelines.
3. **Interactive Visual Dashboard**:
   - Side-by-side financial metric scorecard with automatic category winners.
   - Multi-factor Spider/Radar chart powered by Chart.js.
   - One-click export to Markdown, Print, or JSON.
4. **Reports Directory / Archive**:
   - Searchable, persistent local directory storing all historical analysis reports.
   - Filter by company ticker, name, or verdict with one-click reload.

---

## 🛠️ Quick Start Guide

### 1. Access the Web Frontend
The frontend server is running locally:
👉 **[http://localhost:3000](http://localhost:3000)**

### 2. Import the n8n Workflow
1. Open n8n in your browser: **[http://localhost:5678](http://localhost:5678)**
2. In n8n, click **Workflows** $\rightarrow$ **Add Workflow** $\rightarrow$ Click the **`...`** menu (top right) $\rightarrow$ **Import from File**.
3. Select `workflow_annual_report_comparison.json` from this project folder:
   `c:\Users\Itssa\OneDrive\Desktop\Website offer\AI Automation class 2\workflow_annual_report_comparison.json`
4. Click **Publish / Activate** (or click **Test Workflow** on the Webhook node).

---

## 📁 Project Structure

```
├── index.html                           # Modern financial analyst frontend
├── styles.css                           # Glassmorphism & print styles
├── app.js                               # Frontend logic, PDF extraction, Chart.js & n8n connector
├── server.js                            # Static HTTP server (port 3000)
├── workflow_annual_report_comparison.json # Ready-to-import n8n workflow file
├── sample_company_a_apple.txt           # Sample Apple 10-K filing text
└── sample_company_b_microsoft.txt       # Sample Microsoft 10-K filing text
```
