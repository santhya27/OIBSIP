# RETAIL RADAR — EDA on Retail Sales Data

## 1) Install Python and Jupyter

1. Install Python 3 from https://www.python.org/downloads/ . During setup, tick **Add Python to PATH**.
2. Open Windows Command Prompt or PowerShell and verify:

   ```powershell
   py --version
   ```

3. Create a project environment (run these commands inside this project folder):

   ```powershell
   py -m venv .venv
   .venv\Scripts\activate
   python -m pip install --upgrade pip
   pip install jupyterlab notebook pandas numpy matplotlib seaborn
   ```

4. Launch JupyterLab:

   ```powershell
   jupyter lab
   ```

   Official Jupyter install instructions: https://jupyter.org/install

## 2) Add the dataset

This notebook expects `data/sales_data.csv`.

1. Open https://gist.github.com/summerofgeorge/33dbb09adbdea670c31ee2c4fc9f2617
2. Open `sales_data.csv` and click **Raw**.
3. Save the file as `sales_data.csv` inside this project's `data` folder.

The source labels this data as **simulated**. It includes product names, dates, quantities, unit prices, customer age, and customer gender. Mention this limitation in your report. Do not use it to make real-world claims about an actual retailer.

## 3) Run the notebook

1. In JupyterLab, open `Retail_Radar_EDA.ipynb`.
2. Choose the Python 3 kernel.
3. Run the cells from top to bottom (Shift+Enter).
4. When finished, use **Kernel → Restart Kernel and Run All Cells** to verify it runs cleanly.
5. Review the automatically generated chart observations and recommendations. Add or refine your own markdown notes based on the figures.

## 4) What it produces

- `outputs/retail_sales_cleaned.csv`
- `outputs/descriptive_statistics.csv`
- `outputs/monthly_sales.csv`
- `outputs/quarterly_sales.csv`
- `outputs/top_10_products_by_units.csv`
- `outputs/revenue_by_category.csv`
- `outputs/sales_by_age_group.csv`
- `outputs/sales_by_gender.csv`
- `outputs/executive_kpis.csv`
- Eight PNG charts under `outputs/figures/`

## 5) Checklist coverage

- Shape, columns, dtypes, missing values, duplicate rows — Sections 2–3
- Mean, median, mode, standard deviation — Section 5
- Monthly and quarterly sales line charts — Sections 6–7
- Age-group and gender distributions — Sections 8–9
- Top 10 products and category revenue — Sections 10–11
- Correlation heatmap — Section 12
- Additional Pareto/revenue-concentration visualisation — Section 13
- Observations after charts — Sections 6–13
- At least three evidence-based business recommendations — Section 15
- Conclusion and limitations — Section 17

## 6) If the CSV columns differ

The notebook maps several common column-name variants. It requires date, product name, quantity, unit price, customer age, and customer gender. A basic Kaggle Retail Sales Dataset with only `Product Category` cannot support a true top-10 individual-product ranking; choose a richer dataset rather than inventing product names.
