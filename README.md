<div align="center">

# Abdallah Abukhalil

### Data Analyst · Analytics Engineer 

*B.Sc in Stat & CS - Ain Shams University*

<br>
I work with data to understand what is happening,
why it is happening, and what we can learn from it.

Currently exploring **Machine Learning** and the intersection of **data & media**.

<br>

<a href="https://www.linkedin.com/in/abdallahabukhalil/">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/linkedin-white.svg">
    <source media="(prefers-color-scheme: light)" srcset="./assets/linkedin-black.svg">
    <img src="./assets/linkedin-black.svg" width="32" alt="LinkedIn">
  </picture>
</a>
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://github.com/abdallahabukhalil">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/github-white.svg">
    <source media="(prefers-color-scheme: light)" srcset="./assets/github-black.svg">
    <img src="./assets/github-black.svg" width="32" alt="GitHub">
  </picture>
</a>
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://huggingface.co/abdallahabukhalil">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/huggingface-white.svg">
    <source media="(prefers-color-scheme: light)" srcset="./assets/huggingface-black.svg">
    <img src="./assets/huggingface-black.svg" width="32" alt="Hugging Face">
  </picture>
</a>

</div>

<br>

<div align="center">

`Python`  ·  `SQL`  ·  `Power BI`  ·  `Excel`  ·  `Pandas`  ·  `scikit-learn`  ·  `DAX`  ·  `FastAPI`  ·  `Git`

</div>

<br>

---
<div align="center">

## Selected Work

*Projects where I worked with data from collection to analysis and insight.*

</div>

<br><br>

<table>
<tr>
<td align="center">

<div align="center">

<picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/bynat-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="./assets/bynat-light.svg">
    <img src="./assets/bynat-light.svg" width="300" alt="bynat">
</picture>

<h3>A Python toolkit for simplifying data workflows.</h3>

**Tidy, Enrich & Cache Tabular Data**

</div>

<br>

<div align="center">
A Python toolkit made of small, reusable utilities for tidying, enriching, loading, saving and caching tabular data.
</div>

<br>

<div align="center">
Built on pandas. Use it as a <code>df.bynat</code> accessor or through the <code>BaseData</code> class, and let a SQLite cache remember slow lookups between runs.
</div>

<br>

</td>
</tr>
</table>
<br>

Cleaning:
<div align="center">

  ### Messy Table → df.bynat or BaseData → Cleaning Methods → Tidy Table

</div>

Caching:
<div align="center">

  ### Unique Values → Cache Lookup → Fetch Misses → Checkpoint to SQLite

</div>

<br>

<div align="center">
<table>
<tr>
<td align="center" width="25%">

**2**

core
dependencies

</td>

<td align="center" width="25%">

**6**

optional
integrations

</td>

<td align="center" width="25%">

**3**

fill
strategies

</td>

<td align="center" width="25%">

**1**

SQLite file
per cache folder

</td>
</tr>
</table>

<br>

<table>
<tr>
<td width="50%" valign="top">

### What You Can Do

* Clean ordinary pandas tables with the **`df.bynat`** accessor, or use the class API (`BaseData`, `JsonFile`, `CsvFile`). Both use the same cleaning code
* Work **by group**: `fill_missing`, `handle_outliers`, `drop_outliers` and `get_hierarchical_stats` follow a hierarchy such as country → job title
* Reshape columns: rename, drop, reorder and move them, use `melt_transform_pivot`, and split list cells with `split_list_objects`
* Work with text: `extract_keywords`, `categorize_by_reference`, `truncate_after_substring` and `impute_by_language`
* Add outside information: translation, geocoding, `convert_to_usd` and spaCy entity extraction
* Load and save: `read_csv`, `read_json`, `save_to_json` (with append and deduplication) and `save_to_sql`
* Check the work: tests run offline with fake modules, and the faster methods have equivalence tests and benchmark scripts

</td>

<td width="50%" valign="top">

### Why Analysts Will Like It

**Cleaning That Knows Your Groups:** <br>
A missing salary should not get one number for the whole table. bynat fills it from its own group, like country and job title, and works through the levels step by step. Outliers are checked inside each group too.

<br>

**Numbers You Can Show:** <br>
Ask for `get_hierarchical_stats=True` and you also get the group values the cleaning was based on, taken before anything changed. Now you can show your team why a value was filled or removed.

<br>

**Slow Lookups, Done Once:** <br>
Translating categories, finding coordinates and converting money to USD all take time. bynat asks for each unique value once and keeps the answer in a SQLite file, so the same lookup is not repeated on the next run. Progress is saved every `save_every` values, and failed lookups are tried again later.

<br>

**Light to Start:** <br>
You only need `numpy` and `pandas`. Want translation, maps, currency, NLP or SQL? Add just the extra you need. You can also bring your own translator, geocoder or rate source with `provider=`.

<br>

**Short, Readable Cleanups:** <br>
Methods chain, so a cleanup takes one line: `records.bynat.rename_all_DOTS().bynat.drop_by_substring("user")`. Prefer classes? `BaseData` does the same jobs.

<br>

One small workbench for the fiddly jobs around a table.

</td>
</tr>
</table>
</div>

<br>

<div align="center">

`Python` · `pandas` · `NumPy` · `SQLite` · `spaCy` · `SQLAlchemy` · `pytest` · `Ruff` · `mypy` · `GitHub Actions`

<br>

<a href="https://pypi.org/project/bynat/">
PyPI →
</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://github.com/bynat-lab/bynat">
Source Code →
</a>

</div>

<br>
<br>

---

<table>
<tr>
<div align="center">

<p><img src="./assets/ludova-logo.svg" alt="Ludova Logo" width="42" align="middle"> <h3>Ludova</h3> </p>

<h3>Game Recommender</h3>

**Content-Based Recommendation & Blender Systems**

</div>

<br>

<div align="center">
A team project built around a content-based Steam game recommendation system and a separate game blending system that uses recommendation results to build a final set of games.
</div>

<br>

<div align="center">
As a <b>Contributor</b>, I designed and implemented the Python Recommendation Engine and separately the Python Post-Process Game Blender, while keeping both components compatible with the project's original implementations through fallbacks.
</div>

<br>

</tr>
</table>
<br>

Game Recommender:
<div align="center">

  ### Selected Games → TF-IDF Representations → MixScore → Ranked Candidates

</div>

Game Blender:
<div align="center">
  
  ### Ranked Candidates → Raw Tags → P75 Groups → Final Selection

</div>

<br>

<div align="center">
<table>
<tr>
<td align="center" width="25%">

**20K+**

Steam games

</td>

<td align="center" width="25%">

**2**

content
signals

</td>

<td align="center" width="25%">

**P75**

tag-based
grouping

</td>

<td align="center" width="25%">

**2**

separate systems

</td>
</tr>
</table>

<br>

<table>
<tr>
<td width="50%" valign="top">

### What I Built

* Python **Recommendation Engine** using separate TF-IDF representations for game Tags and review-derived Keywords
* Character-level TF-IDF with `char_wb`, using `(3,5)` n-grams for Tags and `(2,4)` n-grams for Keywords
* **MixScore** combining Tag and Keyword similarity using their geometric mean without manually assigned weights
* Candidate generation and ranking based on the selected games and their content similarity
* Python **Game Blender** that works with ranked candidates from the Recommendation Engine and their raw Tags
* P75 grouping, Exclusive Tags, and CoverageCount logic for the final game selection

</td>

<td width="50%" valign="top">

### What I Built Around

**Recommendation Ranking:** <br>
The new scoring engine combines two independent content signals — Tags and review-derived Keywords — into a single MixScore for ranking candidate games.

<br>

**Game Blending:** <br>
The Blender takes the ranked candidates and groups them by their raw Tags, then uses P75 grouping, Exclusive Tags, and CoverageCount to build the final recommendation set.

<br>

The pipeline is designed to combine content similarity with tag coverage without relying on manually assigned weights.

</td>
</tr>
</table>
</div>

<br>

<div align="center">

`Python` · `scikit-learn` · `Pandas` · `TF-IDF` · `Cosine Similarity` · `FastAPI` · `Git` · `GitHub`

<br>

<a href="https://game-recommender.runasp.net/">
Live Demo →
</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://github.com/moaazali3/Game-Recommender-API">
Source Code →
</a>

</div>

<br>
<br>

---

<table>
<tr>
<div align="center">
<p><img src="./assets/InsightHub%20Logo.svg" alt="InsightHub Logo" width="42" align="middle"> <h3>InsightHub</h3> </p>

**Job Market Analytics Platform**
</div>

<br>

<div align="center">
A graduation project built to make job market data easier to explore by bringing job listings, market trends, career information, and other resources into one platform.
</div>

<br>

<div align="center">
As <b>Project Lead & Data Analyst</b>, I led the analytics side of the project — building the data workflows and the Analytics Engine behind the platform's insights.
</div>

<br>

</tr>
</table>


<div align="center">
  
### Raw Data → Refresh Stage → Shared Data → Analytics Engine → Endpoints → Insights

</div>

<br>

<div align="center">
<table>
<tr>
<td align="center" width="25%">

**10K+**

job records
per run

</td>

<td align="center" width="25%">

**65%**

less repeated
processing

</td>

<td align="center" width="25%">

**1.9×**

Junior → Lead
salary growth

</td>

<td align="center" width="25%">

**70%**

higher Senior
demand

</td>
</tr>
</table>

<br>

<table>
<tr>
<td width="50%" valign="top">

### What I Built

* Backend **Analytics Engine** using Python, Pandas, FastAPI, and Requests
* Data collection, cleaning, transformation, and preparation workflows
* Classification and caching logic reducing repeated processing by **up to 65%**
* Dynamic KPIs and calculations for platform dashboards
* Geocoding and multi-currency conversion for data enrichment
* APIs connecting the analytics layer with the Backend and Flutter teams

</td>

<td width="50%" valign="top">

### What I Found

**Salary Growth:**
<br>
Junior → Lead roles showed around **1.9× salary growth**.

<br>

**Senior Demand:**
<br>
Senior positions showed approximately **70% higher demand in the gig economy**.

<br>

The analysis turned the collected job data into a clearer view of how roles, salaries, and demand change across the market.

</td>
</tr>
</table>
</div>

<br>

<div align="center">

`Python` · `Pandas` · `FastAPI` · `Requests` · `spaCy` · `Git` · `GitHub`

<br>

<a href="https://app.notion.com/p/InsightHub-Documentation-3599d9622f6e80348c9fdad909684c36?session_sync_attempted=1">
Documentation →
</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://github.com/InsightHubapp/Analytics-Department">
Analytics Engine →
</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://github.com/InsightHubapp/InsightHub">
Full Project →
</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://github.com/InsightHubapp">
Organization →
</a>

</div>

<br>
<br>

---

<tr>
<td>

<div align="center">

### Apple Retail Sales

**Analysis · DEPI**
</div>

<br>

<div align="center">
A collaborative Power BI project exploring 2024 Apple retail sales data covering <b>$1B in revenue</b> and <b>1M units sold</b>.
</div>

<br>

<div align="center">
The project focused on product performance, sales patterns, and warranty data while using Git and GitHub for team collaboration.
</div>

<br>

<div align="center">
  
### A Few Numbers

</div>

<br>

<div align="center">
<table width="100%">
<tr>
<td align="center" width="25%">

**$1B**

revenue

</td>

<td align="center" width="25%">

**1M**

units

</td>
<td align="center" width="25%">

**$337M**

top categories

</td>

<td align="center" width="25%">

**66%**

faster delivery

</td>
</tr>
</table>
</div>

<br>

<table>
<tr>
<td width="50%" valign="top">

### What I Built

* Cleaned and preprocessed data and designed a star schema.
* Used Git and GitHub for version control and team collaboration, reducing project delivery time by 66%, from 30 days to 10 days.
* Contributed to standardizing the dashboard layout and grid structure.

</td>

<td width="50%" valign="top">

### What I Found

<br>

* Tablets and Accessories generated **$337M** in revenue.
* Beats Fit Pro generated **$21.7M**, despite AirPods Pro selling more units.
* Git and GitHub reduced delivery time from **30 days to 10 days**.

</td>
</tr>
</table>

<div align="center">

`Power BI` · `DAX` · `Git` · `GitHub`

<br>

<a href="https://github.com/ALI-FADLOUN/DEPI-Project">

**View Project →**

</a>
</div>

<br>
<br>

---

<div align="center">

## Other Projects & Code Collections

</div>

* **[Core Algorithms in Python](https://github.com/abdallahabukhalil/Algorithms):** A collection of core algorithms originally studied as college pseudocode, now implemented in Python code.
* **[Core Data Structures](https://github.com/abdallahabukhalil/Data-Structure):** Legacy data structure implementation in python Programs
* **[Dawak Pharmacy Database](https://github.com/abdallahabukhalil/Pharmacy-Chain-Database---Dawak-University-Project-):** Database architecture, EER diagrams, and SQL queries for a pharmacy chain management system.

<br>

<div align="center">

**<a href="https://github.com/abdallahabukhalil?tab=repositories">View More Repositories →</a>**

</div>

<br>

---

<div align="center">

## What I'm Exploring

### Machine Learning

**Supervised Learning** · **Modeling** · **Data-driven prediction**

I'm building on my background in statistics and data analysis to understand how machine learning can answer a wider range of questions.

**[Explore my Machine Learning Journey workspace →](https://github.com/abdallahabukhalil/Machine-Learning-Journey)**

<br>

### Data × Media

I'm also interested in how data can work with **advertising, content, and the broader media industry**.

</div>

<br>

---
<div align="center">

### Let's connect

<a href="https://www.linkedin.com/in/abdallahabukhalil/">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/linkedin-white.svg">
    <source media="(prefers-color-scheme: light)" srcset="./assets/linkedin-black.svg">
    <img src="./assets/linkedin-black.svg" width="32" alt="LinkedIn">
  </picture>
</a>
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://github.com/abdallahabukhalil">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/github-white.svg">
    <source media="(prefers-color-scheme: light)" srcset="./assets/github-black.svg">
    <img src="./assets/github-black.svg" width="32" alt="GitHub">
  </picture>
</a>
&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://huggingface.co/abdallahabukhalil">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/huggingface-white.svg">
    <source media="(prefers-color-scheme: light)" srcset="./assets/huggingface-black.svg">
    <img src="./assets/huggingface-black.svg" width="32" alt="Hugging Face">
  </picture>
</a>

<br>

<sub>Always learning. Always building.</sub>

</div>
