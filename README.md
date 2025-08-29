# DEPRODATA Toolkit — Public Release

This repository provides a **public reproducibility package** derived from the private DEPRODATA Toolkit.  
It contains **minimal data, scripts, and documentation** to regenerate selected figures and metrics presented in related publications.  

⚠️ **Note:** This is *not* the full DEPRODATA Toolkit. The complete codebase remains private.  
The purpose of this repository is to ensure **academic transparency, citability, and reproducibility** of published results.

---

## Contents
- `data/` → minimal example datasets (CSV, XLSX, JSON).
- `scripts/` → lightweight Python scripts to regenerate example figures (PSD plots, radar plots).
- `figures/` → pre-generated example images.
- `CITATION.cff` → citation metadata.
- `.zenodo.json` → Zenodo metadata for DOI assignment.

---

## Citation
If you use material from this repository, please cite as:

**Espinosa, D. (2025). DEPRODATA Toolkit (Public Release). Zenodo. https://doi.org/10.5281/zenodo.XXXXXXX**

---

## License
This repository uses a **dual licensing scheme**:

- **Code (scripts/):** GNU General Public License v3.0 (GPLv3)  
- **Data & Figures (data/, figures/):** Creative Commons Attribution 4.0 International (CC BY 4.0)

---

## How to regenerate the figures
```bash
# Python 3.11+ recommended
pip install -r environment.txt

# Example commands:
python scripts/plot_radar_from_csv.py data/anchor_global_example.csv figures/example_radarplot.png
python scripts/make_psd_figures_from_xlsx.py data/psd_example.xlsx figures/example_psd.png
