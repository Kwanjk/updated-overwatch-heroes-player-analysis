# 🏹 **We Are Who We Lock: Overwatch Hero Psychology & Archetype Analysis**

*A Data Science Project for INST414 – Fall 2025*
**Author:** Joshua Kwan

---

## 📌 **Project Overview**

This project extends my module-level Medium post *“We Are Who We Lock: A Similarity Study of Overwatch Heroes & Player Psychology”* into a full multi-method data science analysis combining:

* **Cosine similarity** (network science)
* **Dimensionality reduction (PCA)**
* **Unsupervised learning (K-Means clustering)**
* **Evaluation metrics (silhouette score)**
* **Feature scaling, visualization, and interpretability techniques**

The goal of this project is to answer a central question:

> **Do Overwatch heroes naturally form psychological archetypes—and can these archetypes help players find heroes that match their natural playstyle?**

This repository contains all source code, datasets, charts, and analysis used to build the final Medium article.

---

## 🎯 **Motivation**

Players often gravitate toward specific heroes—mobile duelists, precision snipers, utility supports, or tanky frontline anchors.

This project attempts to **quantify playstyle archetypes** using hero attribute data and modern data science methods.
The insights help:

* **New players** discover heroes aligned with their instincts
* **Intermediate players** understand their strengths and expand their roster
* **Analysts** visualize the hero ecosystem in a psychological feature space

---

## 📁 **Repository Structure**

```
.
├── data/
│   ├── overwatch_hero_psychology_full.csv
│   ├── overwatch_full_similarity_top5.csv
│   ├── overwatch_hero_archetypes.csv
│   └── (any additional processed outputs)
│
├── notebooks/
│   ├── overwatch_hero_archetype_analysis_final.ipynb
│   └── (archived drafts)
│
├── images/
│   ├── pca_plot.png
│   ├── similarity_heatmap.png
│   ├── cluster_radar_charts.png
│   ├── parallel_coordinates.png
│   └── (other exported visuals)
│
├── README.md   ← You are here
└── requirements.txt (optional)
```

---

## 📊 **Methods Used**

### 🔹 **1. Cosine Similarity**

Used to construct a 45×45 psychological similarity matrix between all heroes.

### 🔹 **2. PCA (Principal Component Analysis)**

Reduces 4D hero features → 2D “hero psychology map.”

### 🔹 **3. K-Means Clustering**

Finds latent archetypes independent of hero role:

* **Skirmishers**
* **Tacticians**
* **Anchors**
* **Sharpshooters**

Validated with silhouette scoring.

### 🔹 **4. Visualizations**

Includes:

* PCA hero map
* Cosine similarity heatmap
* Radar charts (archetype profiles)
* Parallel coordinate plots
* Role distribution across clusters

---

## 🧪 **How to Run**

### **1. Clone the repository**

```
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

### **2. Install dependencies**

You can manually install or use a requirements file.

```
pip install pandas numpy matplotlib seaborn scikit-learn
```

### **3. Open the analysis notebook**

```
jupyter notebook notebooks/overwatch_hero_archetype_analysis_final.ipynb
```

### **4. Run all cells**

The notebook will:

* Load the dataset
* Scale and preprocess features
* Compute PCA and cosine similarity
* Perform clustering
* Output all figures and CSV files

---

## 📈 **Key Outputs**

### ✔ **Archetype Assignments**

File: `overwatch_hero_archetypes.csv`
Maps: Hero → Role → Cluster → Archetype name

### ✔ **Top-5 Similar Heroes per Hero**

File: `overwatch_full_similarity_top5.csv`

### ✔ **PCA 2D Hero Map**

Shows how heroes cluster organically in playstyle space.

### ✔ **Final Radar Charts**

Visual fingerprints of each archetype.

---

## 🧹 **Data Cleaning & Bugs to Avoid**

This project included:

* Normalizing numeric features
* Adjusting HP scale for comparability
* Ensuring consistent column naming
* Re-checking new heroes (Hazard, Vendetta, Juno, etc.)

Common pitfalls others may run into:

* Forgetting to scale HP → breaks PCA
* Missing a hero in one-hot encoding → misaligns clustering
* Typos in dictionary → breaks DataFrame creation
* Using unscaled data in K-Means → distort clusters

---

## 🤖 **AI Assistance Statement**

ChatGPT was used for:

* Debugging code
* Improving visualization aesthetics
* Structuring the Medium article
* Generating descriptive labels and archetype names
* Ensuring scalability of the pipeline

All outputs were carefully checked, corrected, and validated manually for accuracy.

---

## 📜 **Final Medium Article**

🔗 **Medium Link:**
*Insert Medium article URL here once published.*

This article contains the full narrative, explanations, and charts used to communicate the results.

---

## ⚠️ **Limitations & Ethics**

* Hero stat ratings are semi-subjective
* Patch changes may alter hero profiles
* PCA reduces complexity at the cost of nuance
* K-Means assumes spherical clusters (may oversimplify)
* No user gameplay data analyzed (privacy preserved)

Players should use this as **guidance**, not strict categorization.

---

## 🏁 **Conclusion**

This project demonstrates that Overwatch heroes naturally separate into statistically meaningful playstyle archetypes, reflecting real psychological differences in how players approach the game.

These archetypes help players:

* Better understand their strengths
* Explore new heroes confidently
* Build wider, more intuitive hero pools
* Reflect on their personal playstyle identity

Ultimately:
**We really are who we lock.**

---

## 📬 **Contact**

Feel free to reach out if you want to collaborate, provide feedback, or build on this project!

**Author:** Joshua Kwan
**Email:** (optional)

---

If you'd like, I can also generate:

✔ A polished **requirements.txt**
✔ A matching **LICENSE file**
✔ A banner image for the repo
✔ A short project description for your GitHub sidebar

Just say **“add requirements.txt”** or **“create license”** and I’ll generate it.
