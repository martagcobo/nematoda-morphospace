# 3D Functional Morphospace Explorer: Marine Cave Nematodes

[![Paper Status](https://img.shields.io/badge/Paper-Under%20Peer%20Review-amber.svg)](https://github.com/)
[![Web App](https://img.shields.io/badge/Interactive%20Web-Live%20Explorer-0a9396.svg)](./index.html)
[![License](https://img.shields.io/badge/License-CC%20BY%204.0-blue.svg)](https://creativecommons.org/licenses/by/4.0/)

An interactive 3D web platform for exploring the functional morphospace, trait selection, and partitioned functional $\beta$-diversity of subterranean cave versus surface control marine nematode assemblages (*N* = 406 specimens).

This repository contains the interactive data visualization web application associated with the scientific manuscript:

> **"Are caves environmental filters for nematode body forms?"**  
> *Currently under peer review.*

---

## 🔬 Overview & Key Features

This explorer visualizes multi-trait functional morphospaces generated via block-weighted Gower dissimilarity matrices (`gawdis`) and Principal Coordinates Analysis (PCoA).

* **Interactive 3D Morphospace Visualization:**
  * Explore the first three orthogonal PCoA axes (retaining 47.6% of total functional variation).
  * Toggleable layers: Real Specimen Points (*N* = 406), 3D Alpha-Hull Boundary Meshes, and Gaussian Kernel Density Estimation (KDE) space.
  * Presets for standard views (Isometric 3D, PCoA 1 vs 2, PCoA 1 vs 3, PCoA 2 vs 3).
* **Regional Scope & Paired Locality Filtering:**
  * Dynamic filtering across four oceanic island and coastal cave systems: **Cozumel** (Mexico), **Madeira** (Portugal), **Selvagens** (Portugal), and **Tenerife** (Canary Islands, Spain).
* **Partitioned Functional $\beta$-Diversity Metrics:**
  * Real-time calculation of total functional dissimilarity ($B_{\text{total}}$), functional replacement/turnover ($B_{\text{repl}}$), and richness differences/nestedness ($B_{\text{rich}}$) using kernel density hypervolumes (`BAT` R package), along with Sørensen and Jaccard overlap indices.
* **Specimen-Level Trait Inspector & Anatomical Schema:**
  * Click any individual specimen point to inspect its morphometrics (body length, cephalic setae length, PCoA coordinates) and functional states across five key modules:
    1. **Sensory:** Amphid shape types.
    2. **Feeding Guild:** Buccal cavity morphology.
    3. **Pharyngeal Structure:** Bulb shape.
    4. **Body Wall:** Cuticle structure.
    5. **Locomotion & Attachment:** Tail shape.
  * Features a dynamic vector schematic of nematode anatomy highlighting individual trait locations.
* **Interactive Morphological Trait Gallery:**
  * Built-in modal gallery displaying high-resolution anatomical drawings for all categorical and qualitative trait states.

---

## 📁 Repository Structure

```text
.
├── index.html         # Main web application (HTML5, Tailwind CSS, Plotly.js, Lucide Icons)
├── img/               # Morphological trait drawings directory
│   ├── 1A.png         # Selective deposit feeder (Buccal cavity)
│   ├── 1B.png         # Non-selective deposit feeder (Buccal cavity)
│   ├── 2A.png         # Epistratum feeder (Buccal cavity)
│   ├── 2B.png         # Predator / Omnivore (Buccal cavity)
│   ├── extendedlips.png
│   ├── pore.png       # Inconspicuous / Pore amphid
│   ├── slit.png       # Longitudinal slit amphid
│   ├── circular.png   # Circular amphid
│   ├── criptospiral.png
│   ├── spiral.png
│   ├── unispiral.png
│   ├── pocket.png     # Pocket / Cup-shaped amphid
│   ├── vesicular.png
│   ├── photoreceptor.png
│   ├── smooth.png     # Smooth cuticle
│   ├── annulated.png  # Annulated cuticle
│   ├── punct.png      # Punctuated cuticle
│   ├── plates.png     # Cuticular plates
│   ├── swolen.png     # Indistinct / Slightly swollen pharyngeal bulb
│   ├── rounded.png    # Rounded bulb
│   ├── double.png     # Double bulb
│   ├── elongated.png  # Elongated bulb
│   ├── conical.png    # Conical tail
│   ├── shortrounded.png # Short & rounded tail
│   ├── clavated.png   # Clavate tail
│   └── filiform.png   # Elongated filiform tail
└── README.md          # Repository documentation
```

---

## 🚀 How to Run Locally

No server setup or dependencies installation is required.

1. Clone or download this repository:
   ```bash
   git clone https://github.com/your-username/nematode-morphospace.git
   ```
2. Ensure the `img/` folder is in the same directory as `index.html`.
3. Open `index.html` directly in any modern web browser (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari).

---

## 🌐 Online Deployment (GitHub Pages)

To host the interactive explorer online:

1. Push this repository to GitHub.
2. Go to **Settings > Pages** in your GitHub repository.
3. Under **Branch**, select `main` (or `master`) and folder `/ (root)`.
4. Click **Save**. Your interactive explorer will be published at `https://<your-username>.github.io/<repository-name>/`.

---

## 📖 How to Cite

If you use this visualization tool, dataset, or code in your research, please cite:

```text
[Authors]. (2026). Are caves environmental filters for nematode body forms? 
[Journal Name] (Under Peer Review).
```

*Note: Citation details, DOI, and journal reference will be updated upon formal manuscript publication.*

---

## 📄 License

This project and associated visualization data are licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).