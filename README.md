
# 🌍 World Population Analysis

This repository provides an exploratory analysis of world population data, focusing on trends over time, regional and income group distributions, and visualizations through Python and Power BI.

---

## 📁 File Structure

- **`World_Population_analysis.ipynb`**: A Jupyter notebook for data cleaning, transformation, and exploratory analysis.
- **`World_Population_analysis.pbix`**: A Power BI dashboard with interactive visualizations.
- **`total_cleaned.csv`**: The cleaned dataset used for analysis.
- **`README.md`**: Documentation for the repository (this file).

---

## 🛠️ Features and Steps
## 🧩 Code Explanation

### Python Script: `world_population_analysis.pynb`

1. **Importing Libraries**:
   - `numpy` and `pandas` for data manipulation.
   - `google.colab` for file operations in Google Colab.

2. **Data Loading**:
   - The script mounts Google Drive and uploads `total_population.csv` to Colab.

3. **Initial Data Inspection**:
   - Displays the structure of the population and metadata datasets using `.head()` and `.info()`.

4. **Data Cleaning**:
   - Removes redundant columns like `Indicator Name`, `Indicator Code`, and `2023` in the population data.
   - Drops `SpecialNotes` from the metadata.
   - Handles missing values by removing rows with NaN values.

5. **Merging and Renaming**:
   - Combines population and metadata datasets using a common key, `Country Code`.
   - Renames columns for consistency (e.g., `IncomeGroup` → `Income`).

6. **Data Transformation**:
   - Converts the dataset into long-format using the `.melt()` function.
   - Creates a column for `Year` and another for `Population`.

7. **Exporting Cleaned Data**:
   - Saves intermediate and final cleaned datasets (`new01.csv` and `new02.csv`) to Google Drive for further analysis.

### 🌐 Hosted Links
- **Colab Notebook**: [Run on Google Colab](https://colab.research.google.com/drive/1zvfX0bbzHFWaSU_TAv0mL99SpjqEfDdf?usp=sharing)

---

## 📦 How to Clone and Run the Repository

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/adityarathore622/World-Population-Analysis.git
   ```
2. **Navigate to the Repository**:
   ```bash
   cd World-Population-Analysis
   ```
3. **Run the Notebook**:
   - Open the `World_Population_analysis.ipynb` file in Jupyter Notebook or Google Colab.
   - Ensure dependencies like `pandas` and `numpy` are installed.
   - Use the Colab link for a ready-to-run environment.

4. **Power BI Analysis**:
   - Open `World_Population_analysis.pbix` in Power BI Desktop to explore visualizations.

---
## 🗂️ Repository Content

```
World-Population-Analysis/
├── README.md
├── World_Population_analysis.pbix
├── World_Population_analysis.ipynb
└── total_cleaned.csv
```

## 👨‍💻 Author

- **Aditya Rathore**  
  GitHub: [adityarathore622](https://github.com/adityarathore622)

---


✨ Happy exploring global population data! 🚀
