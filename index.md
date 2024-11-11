## Informatics and Data Science Projects

---

### NLP API for extraction of structured data from freetext palliative care consult questions


I developed a rule-based natural language processing tool using MedSpacy which can extract the diagnosis and reason for consult from free-text palliative care consult questions. 

This tool is planned for use as part of our department's push to integrate with the Palliative Care Quality Collaborative, a nation wide database of palliative care programs used for benchmarking and QA/QI initiatives.

The code can be used within Jupyter Notebooks, but for ease of deployment and transportability I also turned it into a dockerized FastAPI and deployed the API to a DigitalOcean Droplet.

<img src="images/api.png?raw=true"/>

<img alt="Static Badge" src="https://img.shields.io/badge/Python-grey?logo=Python"> <img alt="Static Badge" src="https://img.shields.io/badge/Pandas-grey?logo=Pandas">
 <img alt="Static Badge" src="https://img.shields.io/badge/spaCy-grey?logo=spaCy"> <img alt="Static Badge" src="https://img.shields.io/badge/FastAPI-grey?logo=fastAPI"> <img alt="Static Badge" src="https://img.shields.io/badge/Docker-grey?logo=Docker"> <img alt="Static Badge" src="https://img.shields.io/badge/DigitalOcean-grey?logo=DigitalOcean">

 [View code on GitHub](https://github.com/kmacman/Palliative-Consult-NLP)<br>
 [Try API in Google Colab](https://colab.research.google.com/drive/16JjCPyPETtcCCg1V32wj3jnYWnqQTs-V?usp=sharing)<br>
 [View API Docs](http://palliapi.kentmccannmd.com/docs#/default/analyze_text_analyze_post)

---

### Sentiment Analysis of Student Doctor Network Specialty Forums from Inception through 2023

To see how sentiment of various specialties has changed over time, I scraped forum posts from the Student Doctor Network subspecialty boards using BeautifulSoup. I then analyzed the sentiment of each post using a HuggingFace Transformer.

An abstract using this data was accepted as a quick shot presentation to the American College of Surgeons Clinical Congress 2024.

Here are the results for each specialty, averaged by year, rendered using D3Blocks (click the specialties to see their plots):

<iframe src="images\timeseries.html" width="100%" height="520" frameborder="0" style="border: none; display: block; margin: auto;"></iframe>

<img alt="Static Badge" src="https://img.shields.io/badge/Python-grey?logo=Python"> <img alt="Static Badge" src="https://img.shields.io/badge/Pandas-grey?logo=Pandas"> <img alt="Static Badge" src="https://img.shields.io/badge/HuggingFace-grey"> <img alt="Static Badge" src="https://img.shields.io/badge/BeautifulSoup-grey"> <img alt="Static Badge" src="https://img.shields.io/badge/D3Blocks-grey?logo=d3.js"> 

[Jupyter Notebook of Scraping/Sentiment Analysis Script](pdf\Scraping_Script.html) 

(SDN has since changed to dynamically loaded content, so this scraping script no longer works)

---

### Department QA/QI Dashboard

I created a Streamlit dashboard to explore departmental consultation data for our inpatient palliative care service.

The ETL process is automated, so newly generated EHR reports can easily be added to the existing data.

The NLP program above is utilized to enrich the data to allow for more granular analysis of patient diseases and reasons for consults.

The data is filterable by all columns and all visualizations automatically update to reflect filtering.

<img src="images\dashboard.png"/>

_Examples of the visualizations within the dashboard, values have been edited out_

<img alt="Static Badge" src="https://img.shields.io/badge/Python-grey?logo=Python"> <img alt="Static Badge" src="https://img.shields.io/badge/Pandas-grey?logo=Pandas"> <img alt="Static Badge" src="https://img.shields.io/badge/Streamlit-grey?logo=Streamlit"> <img alt="Static Badge" src="https://img.shields.io/badge/Plotly-grey?logo=Plotly">  

---
<p style="font-size:11px">Page template forked from <a href="https://github.com/evanca/quick-portfolio">evanca</a></p>
<!-- Remove above link if you don't want to attibute -->
