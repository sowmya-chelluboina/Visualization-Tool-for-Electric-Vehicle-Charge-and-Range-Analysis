#!/bin/bash

# ======================================================
# ⚡ EV Charge & Range Visualization - Complete Setup
# ======================================================

set -e

PROJECT_NAME="EV-Charge-Range-Visualization"

echo "🚀 Creating project: $PROJECT_NAME"

# 1️⃣ Create Project Structure
mkdir -p $PROJECT_NAME/{data,src,dashboard,images}
cd $PROJECT_NAME

# 2️⃣ Create Virtual Environment
echo "🐍 Setting up virtual environment..."
python3 -m venv venv
source venv/bin/activate

# 3️⃣ Upgrade pip
pip install --upgrade pip

# 4️⃣ Install Dependencies
echo "📦 Installing dependencies..."
pip install pandas numpy matplotlib seaborn plotly streamlit

# 5️⃣ Save requirements.txt
pip freeze > requirements.txt

# 6️⃣ Create Sample Dataset
echo "📊 Creating sample dataset..."
cat <<EOF > data/ev_dataset.csv
battery_capacity_kwh,soc_percent,consumption_kwh_per_km
60,80,0.15
75,65,0.18
50,90,0.14
85,40,0.20
100,55,0.17
EOF

# 7️⃣ Create Data Processing Script
echo "⚙ Creating data processing module..."
cat <<EOF > src/data_processing.py
import pandas as pd

def load_data(path):
    return pd.read_csv(path)

def calculate_range(df):
    df["estimated_range_km"] = (
        (df["soc_percent"] / 100) *
        df["battery_capacity_kwh"] /
        df["consumption_kwh_per_km"]
    )
    return df
EOF

# 8️⃣ Create Streamlit Dashboard
echo "🖥 Creating Streamlit dashboard..."
cat <<EOF > dashboard/app.py
import streamlit as st
import sys
import os

sys.path.append(os.path.abspath("../src"))

from data_processing import load_data, calculate_range
import plotly.express as px

st.set_page_config(page_title="EV Charge & Range Tool", layout="wide")

st.title("⚡ Electric Vehicle Charge & Range Visualization")

data_path = "../data/ev_dataset.csv"

df = load_data(data_path)
df = calculate_range(df)

st.subheader("📊 EV Dataset")
st.dataframe(df)

st.subheader("📈 Estimated Range vs State of Charge")

fig = px.scatter(
    df,
    x="soc_percent",
    y="estimated_range_km",
    size="battery_capacity_kwh",
    color="battery_capacity_kwh",
    hover_data=["consumption_kwh_per_km"],
    labels={
        "soc_percent": "State of Charge (%)",
        "estimated_range_km": "Estimated Range (km)"
    }
)

st.plotly_chart(fig, use_container_width=True)

st.success("✅ Visualization Generated Successfully")
EOF

# 9️⃣ Create .gitignore
echo "📝 Creating .gitignore..."
cat <<EOF > .gitignore
venv/
__pycache__/
*.pyc
.DS_Store
EOF

# 🔟 Create README.md
echo "📘 Creating README.md..."
cat <<EOF > README.md
# ⚡ EV Charge & Range Visualization Tool

This project visualizes Electric Vehicle battery charge levels and estimated driving range.

## Features
- Battery State of Charge analysis
- Range estimation
- Interactive dashboard (Streamlit)
- Data processing module

## Run the Project

\`\`\`bash
source venv/bin/activate
streamlit run dashboard/app.py
\`\`\`

## Formula Used

Estimated Range (km) =  
(SOC % / 100) × Battery Capacity (kWh) ÷ Consumption (kWh/km)
EOF

echo ""
echo "✅ Project setup complete!"
echo ""
echo "📂 Navigate into project:"
echo "cd $PROJECT_NAME"
echo ""
echo "▶ To run the dashboard:"
echo "source venv/bin/activate"
echo "streamlit run dashboard/app.py"
echo ""
echo "🌐 Streamlit will open in your browser automatically."
