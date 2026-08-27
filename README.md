# MoMA Cultural Heritage & Curation Dynamics (1929–2025)

An advanced exploratory data analysis and editorial visual study examining the institutional growth, curatorial shifts, and acquisition velocity of the Museum of Modern Art (MoMA) Open Access Collection.

---

## 🎨 Design Philosophy & Visual Aesthetic

Crafted with a dark-mode editorial aesthetic (`#121212` background, minimalist typographic hierarchies, and high-contrast luxury accents like metallic gold `#d0ab4d` and electric purple `#a259ff`), this project transitions away from standard data science templates toward publication-grade visual storytelling.

![Dashboard Preview](https://github.com/BenWam254/moma-cultural-heritage-eda/blob/main/assets/moma_curation_dashboard.png?raw=true)

---

## 📊 Key Analytical Insights

* **The Late 1960s Acquisition Surge**: Unveils an unprecedented institutional expansion spike between 1965 and 1970, propelled heavily by massive inflows in Drawings & Prints and Architecture & Design collections.
* **Decadal Curatorial Evolution**: Highlights the structural transition from traditional fine art media dominance toward contemporary classifications, architectural archives, and photography.
* **Compounding Scale**: Traces a steep cumulative collection growth curve, documenting the threshold breakthrough past 150,000 catalogued works.

---

## ⚙️ Technical Architecture & Pipeline

* **Core Language**: Python 3.12
* **Data Ecosystem**: Pandas, NumPy, Matplotlib, Seaborn
* **Ingestion Engineering**: Overcame GitHub Large File Storage (LFS) pointer barriers by utilizing direct media endpoints (`raw.githubusercontent.com`) for seamless loading of raw 70MB+ Artworks and Artists datasets.
* **Feature Engineering**:
  * Standardized unstructured datetime strings into clean `AcquisitionYear` temporal coordinates.
  * Extracted structured 4-digit creation years using robust regular expression pattern matching (`CleanYear`).
  * Applied 3-year and 5-year rolling averages to smooth institutional acquisition volatility.

---

## 🚀 Getting Started (GitHub Codespaces)

This project is fully configured to run directly in your browser via GitHub Codespaces without requiring any local environment setup:

1. Navigate to the main repository page on GitHub.
2. Click the green **Code** button, select the **Codespaces** tab, and click **Create codespace on main**.
3. Once the cloud environment initializes, open the notebook from the terminal or file tree:
   ```bash
   jupyter notebook notebooks/moma_cultural_heritage_eda.ipynb
