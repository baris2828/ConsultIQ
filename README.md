<!-- README of the PUBLIC showcase repo (baris2828/ConsultIQ).
     The source code lives in the private deploy repo; this is a showcase + links only. -->

<div align="center">

# 🎯 ConsultIQ
### Business-development cockpit for German IT consultancies

*Unsupervised ML segments profitable B2B customers, defines ICPs and prioritises high-value leads — mapped to the German market context (industry classification + federal state).*

[![Live Demo](https://img.shields.io/badge/▶_Live_Demo-Streamlit-FF4B4B?style=for-the-badge)](https://consultiq.streamlit.app/)
&nbsp;
![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-1.51-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)

</div>

---

## 🖼️ Preview

**Cockpit** — KPI bar, 2D lead radar (PCA), the "Why this score?" waterfall and the lookalike finder at a glance:

![Cockpit](screenshots/01_cockpit.png)

| Lead table & dossier export | Scoring weights & filters |
|:--:|:--:|
| ![Lead table and export](screenshots/02_leads_export.png) | ![Scoring weights and filters](screenshots/03_controls.png) |

## 💡 What ConsultIQ does
- 🧩 **ICP segmentation** — RFM + CLV → K-Means (silhouette-selected) + DBSCAN.
- 🛰️ **2D lead radar** — PCA signature view of every account, with the reference and its lookalikes highlighted.
- ⚖️ **Live scoring simulator** — drag the weights, the ranking updates instantly; "Why this score?" waterfall.
- 👯 **Lookalike finder** — find accounts similar to a top customer.
- 🗺️ **Germany map** — leads per federal state.
- 📤 **Dossier export** — Excel list & one-page PDF.

## 🛠️ Tech stack
`Python` · `Streamlit` · `pandas` · `scikit-learn` · `Plotly` · `Pydeck` · `pyarrow`

## 🏗️ Architecture (in short)
Local raw data → Python pipeline → a lean **Parquet artifact** → the app reads
exclusively through a **swappable data-source interface** (MySQL can be plugged in
as a v2 without changing the app).

## 🔍 Transparency
The dataset is *Online Retail II* (UK retail). The **federal state and industry
classification** are a **deliberately transparent, rule-based mapping layer** (demo) —
honestly documented on the app's methodology page.

---

<div align="center">

**👉 [Try the live demo](https://consultiq.streamlit.app/)**

Built by **Baris Aydin** · Data Science Portfolio

</div>
</content>
