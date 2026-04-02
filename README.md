# 📊 Comprehensive EDA Dashboard
*Exploratory Data Analysis Report Ecosystem for Tabular, Text, and Image Datasets*

This repository contains a full-stack, aesthetically elegant dashboard system that dynamically renders interactive analytical visualizations directly from Jupyter Notebook `.ipynb` outputs. It is deeply structured to provide **Academic Observations, Methodologies, and Interactive Data Views**.

## 🚀 Features
- **Multi-Modal Support:** Pre-configured analysis for `Tabular (Bank Telemarketing)`, `Text (AG News NLP)`, and `Image (ADE20K Semantic Segmentation)`.
- **Dynamic HTML Generator:** `notebook_to_dashboard_detailed.py` parses arbitrary Notebooks and extracts Plotly graphs, DataFrames, and PNGs directly into a high-end UI layout.
- **Academic Rigor:** Every generated chart is wrapped in an elegant glass-morphism container with auto-generated *What/Why/How* contextual bounds and Deep Insight summaries.
- **Native Plotly Support:** Retains 100% interactivity for scatter plots, histograms, heatmaps, and TF-IDF variance models.

---

## 🛠️ Installation & Setup

### 1. Dependencies
To execute the backend notebooks and regenerate the HTML dashboards, you need the following standard Data Science Python stack:

```bash
# Core Data pipelines & Plotting
pip install pandas numpy matplotlib plotly

# NLP & Text Analysis (For AG News)
pip install scikit-learn nltk kagglehub

# Computer Vision & Segmentation (For ADE20K)
pip install opencv-python pillow datasets
```

### 2. How to Regenerate the Dashboards
If you ever modify the python code inside the `.ipynb` files (e.g. running new models or plotting new charts), you can rebuild the beautiful web interface with a single command:
```bash
python3 notebook_to_dashboard_detailed.py
```
*Note: This script will recursively scan `text_data.ipynb` and `image_data.ipynb`, stripping out raw JSON Plotly graphs and embedding them into the beautiful UI blocks seen in `eda_report_v2.html`.*

### 3. Viewing the Reports
The dashboards are purely static `HTML/CSS/JS`. No heavy backend is required.
You can view the site locally by running a simple HTTP server:
```bash
python3 -m http.server 8000
```
Then, open your browser and navigate to: [http://localhost:8000](http://localhost:8000)

---

## 📂 Project Structure
```text
.
├── index.html                           # Landing Page bridging all reports
├── notebook_to_dashboard_detailed.py    # The Core Dashboard UI Generator 
├── tabular/                             
│   └── eda_report_v2.html               # Reference Master Tabular Report
├── text/                                
│   ├── text_data.ipynb                  # Raw NLP Model Executions
│   └── eda_report_v2.html               # Auto-Generated Text Dashboard
└── image/                               
    ├── image_data.ipynb                 # CV / Mask Overlay Executions
    └── eda_report_v2.html               # Auto-Generated Image Dashboard
```

## 📝 Design Philosophy
The UI was meticulously handcrafted to overcome the standard flat, boring layout of `Jupyter nbconvert`. It isolates overlapping numerical matrices, provides glowing neon bounds, embeds detailed academic context summaries, and retains full responsive behavior. This ensures the output is always "Presentation Ready" for academic reviewers and stakeholders.
