# Portfolio — Mathieu Bellini

Portfolio-CV statique (HTML/CSS/JS) pour GitHub Pages.

## Déploiement (2 min)

1. Créer le repo `mathieubellini.github.io` (ou n’importe quel nom).
2. Uploader tous les fichiers de ce dossier.
3. **Settings → Pages → Build and deployment**  
   - Source: `Deploy from a branch`  
   - Branch: `main` / folder `/ (root)`  
4. Attendre 1–2 min → site en ligne : `https://<ton_user>.github.io/`.

## Mettre à jour les projets

- Éditer `data/projects.json` (miniatures dans `assets/img/`).
- Les liens `link_demo` / `link_repo` peuvent pointer vers :
  - Power BI Service (rapport public)  
  - Tableau Public  
  - GitHub (code, notebooks)

## Personnalisation

- Styles → `assets/style.css`  
- Portrait → `assets/img/portrait.jpg`  
- CV PDF → `CV_Mathieu_Bellini.pdf`

## À faire plus tard (placeholders déjà prévus)

- Miniatures réelles des projets (`assets/img/p*.jpg`)  
- Liens démo/repo pour chaque projet  
- Liens de publication des dashboards (page CV, section Dashboards)
- Vidéos de formation (liens YouTube ou fichiers)

```mermaid

%%{init: {
  "theme": "default",
  "gantt": { "todayMarker": "stroke-width:2", "topPadding": 50, "leftPadding": 100 }
}}%%
gantt
    title Aéroworld — Diagramme de Gantt (MVP)
    dateFormat  YYYY-MM-DD
    axisFormat  %d/%m
    todayMarker stroke:#e74c3c,stroke-width:2

    section L1 — Setup
    Repo Pages + squelette HTML/CSS/JS :active, l1, 2025-12-01, 0.5d

    section L2 — Veille
    Collecte 20+ articles + Excel normalisé + mesures : l2, after l1, 1d

    section L3 — Dashboards
    Visuels + KPIs + filtres (Power BI / Tableau) :crit, l3, after l2, 1.5d

    section L4 — Portfolio
    Fiches projets + routes + CV : l4, after l3, 1d

    section L5 — Vidéo & Doc
    Script + enregistrement + README : l5, after l4, 0.5d
```

