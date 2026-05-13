### 1. XBP1 vs GATA3 Scatter Plot

Creates a scatter plot showing expression levels of:

* XBP1
* GATA3

Each point represents one patient.

Color indicates:

* `0` → ER-
* `1` → ER+

---

### 2. PCA Clustering

Performs:

* Standardization of gene expression data
* PCA dimensionality reduction
* 2D visualization of patient clustering

Outputs:

* PC1 variance explained
* PC2 variance explained

---

## Requirements

Install the required Python libraries before running the script.

### Install Dependencies

```bash
pip install pandas matplotlib scikit-learn
```

---

## How to Run

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

---

### Step 2: Add Dataset Files

Place the following files inside the project directory:

* `filtered.tsv.gz`
* `class.tsv`
* `columns.tsv.gz`

---

### Step 3: Run the Script

```bash
python analysis.py
```

---

## Output

The script generates:

### Scatter Plot

Saved as:

```bash
scatter_plot.png
```

### PCA Plot

Saved as:

```bash
pca_plot_final.png
```

Console output example:

```bash
PCA complete. PC1 explains 32.45% of the variance.
```

---

## Dataset Description

| File              | Description                       |
| ----------------- | --------------------------------- |
| `filtered.tsv.gz` | Gene expression matrix            |
| `class.tsv`       | Patient labels (ER-/ER+)          |
| `columns.tsv.gz`  | Mapping of Gene IDs to Gene Names |

---

## Technologies Used

* Python
* Pandas
* Matplotlib
* Scikit-learn

---

## Notes

* Ensure all dataset files are present before running the script.
* Standardization is important before PCA for biological datasets.
* The script automatically identifies Gene IDs for:

  * `XBP1`
  * `GATA3`

---

## License

This project is open-source and available under the MIT License.

```
