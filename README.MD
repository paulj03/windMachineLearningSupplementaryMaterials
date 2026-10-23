# Wind Machine Learning Supplementary Materials

Supplementary materials, datasets, and visualizations for wind machine learning models and data analysis.

## 📂 Repository Contents

This repository contains the following supplementary data and source files:

*   **`AWS _Bokwang_Station_Information.txt`** — Station information details for the Bokwang Automatic Weather Station (AWS).
*   **`aws2data.tgz`** / **`ICEPOP2018_Bokwang_nonDQ_AWS2_Data.csv`** — Complete weather datasets from the ICEPOP 2018 campaign (managed via Git LFS).
*   **`ICEPOP_WSS_Event_Feb11-13_topoMap_AWS_theta.mp4`** — Topographical visualization map video of the Winter Scientific Sepang (WSS) event spanning February 11–13.
*   **`movie.tgz`** — Additional packaged visualization materials and frames.
*   **`readme.txt`** — Original structural overview text file.

---

## 🛠️ Installation & Setup

### 1. Prerequisites
Ensure you have standard Git installed. Because this repository utilizes **Git Large File Storage (LFS)** to version files larger than 100 MB (such as the raw CSV dataset), you must install Git LFS before cloning to pull the complete data.

*   **Mac (Homebrew):** `brew install git-lfs`
*   **Windows / Linux:** Download from [://github.com](https://://github.com)

### 2. Cloning the Repository
Clone the repository and initialize Git LFS to pull down all pointers and deep datasets automatically:

```bash
# Clone the repository
git clone https://github.com

# Navigate into the folder
cd windMachineLearningSupplementaryMaterials

# Pull down the large LFS data objects
git lfs pull
```

---

## 🔬 Dataset Overview
The primary data originates from the **ICEPOP 2018** campaign (International Collaborative Experiments for Pyeongchang 2018 Olympic and Paralympic Winter Games), focusing on high-resolution meteorological configurations, specific topographical structures, and wind event observations around the Bokwang station. 

---

## 🤖 Usage in Machine Learning
To use the compressed features or the extracted `.csv` dataset in your local Python environment:

```python
import pandas as pd
import tarfile

# Example: Extracting data if working directly from the tgz archive
# with tarfile.open("aws2data.tgz", "r:gz") as tar:
#     tar.extractall()

# Loading the primary dataset
df = pd.read_csv("ICEPOP2018_Bokwang_nonDQ_AWS2_Data.csv")
print(df.head())
```

---



## ✉️ Contact & Citation
For inquiries regarding the machine learning methodologies or dataset parameters, please open an issue in this repository or contact the administrator via GitHub profile options.