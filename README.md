# 📘 Analyse Syntaxique NLP

## 🚀 Description
Ce projet est une **analyse syntaxique multilingue** (français et coréen) utilisant **SpaCy** pour l'extraction des dépendances syntaxiques et leur **visualisation**.

📌 **Langues supportées** :
- 🇫🇷 Français (`fr_core_news_md`)
- 🇰🇷 Coréen (`ko_core_news_sm`)

📌 **Fonctionnalités** :
- Analyse morphologique et syntaxique avec SpaCy
- Visualisation des dépendances syntaxiques
- Automatisation du traitement
- Sauvegarde des résultats en fichier JSON/CSV

---

## 🛠️ Installation
### 1️⃣ **Cloner le dépôt**
```bash
git clone git@github.com:MarcelALng/analyse-syntaxique-nlp.git
cd analyse-syntaxique-nlp
```

### 2️⃣ **Créer un environnement virtuel et installer les dépendances**
```bash
python -m venv venv
source venv/bin/activate  # macOS/Linux
# Pour Windows : venv\Scripts\activate
pip install -r requirements.txt
```

### 3️⃣ **Télécharger les modèles SpaCy**
```bash
python -m spacy download fr_core_news_md
python -m spacy download ko_core_news_sm
```

---

## 🚀 **Utilisation**

### 1️⃣ **Exécuter le script d’analyse syntaxique**
```bash
python analyse.py
```

### 2️⃣ **Visualiser les dépendances syntaxiques**
Le script génère des visualisations interactives avec **displaCy**. Pour les voir :
```bash
python analyse.py --visualisation
```

### 3️⃣ **Sauvegarder les résultats**
Les résultats seront stockés dans `output/` sous format JSON ou CSV.

---

## 📊 **Exemple de Résultat**
Extrait d’analyse syntaxique :
```json
{
  "phrase": "Le chat noir dort sur le canapé.",
  "tokens": [
    {"text": "Le", "pos": "DET"},
    {"text": "chat", "pos": "NOUN"},
    {"text": "noir", "pos": "ADJ"},
    {"text": "dort", "pos": "VERB"},
    {"text": "sur", "pos": "ADP"},
    {"text": "le", "pos": "DET"},
    {"text": "canapé", "pos": "NOUN"},
    {"text": ".", "pos": "PUNCT"}
  ]
}
```

---

## 🏗️ **Structure du Projet**
```bash
📂 analyse-syntaxique-nlp/
├── 📂 data/                # Données d'entrée
├── 📂 output/              # Résultats analysés (JSON/CSV)
├── 📂 notebooks/           # Notebooks Jupyter
├── 📜 analyse.py           # Script principal
├── 📜 requirements.txt     # Dépendances Python
├── 📜 README.md            # Documentation
```

---

## 🤝 **Contribuer**
Si vous souhaitez contribuer, ouvrez une issue ou soumettez une PR sur GitHub !

---

## 📄 **Licence**
Ce projet est sous licence **MIT**. Voir le fichier `LICENSE` pour plus d’informations.

---

## 📧 **Contact**
👤 **Marcel Albert NGUYEN**  
✉️ [Email](mailto:marcelalbert@example.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/marcelalbert)


Analyse_Syntaxique_NLP
==============================

Analyst syntaxique multilingue (français, coréen) avec SpaCy et visualisation des dépendances.

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
