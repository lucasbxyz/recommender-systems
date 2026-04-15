# Recommender Systems – MovieLens

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lucasbxyz/recommender-systems/HEAD)

Aufbau eines Film-Empfehlungssystems auf dem MovieLens-100k-Datensatz mit zwei Ansätzen: Memory-based Collaborative Filtering (User-User- und Item-Item-Ähnlichkeit mittels Cosine Similarity) sowie Model-based Collaborative Filtering (SVD-Matrixfaktorisierung).

## Ausführung

1. Auf den **Binder Badge** oben klicken — die Umgebung startet automatisch.
2. Im Jupyter-Interface das Notebook `2-Fortgeschrittene_Empfehlungssysteme.ipynb` öffnen.
3. **Cell → Run All** ausführen (oder Zellen einzeln mit Shift+Enter durchlaufen).
4. Die Ausführung dauert ca. 2–3 Minuten.

## Erwartete Ergebnisse

- **Datenübersicht:** 100.000 Bewertungen von 944 Nutzern für 1682 Filme.
- **Seltenheitslevel (Sparsity):** ca. **93.7 %** — typisch für Recommender-Datensätze.
- **Memory-based CF – RMSE-Werte:**
  - User-based CF RMSE: ca. **3.1**
  - Item-based CF RMSE: ca. **3.5**
- **Model-based CF (SVD):** RMSE niedriger als bei Memory-based CF — zeigt die Überlegenheit der Matrixfaktorisierung.
- Zusätzlich werden User-Item-Ähnlichkeitsmatrizen und Vorhersage-Matrizen berechnet.

## Dateien

| Datei | Beschreibung |
|-------|-------------|
| `2-Fortgeschrittene_Empfehlungssysteme.ipynb` | Jupyter Notebook mit der Analyse |
| `U.data` | MovieLens-Bewertungsdaten |
| `U.item` | Film-Metadaten |
| `Movie_Id_Titles` | Zuordnung Film-ID → Titel |
| `requirements.txt` | Python-Abhängigkeiten für Binder |
