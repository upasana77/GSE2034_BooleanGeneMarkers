# GSE2034_BooleanGeneMarkers
Boolean analysis of gene expression data from GSE2034 for breast cancer relapse markers”
# 🧬 Boolean Analysis of Gene Expression in Breast Cancer (GSE2034)

This project applies Boolean logic to gene expression data to identify marker genes associated with bone relapse in breast cancer patients. Inspired by the work of Dr. Debashis Sahoo’s lab, this notebook demonstrates how binary gene activity can reveal significant biological patterns.

## 📦 Dataset
- **Source**: [GEO: GSE2034](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE2034)
- **Platform**: Affymetrix Human Genome U133A Array
- **Samples**: 286 breast cancer patients with relapse metadata

## 🧰 Tools & Libraries
- `pandas`, `numpy`
- `seaborn`, `matplotlib`
- `gseapy` (for enrichment analysis)
- Jupyter Notebook (for step-by-step coding)

## 🚀 Project Workflow

1. 🔓 **Data Extraction**  
   - Decompressed `.txt.gz` GEO matrix  
   - Loaded gene expression values (rows = genes, columns = patients)

2. 🔄 **Boolean Conversion**  
   - Converted gene expression to binary ON/OFF using gene-wise median thresholds

3. 🧪 **Clinical Grouping**  
   - Extracted bone relapse metadata  
   - Labeled samples into “Relapse” vs. “No Relapse”

4. 🎯 **Marker Gene Discovery**  
   - Selected genes ON in ≥60% of relapse & OFF in ≥60% of no-relapse patients  
   - Also tested stricter 80%/20% criteria

5. 🧬 **Pathway Enrichment (KEGG)**  
   - Mapped gene symbols  
   - Identified enriched biological pathways via gseapy

6. 📊 **Visualization**  
   - Heatmaps for ON/OFF gene activity  
   - Bar plots of enriched pathways

## 🔍 Key Findings
- Marker genes with distinct ON/OFF patterns in relapse vs. no-relapse
- Top enriched pathways:
  - Prion Disease
  - Estrogen Signaling
  - Oxidative Phosphorylation
  - Parkinson’s Disease

## 📁 Repository Contents
| File                          | Description                             |
|------------------------------|-----------------------------------------|
| `GSE2034_BooleanAnalysis.ipynb` | Main annotated notebook                  |
| `GSE2034_BooleanAnalysis.html`  | Optional HTML version for quick preview |
| `requirements.txt`           | List of required Python packages        |

## 🧠 About the Author
Prepared by **Upasana Purohit**, aspiring PhD candidate in Bioinformatics.  
Passionate about applying computational methods to uncover hidden patterns in cancer biology.


- 📧 your.email@example.com

> ⚠️ *This project is part of an independent learning journey and is inspired by Boolean lab principles from Dr. Debashis Sahoo.*
