# 3D Functional Morphospace Explorer: Marine Cave Nematodes

> 🌐 **Live Interactive Visualizer:**  
> **[https://martagcobo.github.io/nematoda-morphospace/](https://martagcobo.github.io/nematoda-morphospace/)**

An interactive 3D web platform for exploring the functional morphospace, trait selection, and partitioned functional $\beta$-diversity of subterranean cave versus surface control marine nematode assemblages (*N* = 406 specimens).

This repository contains the interactive data visualization web application associated with the scientific manuscript:

> **"Are caves environmental filters for nematode body forms?"**  
> *Currently under peer review.*

---

## 🌐 Quick Access

You can access and interact with the full 3D visualizer directly in your web browser without downloading any files:
👉 **[Open Interactive Visualizer](https://martagcobo.github.io/nematoda-morphospace/)**

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

```
.
├── index.html         # Main web application (HTML5, Tailwind CSS, Plotly.js, Lucide Icons)
├── img/               # Morphological trait drawings directory
│   ├── 1A.png        
│   ├── 1B.png         
│   ├── 2A.png         
│   ├── 2B.png         
│   ├── extendedlips.png
│   ├── pore.png       
│   ├── slit.png      
│   ├── circular.png   
│   ├── criptospiral.png
│   ├── spiral.png
│   ├── unispiral.png
│   ├── pocket.png     
│   ├── vesicular.png
│   ├── photoreceptor.png
│   ├── smooth.png   
│   ├── annulated.png  
│   ├── punct.png     
│   ├── plates.png     
│   ├── swolen.png   
│   ├── rounded.png    
│   ├── double.png     
│   ├── elongated.png  
│   ├── conical.png   
│   ├── shortrounded.png 
│   ├── clavated.png   
│   └── filiform.png  
└── README.md          
```

---

## 🚀 How to Run Locally

If you prefer to run the visualization offline:

1. Clone or download this repository:
   ```bash
   git clone https://github.com/martagcobo/nematoda-morphospace.git
   ```
2. Ensure the `img/` folder is in the same directory as `index.html`.
3. Double-click `index.html` to open it in any web browser.

---


## 📄 License

This project and associated visualization data are licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
