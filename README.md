# Mathieu Bellini — Portfolio / CV

Site statique (HTML/CSS/JS) pour présenter mes projets **Data / BI Analyst**  
Stack : **Power BI · Tableau · Python (pandas) · KNIME · SQL**

**🌐 Live (préprod) :** https://materwwelon.github.io/mathieubellini.github.io/  
**📂 Repo :** ce dépôt

---

## 👀 Aperçu

<p align="center">
  <a href="https://materwwelon.github.io/mathieubellini.github.io/">
    <img src="assets/img/loom_thumb.png" width="720" alt="Aperçu du portfolio">
  </a>
</p>

---

## 🧭 Navigation

- **Accueil / Portfolio** → [`/data/index.html`](data/index.html)
- **Projets** → [`/data/projects.html`](data/projects.html)
- **CV & Livrables** → [`/data/cv.html`](data/cv.html)

> Le site utilise une feuille de style unique : [`/assets/style.css`](assets/style.css)

---

## 🎬 Vidéo de formation

- **Loom (démo / tutoriel)**  
  👉 https://www.loom.com/share/0c1bbddcb0a14fa798b59467d7be5648

---

## 📑 Documents

## 📚 Documentation

- [Documentation — Portfolio (Word)](assets/docs/Documentation.docx)

- **Analyse du besoin métier client — Aéroworld (Word)**  
  [`/assets/docs/Analyse_du_besoin_métier_client.docx`](assets/docs/Analyse_du_besoin_métier_client.docx)

- **Cahier des charges — Aéroworld (Word)**  
  [`/assets/docs/Cahier_des_charges.docx`](assets/docs/Cahier_des_charges.docx)

- **CV (PDF)**  
  [`/assets/docs/CV_Mathieu_Bellini.pdf`](assets/docs/CV_Mathieu_Bellini.pdf)

- [Carte mentale — Portfolio (PDF)](assets/docs/carte_mentale.pdf)

### Rapports Power BI (PBIX)

- [⬇️ Télécharger — Tableau de bord de veille (PBIX)](assets/pbix/Veille.pbix)
- [⬇️ Télécharger — Portfolio interactif (PBIX)](assets/pbix/Portfolio.pbix)



---

## 🧱 Structure du dépôt


- Les pages HTML de `/data` pointent vers les ressources avec des **chemins relatifs** `../assets/...`.
- Les miniatures des cartes projet sont dans `assets/img/` (ex. `p07.svg`…`p12.svg`).

---

## 🗂️ Projets (extraits)

| Miniature | Projet | Rôle / Année | Stack | Résumé |
|---|---|---|---|---|
| ![p07](assets/img/p07.svg) | **Project Cost Alerts — Star Schema** | BI Analyst · 2025 | Power BI, DAX | Alerte écarts coûts (≥15%), refactor en schéma en étoile |
| ![p08](assets/img/p08.svg) | **Executive Dashboard — Direction** | BI Analyst · 2025 | Power BI | Vue exécutive 3 pages, navigation par bookmarks |
| ![p09](assets/img/p09.svg) | **Gender Equality Index — KNIME Workflow** | Data Analyst · 2025 | KNIME, Python | Rule Engine patterns, export CSV reproductible |
| ![p10](assets/img/p10.svg) | **Water & Stability — 3 Tableau Views** | Data Viz · 2025 | Tableau | Monde → Continent → Pays + KPIs |
| ![p11](assets/img/p11.svg) | **Portfolio Catalog — Project Cards** | BI / Front · 2025 | Power BI | Cartes réutilisables, liens vers dashboards |
| ![p12](assets/img/p12.svg) | **Recruiter Path — 2-minute overview** | BI UX · 2025 | Power BI | Boutons + bookmarks, page KPI d’atterrissage |

> 🔗 Détails et cartes complètes : [`/data/projects.html`](data/projects.html)

---

## 🔁 Mettre à jour les projets

Deux options :

### A) Édition rapide (statique)
Modifier directement les cartes HTML dans [`/data/projects.html`](data/projects.html).

### B) Source JSON (dynamique)
Utiliser [`/data/projects.json`](data/projects.json) — le script embarqué remplace les cartes statiques si le JSON est chargé avec succès.

**Exemple d’entrée :**
```json
{
  "anchor": "p-cost-alerts",
  "title": "Project Cost Alerts — Star Schema",
  "year": "2025",
  "role": "BI Analyst",
  "stack": "Power BI, DAX",
  "img": "p07.svg",
  "summary": "Alerte écarts coûts (≥15%), refactor en schéma en étoile"
}
```
```mermaid

%%{init: { "theme": "default", "gantt": { "todayMarker": {"stroke-width": 2}, "topPadding": 50, "leftPadding": 100 }}}%%
gantt
  title Aéroworld — Diagramme de Gantt (MVP)
  dateFormat  YYYY-MM-DD
  axisFormat  %d/%m
  todayMarker stroke:#e74c3c,stroke-width:2

  section L1 — Setup
  Repo Pages + squelette HTML/CSS/JS :active, 11, 2025-12-01, 0.5d

  section L2 — Veille
  Collecte 20+ articles + Excel normalisé + mesures : 12, after 11, 1d

  section L3 — Dashboards
  Visuels + KPIs + filtres (Power BI / Tableau) :crit, 13, after 12, 1.5d

  section L4 — Portfolio
  Fiches projets + routes + CV : 14, after 13, 1d

  section L5 — Vidéo & Doc
  Script + enregistrement + README : 15, after 14, 0.5d

```
