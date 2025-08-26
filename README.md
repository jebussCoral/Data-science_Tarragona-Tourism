# Data-science_Tarragona-Tourism
# Data Science | Tourism Analysis in Tarragona (2025)

This project performs an exploratory data analysis (EDA) of official tourism data in Tarragona, Spain.  
The dataset was obtained from the Spanish National Statistics Institute (INE) and includes information on the number of travelers by origin (domestic and international) and time period (monthly data for 2025).  

The goal of this project is to practice data cleaning, transformation, and visualization using Python and to extract insights about the seasonality and structure of tourism in Tarragona.

---

## Dataset
- **Source:** INE (Instituto Nacional de Estadística, Spain)  
- **Territorial scope:** Tarragona province (Catalonia, Spain)  
- **Period:** Monthly data, year 2025  
- **Variables:**
  - Province
  - Type of indicator: Travelers / Overnight stays
  - Origin: Nationals (Spain) or Foreigners
  - Period (YYYYMM format)
  - Total number of travelers

---

## Analysis Performed
1. **Data Cleaning**
   - Removed province codes (e.g., "43 Tarragona" → "Tarragona").
   - Converted the `Total` column from string with thousand separators into integers.
   - Parsed `Period` into year and month using `datetime`.

2. **Exploratory Analysis**
   - General evolution of travelers over time.
   - Comparison between national and international travelers.
   - Stacked area charts to analyze absolute values and relative proportions.

3. **Visualizations**
   - Line chart of monthly traveler evolution.
   - Line chart comparing nationals vs foreigners.
   - Stacked area chart (absolute values).
   - Stacked area chart (percentage distribution).

---

## Key Findings
### Absolute Numbers
- January–March: Low tourism (<200k travelers), mostly nationals.
- April–May: Growth to ~1M travelers, foreigners increase strongly.
- June–July: Peak of ~2.5M travelers, growth mainly driven by foreigners.

### Proportions
- Winter: Nationals account for 75–80% of travelers.
- Spring: Foreigners rise quickly, reaching about 50%.
- Summer: Foreigners become the majority, exceeding 55–60%.

### Conclusion
Tourism in Tarragona shows a clear seasonal pattern:  
- In winter, activity depends on domestic travelers.  
- In summer, growth is largely sustained by international visitors.  

Overall, Tarragona’s tourism economy is supported by nationals during the low season but relies heavily on international tourism during the high season.

---

## Tools Used
- Python 3.11  
- pandas  
- seaborn  
- matplotlib  
- Jupyter Notebook  

---

## Repository Structure
- `tarragona_tourism_analysis.ipynb` → Jupyter Notebook with the full analysis.  
- `tarragona_tourism_analysis.html` → Exported HTML report.  
- `README.md` → Project description and results.  

---

## Author
Prepared by *David Coral*, 2025.
