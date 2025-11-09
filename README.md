# FinQuery — Natural Language to Pandas Financial Assistant

FinQuery is a **local, secure, and intelligent data analysis tool** that converts natural language (NL) financial queries into **safe Pandas (Python Data Analysis Library) operations**.  
It enables users to ask questions about bank or expense data in plain language and receive accurate tables, charts, and insights instantly.

---

## 🚀 Project Goal
To build a sandboxed system that:
- Understands financial questions in natural language (NL)
- Converts them into validated Python/Pandas code
- Executes them securely in a restricted environment
- Displays results visually using tables and charts
- Works offline with **no paid API (Application Programming Interface)** required

---

## 🧠 Key Features
- **Natural Language Querying** (e.g., *"Show my total spend in March"*)
- **Safe Code Generation** using AST (Abstract Syntax Tree) validation
- **Sandboxed Execution** to prevent harmful code execution
- **Financial Insights** using charts and structured data
- **Store and Reuse Queries**
- **Streamlit UI (User Interface)** for interactive usage
- **Synthetic or real CSV (Comma Separated Values) support**

---

## 🏗 Project Structure

finquery/
├─ data/ # Sample synthetic CSV datasets
├─ finquery/
│ ├─ nl_parser.py # Query parsing logic
│ ├─ ast_schema.py # Code safety schema
│ ├─ generator.py # Natural Language → Pandas code
│ ├─ sandbox.py # Safe execution environment
│ ├─ renderer.py # Charts & table rendering
│ └─ ui_streamlit.py# Streamlit dashboard UI
├─ tests/ # Unit test files
├─ README.md # Project documentation
├─ pyproject.toml # Project configuration
└─ Dockerfile # Optional deployment file

## Install
git clone https://github.com/<your-github-username>/PyfinQuery.git
cd PyfinQuery
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

## Run
streamlit run finquery/ui_streamlit.py

## Test
pytest tests/

## Examples
"Show total expenses this month"
"Highest transaction last 30 days"
"Plot monthly spending trend"
"Group expenses by category"

## Tech
Python, Pandas, Streamlit, Matplotlib, AST, PyTest

## Notes
Works offline, safe execution, structured CSV input required

## Author
1. Khushan Pant
2. Veval Gupta
3. Shubhra Sarder
4. Sachin Negi
