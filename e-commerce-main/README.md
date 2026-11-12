# E-Commerce Data Insights

A data analytics project exploring Amazon India order records to understand sales patterns, product mix, fulfilment, delivery status, and customer geography. The repository includes an exported Power BI report, its editable `.pbix` file, a Jupyter notebook, and a responsive animated project showcase.

> **Project type:** Analytics and dashboard portfolio project — not a live ecommerce storefront or order-processing service.

## Project highlights

- **128,975 transaction records** and 24 fields are shown in the notebook's dataset inspection.
- Explore order status, fulfilment method, sales channel, category, size, shipping service, and delivery geography.
- Review the exported Power BI report in HTML or open the editable Power BI Desktop file.
- Use the notebook to inspect and analyze the data with Python and pandas.
- A responsive project page features subtle motion, animated chart accents, and reduced-motion support.

## Project contents

| Path | Description |
| --- | --- |
| [`index.html`](index.html) | Animated, responsive project landing page and dashboard overview. |
| [`E-Commerece Data analysis/E-commerce.html`](E-Commerece%20Data%20analysis/E-commerce.html) | Exported HTML report. |
| [`E-Commerece Data analysis/E-Commerce.pbix`](E-Commerece%20Data%20analysis/E-Commerce.pbix) | Power BI report source; open with Power BI Desktop. |
| [`E-Commerece Data analysis/E-commerce.ipynb`](E-Commerece%20Data%20analysis/E-commerce.ipynb) | Jupyter notebook for data inspection and analysis. |
| [`E-Commerece Data analysis/Screenshot 2025-09-01 180243.png`](E-Commerece%20Data%20analysis/Screenshot%202025-09-01%20180243.png) | Dashboard screenshot. |
| [`E-Commerece Data analysis/Screenshot 2025-09-01 180912.png`](E-Commerece%20Data%20analysis/Screenshot%202025-09-01%20180912.png) | Additional dashboard screenshot. |

## Open the project

### View the animated project page

Open `index.html` in a modern browser. It is a standalone page and does not require a build step or external JavaScript packages.

### View the dashboard

- Open the [exported HTML report](E-Commerece%20Data%20analysis/E-commerce.html) in a browser.
- To inspect or edit the report, download the [Power BI file](E-Commerece%20Data%20analysis/E-Commerce.pbix) and open it in [Power BI Desktop](https://powerbi.microsoft.com/desktop/).

### Run the notebook

1. Clone or download this repository.
2. Install Python 3 and Jupyter, then install pandas:

   ```bash
   python -m pip install pandas jupyter
   ```

3. Obtain the source CSV dataset separately if it is not already available to you. The raw CSV is not included in this repository.
4. Open `E-Commerece Data analysis/E-commerce.ipynb` in Jupyter Notebook or JupyterLab.
5. Update the CSV path in the first notebook cell to point to your local dataset, then run the notebook cells.

The notebook currently contains a machine-specific Windows file path. Change it before running on another computer. For example:

```python
from pathlib import Path
import pandas as pd

csv_path = Path("data") / "Amazon Sale Report.csv"
df = pd.read_csv(csv_path, low_memory=False)
display(df.head())
df.info()
```

## Analysis areas

- Order and courier status, including shipped and cancelled records
- Product category, style, SKU, and size distribution
- Fulfilment and shipping service comparisons
- Sales-channel and business-to-business order composition
- Shipping destinations by city and state
- Data quality checks, missing values, and descriptive statistics

The notebook preview shows 128,975 rows and 24 columns. Some fields contain missing values, and one field has mixed types; clean and validate source data before drawing business conclusions. Any figures shown in the project materials describe the supplied dataset and are not live, continuously updating metrics.

## Technology

- **Dashboard:** Microsoft Power BI (`.pbix`) and exported HTML
- **Data analysis:** Python, Jupyter Notebook, pandas
- **Showcase page:** HTML and CSS (no build tooling or runtime dependencies)

## Motion and accessibility

The showcase uses CSS transitions and lightweight entrance/chart animations to emphasize the project highlights. It adapts to narrow screens, includes semantic page structure and visible focus states, and disables nonessential animation when the visitor has enabled `prefers-reduced-motion`.

## Data and privacy

The repository contains analysis artifacts and a notebook, but not the raw source CSV. Provide your own authorized copy of the dataset and avoid committing personal, confidential, or otherwise restricted information.

## Limitations

- This is an analytical project, not an ecommerce application; it does not provide product checkout, authentication, payment processing, or live order tracking.
- The HTML report is an exported artifact and may have different interactivity from the editable Power BI report.
- The notebook's original data path is local to its author's machine and must be replaced before execution elsewhere.
- Repository contents do not establish that the dashboard is deployed as a public live service.

## Contributing

Improvements to the notebook, report documentation, and showcase are welcome. Please keep dataset access and licensing requirements in mind, avoid adding private data, and describe any new assumptions or transformations.

## License

No license file is currently included. Unless a license is added, reuse and redistribution are not explicitly granted; contact the repository owner for permission.

## Author

Created by [saravanavel07](https://github.com/saravanavel07).
