# MeroJob IT Jobs Scraper

## Overview
This project scrapes IT and Telecommunication job postings from [MeroJob.com](https://merojob.com) using **Python**.  
It extracts **company names, job titles, and required skills**, and saves the data into a CSV file for analysis.

---

## Libraries Used
- `requests` – Fetch web pages  
- `BeautifulSoup` (`bs4`) – Parse HTML content  
- `pandas` – Store and manage data  

---

## Project Steps
1. **Fetch Webpage** – Load the job listings page using `requests.get()` with proper headers.  
2. **Parse HTML** – Use `BeautifulSoup` with the `lxml` parser to navigate the HTML structure.  
3. **Extract Data**  
   - Company names (`h3` tags)  
   - Job titles (`h1` tags with class `text-primary font-weight-bold media-heading h4`)  
   - Skills (`span` tags with `itemprop="skills"`)  
4. **Store Data** – Save the extracted information to a CSV file (`merojob_it_jobs.csv`) using `pandas`.

---

## How to Run
1. Clone the repository:
```bash
git clone https://github.com/YOUR-USERNAME/ML-projects.git

