# Failed Banks — Power BI Report

A compact, insight-driven Power BI report exploring bank failure patterns and related metrics. This repo lets you version the `.pbix`, share screenshots, and track any data-prep scripts used to refresh the model.

> **Suggested repository name:** `failed-banks-powerbi-report`

---

## 📊 What’s inside
- **Report file:** `failed banks.pbix`
- **(Optional) Data-prep:** put any CSVs or scripts in `data/` and `scripts/`
- **Screenshots:** store exports in `images/` for a quick visual readme gallery

---

## 🧭 Overview
Use this report to:
- Track the **count and timeline** of bank failures
- Compare **failures by category** (e.g., region, asset size, charter type—adapt to your model)
- Surface **key KPIs** (YTD failures, running totals, peak periods, etc.)
- Drill down from totals to detailed records

> Tip: Update the bullet list above to match your actual visuals/KPIs if they differ.

---

## 🗂️ Repo structure
```
failed-banks-powerbi-report/
├─ README.md
├─ failed banks.pbix
├─ images/                # optional: add report screenshots here
├─ data/                  # optional: raw / processed data files (kept small)
└─ scripts/               # optional: data-prep scripts (Power Query/M, Python, SQL, etc.)
```

---

## 🚀 Getting started

### Requirements
- **Power BI Desktop** (latest)
- Access to the **data source(s)** used in the `.pbix` (if the model isn’t fully imported)

### Open the report
1. Clone or download this repo.
2. Open **`failed banks.pbix`** with Power BI Desktop.
3. If prompted to connect to data, provide credentials/paths and **Refresh**.

### Refresh & publish
- Use **Transform Data** to review Power Query steps.
- Click **Refresh** to rebuild the model.
- Publish to **Power BI Service** → choose a workspace.
- (Optional) Configure **scheduled refresh** in the Service if your sources are online.

---

## 🔎 Data sources
Document your inputs clearly here, for transparency and reproducibility:

- **Source name:** (e.g., CSV, database, API)
- **Refresh cadence:** (e.g., weekly, monthly)
- **Field notes & assumptions:** (e.g., how you define “failure”, handling missing values)

> If the `.pbix` is fully imported with static data, note that here.

---

## 📈 Key visuals & KPIs (customize to fit your report)
- **KPI cards:** YTD Failures • Total Failures • Peak Year • Average Failures/Year
- **Time series:** Failures over time (monthly/quarterly aggregation)
- **Breakdown charts:** by Region • Bank Size • Charter Type (or your model’s dimensions)
- **Detail table:** searchable table of failed institutions (with slicers)

Add screenshots to `images/` and reference them here:
![Dashboard Overview](images/overview.png)
![Failures Over Time](images/failures-over-time.png)

---

## 🧪 Quality checks (optional)
- Validate totals against a trusted reference (if applicable)
- Spot-check dimension mappings (regions, categories)
- Ensure DAX measures handle **blank** and **div-by-zero** safely

---

## 🔧 Maintenance
- Pin visuals in the Service for a quick **dashboard** view.
- Track measure changes with short, clear commit messages.
- Keep **data source credentials** out of version control.

---

## 📝 Versioning workflow (example)
```bash
# initialize repo
git init
git add "failed banks.pbix" README.md
git commit -m "chore: add Power BI report and README"

# create folders for assets as you go
mkdir -p images data scripts
git add images/ data/ scripts/
git commit -m "chore: scaffold repo structure"

# when you update measures/queries
git commit -am "feat: add YTD and rolling 12-month failure measures"
```

---

## 📄 License
Choose a license (e.g., MIT) and add a `LICENSE` file if you intend to share publicly.

---

## 🙋 Support / contact
- Open an **Issue** for bugs or enhancement ideas.
- Add your contact or LinkedIn link here if you want contributors or feedback.
