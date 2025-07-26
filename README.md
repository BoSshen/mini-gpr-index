# Mini GPR Index Construction

This project simulates a simplified index construction process inspired by Solactive AG’s Global Property Research (GPR) team. It downloads REIT stock data, applies simple eligibility rules, and visualizes closing‐price trends.

---

## 🚀 Quick Start

1. **Clone the repo**  
   ```bash
   git clone https://github.com/yourusername/mini-gpr-index.git
   cd mini-gpr-index

	2.	Install dependencies

pip install -r requirements.txt


	3.	Run the analysis
	•	Open notebook.ipynb in Jupyter (or VSCode’s Notebook view).
	•	Step 1: Download REIT stock data (yfinance → data/*.csv).
	•	Step 2: Eligibility check (market‐cap, price growth, volume).
	•	Step 3: Plot closing‐price trends for eligible stocks.

⸻

📂 Repository Structure

mini-gpr-index/
├── data/             # Raw CSV files downloaded by Step 1
├── charts/           # (Optional) Exported plot images
├── scripts/          # (Optional) Standalone Python scripts for each step
├── notebook.ipynb    # Main Jupyter Notebook with full workflow
├── requirements.txt  # Python dependencies
└── README.md         # This documentation


⸻

🔧 Tech Stack
	•	Language: Python
	•	Key Libraries:
	•	pandas — data manipulation
	•	yfinance — fetch stock data from Yahoo Finance
	•	matplotlib — plotting

⸻

📝 Eligibility Rules
	1.	Market Cap ≥ 30 billion USD
	2.	Total Price Growth (first to last close) ≥ 5%
	3.	Average Daily Volume ≥ 1 million shares

Stocks passing all three filters appear in the final index and get plotted.

⸻

📈 Visualization

After the eligibility check, Step 3 produces a line chart of closing prices over the specified period for all qualifying tickers. Date is on the x‐axis, price (USD) on the y‐axis.

⸻

⚙️ Requirements

pandas
yfinance
matplotlib

You can generate requirements.txt by running:

pip freeze > requirements.txt




