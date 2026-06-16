<!-- Diese Datei wird das README des ÖFFENTLICHEN Showcase-Repos (baris2828/ConsultIQ).
     Der Code liegt im PRIVATEN Repo; hier nur Schaufenster + Links. -->

<div align="center">

# 🎯 ConsultIQ
### Business-Development-Cockpit für deutsche IT-Beratungen

*Unsupervised ML segmentiert profitable B2B-Kunden, definiert ICPs und priorisiert hochwertige Leads — im deutschen Marktkontext (WZ-2008-Branche + Bundesland).*

[![Live Demo](https://img.shields.io/badge/▶_Live_Demo-Streamlit-FF4B4B?style=for-the-badge)](PLATZHALTER_STREAMLIT_URL)
&nbsp;
![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-1.51-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)

</div>

---

## 🖼️ Vorschau

| Cockpit & Lead-Radar | Scoring-Simulator & Wasserfall |
|:--:|:--:|
| ![Cockpit](screenshots/01_cockpit.png) | ![Simulator](screenshots/02_simulator.png) |
| **Deutschlandkarte (Bundesland)** | **Lookalike-Finder & Dossier-Export** |
| ![Karte](screenshots/03_karte.png) | ![Lookalike](screenshots/04_lookalike.png) |

> _Screenshots ersetzen die Platzhalter in `screenshots/` — siehe Hinweis dort._

## 💡 Was ConsultIQ kann
- 🧩 **ICP-Segmentierung** — RFM + CLV → K-Means (Silhouette-Wahl) + DBSCAN.
- 🛰️ **2D-Lead-Radar** — PCA-Signaturansicht aller Accounts, Referenz & Lookalikes hervorgehoben.
- ⚖️ **Live-Scoring-Simulator** — Gewichte verschieben, Ranking ändert sich sofort; **„Warum dieser Score?"**-Wasserfall.
- 👯 **Lookalike-Finder** — finde zu einem Top-Kunden ähnliche Accounts.
- 🗺️ **Deutschlandkarte** — Leads je Bundesland.
- 📤 **Dossier-Export** — Excel-Liste & PDF-One-Pager.

## 🛠️ Tech-Stack
`Python` · `Streamlit` · `pandas` · `scikit-learn` · `Plotly` · `Pydeck` · `pyarrow`

## 🏗️ Architektur (kurz)
Lokale Rohdaten → Python-Pipeline → schlankes **Parquet-Artefakt** → App liest
ausschließlich über eine **austauschbare Datenquellen-Schnittstelle** (MySQL als
v2 andockbar, ohne App-Änderung).

## 🔍 Transparenz
Basis ist *Online Retail II* (UK-Einzelhandel). **Bundesland & WZ-Branche** sind
eine **bewusst transparente, regelbasierte Mapping-Ebene** (Demo) — ehrlich
dokumentiert auf der Methodik-Seite der App.

---

<div align="center">

**👉 [Live-Demo ausprobieren](PLATZHALTER_STREAMLIT_URL)**

Erstellt von **Baris Aydin** · Data Science Portfolio

</div>
