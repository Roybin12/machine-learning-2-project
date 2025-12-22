# NYC Traffic Collisions: Predicting Vulnerable Road User Type

**Students:** רועי בנימיני, עוז ניסנבוים

**Course:** Data Mining 2025

---

## 🎯 Project Goal

Predict whether a traffic collision involving a vulnerable road user (VRU) is a **pedestrian** or **cyclist** incident, using machine learning classification techniques.

---

## 📊 Dataset

- **Source:** [NYC Open Data - Motor Vehicle Collisions](https://catalog.data.gov/dataset/motor-vehicle-collisions-crashes)
- **Original Size:** 2.2M+ collision records
- **VRU Sample:** Pre-filtered dataset containing only pedestrian/cyclist collisions
- **Features:** Temporal, geographic, vehicle type, contributing factors

---

## 🛠️ Methods

### Supervised Learning (5 Models)
| Model | Accuracy | ROC-AUC |
|-------|----------|---------|
| Logistic Regression | 70.6% | 0.635 |
| Decision Tree | 65.2% | 0.615 |
| Random Forest | 73.8% | 0.754 |
| **XGBoost (Best)** | **75.4%** | **0.778** |
| Neural Network (MLP) | 73.4% | 0.736 |

### Unsupervised Learning
- **K-Means Clustering:** Identified 5 geographic collision hotspots
- **Isolation Forest:** Detected anomalous collision patterns

---

## 📁 Repository Structure
```
├── ML2.ipynb                  # Main analysis notebook
├── Sampling.ipynb             # Data sampling/filtering notebook
├── VRU_Crashes_Sample.zip     # Pre-filtered VRU collision data
├── geocoded_locations.csv     # Google Maps API geocoded coordinates
├── nyc_collisions_map.html    # Interactive map visualization
├── requirements.txt           # Python dependencies
├── archive/                   # Previous versions
└── README.md                  # This file
```

---

## 🚀 Quick Start

1. **Clone the repository:**
```bash
   git clone https://github.com/Roybin12/machine-learning-2-project.git
   cd machine-learning-2-project
```

2. **Install dependencies:**
```bash
   pip install -r requirements.txt
```

3. **Run the notebook:**
```bash
   jupyter notebook ML2.ipynb
```

---

## 📈 Key Findings

1. **Vehicle Type** is the strongest predictor (42.5% importance)
2. **Manhattan** has the highest cyclist collision rate (42.1%)
3. **Staten Island** has the lowest cyclist rate (16.3%)
4. **Anomalies** occur mainly at midnight on weekends

---

## 🔧 Technologies Used

- Python 3.9+
- Pandas, NumPy
- Scikit-learn, XGBoost
- Matplotlib, Seaborn
- Folium (Interactive Maps)
- Google Maps Geocoding API

---

## 🤖 AI Tools Disclosure

This project utilized the following AI tools for development assistance:
- **Claude Opus 4.5** (Anthropic) - Code development and debugging
- **Google Gemini 3** (Google) - Research and analysis support

---

## 📄 License

This project is for educational purposes as part of the Data Mining course.
