# ⚡ EV Charge & Range Visualization Tool  

Welcome to **EV Charge & Range Visualization Tool**, an interactive application designed to help users analyze electric vehicle (EV) charging patterns, battery efficiency, and estimated driving range.  

This tool supports **Streamlit** deployment for quick, interactive data exploration, and can also be run locally for custom datasets.  

---

## 📌 Features  

| Feature | Description |
|---------|------------|
| **Battery Charge Analysis** | Visualize battery levels across trips and sessions |
| **Range Estimation** | Estimate vehicle range based on battery state |
| **Charging Session Visualization** | Explore charging efficiency and patterns |
| **Data-driven Insights** | Track historical performance trends |
| **Interactive Dashboards** | Dynamic charts and plots using Streamlit |

---

## 🎥 Demo  

Here’s a preview of the interactive dashboards:  

![App Demo](assets/demo.png)  

---

## 📂 Project Structure  

```text id="f0j2yt"
ev-charge-range-visualization/
│── app.py                 # Main Streamlit application
│── requirements.txt       # Python dependencies
│── data/                  # Sample datasets (CSV)
│── assets/                # Images, charts, and demo GIFs
│── README.md
│── LICENSE


🖥️ Run Locally

Clone the repository and navigate into the project folder:
# Clone repository
git clone :https://github.com/sowmya-chelluboina/Visualization-Tool-for-Electric-Vehicle-Charge-and-Range-Analysis.git
cd ev-charge-range-visualization

# Create virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows

# Install dependencies
pip install -r requirements.txt

# Run the Streamlit app
streamlit run app.py

🚀 Deployment Guide
Streamlit Cloud

Sign in at Streamlit Cloud

Create a New App

Connect your GitHub repository and select the folder containing app.py

Streamlit Cloud will install dependencies and deploy your app automatically

The live app link will appear in your Streamlit dashboard

🛠️ Tech Stack

Python 3.8+ – Core programming language

Streamlit – Interactive visualization and dashboards

Pandas & NumPy – Data manipulation and analysis

Matplotlib, Seaborn & Plotly – Charts and plotting

CSV / Data Files – Input structured EV datasets

📜 License

This project is licensed under the MIT License – see the LICENSE
 file for details.

⭐ Support

If you find this tool useful, consider giving it a ⭐ on GitH
