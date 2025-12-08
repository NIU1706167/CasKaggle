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
- metric_selection.py : script de python en el qual tenim les funcions que utilitzarem amb les mètriques, juntament amb una explicació de quines mètriques utilitzarem i perquè.
- 3_model_previ.ipynb : notebook on tenim els models que entrenem per partides que no han començat, és a dir, models que entrenem sense cap de les variables relacionades amb els moviments. L'objectiu és veure fins a quin punt un model pot predir el guanyador sense informació de la partida actual i, a més, analitzar si ja es pot descartar algun dels models. Per fer això fem una cerca d'hiperparàmetres i una validació creuada en cada model per aconseguir el seu millor rendiment.
- funcions.py : script de pyhton en el qual tenim totes les funcions que es necessiten per obtenir les variables relacionades amb els moviments que hem creat al fitxer "2_preprocessing.ipynb".
- 3_model_partida.ipynb : últim notebook en el qual entrenems models ara afegints les variables dels moviments i acabem seleccionant un model final, després de fer cerca d'hiperparàmetres i validació creuada.

---

## Autores
- Inés Gómez Carmona (1704361)
- Naroa Sarrià Gil (1706167)

Repositori GitHub:
https://github.com/NIU1706167/CasKaggle-Chess
