# Predicció del guanyador de partides d'escacs (Lichess)  
### *Cas Kaggle – Aprenentatge Computacional (UAB)*

Aquest repositori conté el desenvolupament complet d’un projecte d’aprenentatge supervisat amb dades de partides d’escacs de **Lichess.org**, extretes del conjunt de dades de Kaggle: https://www.kaggle.com/datasnaek/chess

L’objectiu és **predir quin jugador guanyarà (blanques = 1, negres = 0)** utilitzant tant informació prèvia dels jugadors com característiques posicionalment derivades dels moviments de la partida.

---

## Estructura del repositori
├── games.csv 
├── games_EDA.csv 
├── games_preprocessed.csv 
├── 1_EDA.ipynb 
├── 2_preprocessing.ipynb 
├── funcions.py 
├── metric_selection.py
├── 3_model_previ.ipynb 
├── 3_model_partida.ipynb
└── README.md

Dins dels 4 notebooks en format Jupyter i dels dos scrpits en Python tenim el següent contingut:
- 1_EDA.ipnb : Anàlisis exploratori de les dades. S'analitza el conjunt de dades, on l'objectiu és entendre les variables que tenim.
- 2_preprocessing.ipnyb : en aquest notebook fem la preparació de les dades que utilitzarem. Creem noves variables i decidim quines utilitzarem en els models.
- metric_selection.py: script de python en el qual tenim les funcions que utilitzarem amb les mètriques, juntament 

---

## Autores
- Inés Gómez Carmona (1704361)
- Naroa Sarrià Gil (1706167)

Repositori GitHub:
https://github.com/NIU1706167/CasKaggle-Chess
