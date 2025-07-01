# Comprehensive Sales Data Cleaning & Validation with Google Sheets

## Unlock the True Power of Your Data

Are you struggling with inconsistent data that hinders your decision-making? **Clean, accurate, and well-structured data is the foundation of every successful business strategy.**

As a dedicated data professional, I specialize in transforming messy datasets into clear, actionable insights. This project showcases a meticulous approach to data cleaning and validation using **Google Sheets built-in features**, specifically for a **sales dataset** sourced from **[mention source, e.g., an internal company report or a publicly available dataset]**.

My work ensures that raw, often challenging data, is converted into a reliable and ready-to-analyze format, driving more informed business decisions.

### Challenges & Solutions Implemented

This project addressed several common data quality issues through a systematic approach:

* **Inconsistent Date & Currency Formats:**
    * **Challenge:** The raw data contained various date formats (e.g., 'DD-MM-YY', 'MM/DD/YYYY') and inconsistent currency representations (e.g., '$100', '100USD', '100').
    * **Solution:** I leveraged Google Sheets' **"Format > Number > Date"** options to apply a uniform 'MM-DD-YYYY' format across all date columns. For currency values, I meticulously used **"Find and Replace"** (e.g., replacing '$' with nothing, 'USD' with nothing) to remove symbols and text, followed by applying **"Format > Number > Number"** to ensure all values were clean numerical data, suitable for financial calculations.

* **Enhanced Readability & Navigation:**
    * **Challenge:** Large datasets often become difficult to navigate, with headers disappearing when scrolling down.
    * **Solution:** I strategically implemented **"View > Freeze > 1 row"** in Google Sheets. This ensured that crucial header rows remained visible at all times, significantly improving user experience and making the dataset much easier to navigate and understand.

* **Intelligent Blank Data Imputation (Region Field):**
    * **Challenge:** The 'Region' column had missing values, which could hinder geographical analysis or reporting.
    * **Solution:** Instead of arbitrary fills, I implemented a context-aware approach. For each row with a missing 'Region', I **cross-referenced the 'Name' field (e.g., customer name, product name, or location name) in that row with other existing records in the dataset that shared the exact same 'Name'**. If a matching 'Name' with a populated 'Region' was found elsewhere in the dataset, I used that confirmed region to fill the missing value. This method ensured that the imputed 'Region' was logically consistent with existing data, maintaining accuracy and data integrity.

* **Comprehensive Data Validation:**
    * **Challenge:** Inconsistent total prices that did not align with their corresponding quantity and unit price.
    * **Solution:** To ensure data integrity, I performed a rigorous validation check. I strategically implemented function like **MULTIPLY()** in a temporary column, then compared it with the existing "Total Price" column. Any discrepancies were identified and corrected, guaranteeing the accuracy and reliability of the final financial figures.

---

### Project Files & How to View

All project data, including both the **raw and cleaned datasets**, are provided as separate CSV files for easy accessibility and direct download.

* **`raw_data/Raw_Data.csv`**: This file contains the original, uncleaned dataset, showcasing the initial challenges.
* **`cleaned_data/Cleaned_Data.csv`**: This file contains the meticulously processed and validated dataset, representing the final, usable output.

You can download these CSV files directly from their respective folders in this GitHub repository to explore the data.

---

### Tools & Technologies Used

* Google Sheets (Specifically leveraging built-in features such as **Format Cells, Find and Replace, Freeze Panes, and function such as MULTIPLY() for data handling/validation techniques**)
* Microsoft Excel (for viewing `.csv` files if preferred)

---

### Live Google Sheets Link (Recommended for Direct View)

For a direct, interactive view of the consolidated data, you can access the live Google Sheets version here:

* **Consolidated Project Data:** [Paste Your Shareable Google Sheet Link Here (Ensure "Anyone with the link" and "Viewer" access)]

---

### Connect With Me

Feel free to connect or ask any questions! I'm always open to discussing data-driven solutions and opportunities.

* **Email:** [Your Professional Email Address]
* **LinkedIn:** [Link to Your LinkedIn Profile]
* **(Optional) Portfolio Website:** [Link to Your Google Sites Portfolio, if you decide to create one later]

---








