# 🩺 PulseScore: Healthcare Operation Dashboard
### Infosys Springboard Internship Project

[![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white)](https://streamlit.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

A production-grade healthcare analytics platform for monitoring India's healthcare infrastructure capacity, resource distribution, and surge readiness using WHO-benchmarked standards.

---

## 📸 Screenshots

| **Dashboard Overview** | **National Snapshot** |
|:---:|:---:|
| ![Dashboard](https://via.placeholder.com/800x450.png?text=PulseScore+Dashboard+Overview) | ![Snapshot](https://via.placeholder.com/800x450.png?text=National+Snapshot+Analytics) |

---

## 🚀 Core Modules

### 1. National Snapshot
*   Executive KPI dashboard (Beds, Doctors, Population, ICU/Emergency coverage).
*   Interactive choropleth map with population density hotspots.
*   Healthcare resource ratios (Doctors/10K, Beds/100K) with regional capacity rankings.

### 2. Structural Gap Diagnosis
*   WHO-benchmarked capacity requirement mapping.
*   **Weighted Structural Deficit Score (SDS)**:
    *   40% Bed Deficit | 30% Doctor Deficit | 20% ICU Deficit | 10% Emergency Deficit.
*   Comparative analysis of the most deficient vs. strongest states.

### 3. Resource Distribution
*   District-level granularity for Bed, ICU, and Emergency facility analysis.
*   Doctor-to-bed ratio benchmarks.
*   Care hierarchy distribution (Primary vs. Secondary vs. Tertiary).

### 4. Surge Risk Intelligence (SRI)
*   Dynamic Surge Risk Index (SRI) calculation based on demand elasticity.
*   Adjustable surge multipliers (1.0x - 3.0x load stress).
*   State & District risk rankings for emergency preparedness.

### 5. Hospital Finder
*   GPS-based radius search for nearest facilities.
*   Search by Pincode, District, or Coordinates.

---

## 🛠️ Tech Stack

- **Frontend**: Streamlit (Premium UI with Dark/Light mode support)
- **Visualization**: Plotly, Kaleido
- **Data Engineering**: Pandas, NumPy
- **Geospatial**: Geopy, GeoJSON mapping
- **Reporting**: FPDF2 (Automated PDF Intelligence Reports)

---

## 📂 Project Structure

```text
Healthcare Operation Dashboard/
├── app.py                     # Main Entry Point
├── requirements.txt           # Dependency Manifest
├── logic/
│   └── core.py                # Analytical Engine & PDF Utilities
├── sections/
│   ├── snapshot.py            # National Overview Module
│   ├── structural_gaps.py     # Deficit Diagnosis Module
│   ├── resource_distribution.py # Resource Density Module
│   ├── surge_intelligence.py  # Surge Modeling Engine
│   └── hospital_finder.py    # Geospatial Finder Module
├── dataset/                   # Master Healthcare Datasets
└── geojson/                   # India State & District Level Map Data
```

---

## 📊 Methodology (WHO Benchmarks)

PulseScore operates on standardized global health metrics:
- **Required Beds**: (Population × 3) / 1,000
- **Required Doctors**: (Population × 1) / 1,000
- **SRI Formula**: $0.4 \times Stress_B + 0.3 \times Stress_D + 0.2 \times Stress_I + 0.1 \times Stress_E$

**Risk Classification:**
- 🟢 **< 1.0**: Stable
- 🟡 **1.0 - 1.2**: Saturated
- 🟠 **1.2 - 1.5**: High Risk
- 🔴 **> 1.5**: Critical (Active Failure)

---

## 📦 Installation & Usage

1. **Clone the Repo:**
   ```bash
   git clone https://github.com/yourusername/pulsescore.git
   cd pulsescore
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Launch the Dashboard:**
   ```bash
   streamlit run app.py
   ```

---

## 🎓 Internship Highlights
*   **Program**: Infosys Springboard Internship
*   **Domain**: Healthcare Infrastructure & Predictive Modeling
*   **Achievement**: Built a comprehensive decision-intelligence framework covering 36 States/UTs and 700+ Districts.

---

## 📄 License
Distributed under the MIT License. See `LICENSE` for more information.

---
*Built as part of the Infosys Springboard Internship 2026.*
