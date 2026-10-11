# 💼 Data Science Salary Calculator — Excel

An interactive Excel tool that shows the **median salary**, the **number of postings with salary data** and the **top job platform** for any combination of job title, country and schedule type. It's built on **32,000+ data-job postings from 2023**.

![Calculator preview](images/calculator.png)

## How it works
Pick a **Job Title**, **Country** and **Type** from the dropdowns. Everything updates instantly:
- Median salary, job count and top platform
- Median salary by job title (your selection highlighted)
- Median salary by schedule type
- A map of median salary by country

## Formula techniques
- **Dynamic dropdowns:** UNIQUE, SORT and FILTER build the input lists automatically from the data.
- **Conditional medians:** MEDIAN(IF(...)) with several conditions, matching schedule types with ISNUMBER(SEARCH()).
- **Lookups:** XLOOKUP with a fallback for combinations with no results.
- **Chart highlighting:** IF(..., NA()) splits the data into two series, so the selected item stands out.
- **Structure:** named ranges for inputs, a structured table (`jobs`) and hidden calculation sheets.

## Credits
Dataset and project idea from Luke Barousse's *Excel for Data Analytics* course. 
