# TP Python/Pandas sur Capytale

## 📋 Fichiers à utiliser

Ce TP propose deux formats pour travailler avec Python et Pandas :

### Pour Capytale (recommandé) :
- **`analyse_films_capytale.ipynb`** : Notebook Jupyter interactif
- **`films_2024.csv`** : Données des films 2024
- **`films_2023.csv`** : Données des films 2023
- **`INSTRUCTIONS_pandas.pdf`** : Guide des commandes Pandas (à compiler depuis le .tex)

### Pour travail classique (script Python) :
- **`TP_donnees_structurees_python_enonce.tex`** : Énoncé au format LaTeX (nécessite le fichier Excel)

---

## 🚀 Installation sur Capytale

### Étape 1 : Créer une activité
1. Connectez-vous à Capytale
2. Créez une nouvelle activité **Notebook Python**

### Étape 2 : Importer les fichiers
1. Cliquez sur le bouton "Importer" ou "Upload"
2. Importez les 3 fichiers suivants :
   - `analyse_films_capytale.ipynb`
   - `films_2024.csv`
   - `films_2023.csv`

### Étape 3 : Ouvrir le notebook
1. Ouvrez le fichier `analyse_films_capytale.ipynb`
2. Le notebook contient toutes les questions et cellules de code
3. Les élèves peuvent exécuter et compléter les cellules directement

---

## 📊 Structure du notebook

Le notebook est organisé en 5 sections principales :

1. **Importation et chargement des données** (pré-rempli)
   - Import de pandas
   - Lecture des fichiers CSV

2. **Analyse sommaire** (Questions 1-3)
   - Film avec le plus d'entrées en 2024
   - Film français avec le plus d'entrées en 2023
   - Nationalité dominante en 2023

3. **Filtrage et agrégation** (Questions 4-6)
   - Top 3 films français
   - Comptage et total d'entrées
   - Statistiques descriptives

4. **Analyse avancée** (Questions 7-17)
   - Films sortis en 2023 mais comptabilisés en 2024
   - Analyse par nationalité (US, GB, FR)
   - Comparaison 2023-2024

5. **Pour aller plus loin** (Questions 18-19)
   - Groupby et agrégations
   - Analyse temporelle (défi)

---

## 🎓 Guide des commandes Pandas

Le fichier `INSTRUCTIONS_pandas.tex` contient un guide de référence avec :
- Commandes de base (head, info, columns, shape)
- Filtrage simple et avancé
- Tri des données
- Calculs statistiques
- Groupby et agrégations
- Tableau récapitulatif

**Pour les élèves :** Compilez ce fichier en PDF ou consultez-le comme référence pendant le TP.

---

## 💡 Avantages du format notebook

✅ **Pas besoin d'installation** : Tout fonctionne dans le navigateur
✅ **Code pré-rempli** : Les imports et exemples sont déjà fournis
✅ **Exécution cellule par cellule** : Les élèves testent au fur et à mesure
✅ **Markdown intégré** : Questions et explications dans le même fichier
✅ **Fichiers CSV** : Plus faciles à uploader que les fichiers Excel

---

## 📝 Déroulement du TP

1. Les élèves ouvrent le notebook sur Capytale
2. Ils lisent les instructions dans les cellules markdown
3. Ils complètent les cellules de code vides
4. Ils exécutent leurs réponses avec Shift+Entrée
5. Ils notent leurs observations dans un document séparé (LibreOffice Writer)

---

## 🔧 Alternative : Téléchargement direct depuis data.gouv.fr

Si vous souhaitez que les élèves téléchargent eux-mêmes les données, ajoutez cette cellule au début du notebook :

```python
import pandas as pd
import urllib.request

# URL du fichier sur data.gouv.fr
url = "https://www.data.gouv.fr/fr/datasets/r/[ID_RESSOURCE]"

# Télécharger et lire le fichier
urllib.request.urlretrieve(url, "films.xlsx")
df_2024 = pd.read_excel("films.xlsx", sheet_name='2024', header=6)
```

*(Remplacez `[ID_RESSOURCE]` par l'ID réel du fichier sur data.gouv.fr)*

---

## 📤 Rendu du travail

Les élèves peuvent rendre :
- Le notebook complété (`.ipynb`)
- Un export HTML du notebook (Fichier > Télécharger > HTML)
- Un document LibreOffice Writer avec leurs réponses et analyses

---

## ❓ Questions fréquentes

**Q : Pandas n'est pas installé sur Capytale**
R : Pandas est préinstallé sur tous les environnements Python de Capytale. Si vous rencontrez une erreur, vérifiez l'orthographe de `import pandas as pd`.

**Q : Les fichiers CSV ne sont pas trouvés**
R : Vérifiez que les fichiers sont bien dans le même dossier que le notebook sur Capytale. Les noms de fichiers doivent être exacts : `films_2024.csv` et `films_2023.csv`.

**Q : Comment les élèves notent-ils leurs réponses ?**
R : Ils peuvent soit ajouter des cellules markdown dans le notebook, soit rédiger un document séparé dans LibreOffice Writer.

**Q : Peut-on utiliser ce TP sans Capytale ?**
R : Oui ! Le notebook fonctionne dans n'importe quel environnement Jupyter (Jupyter Lab, Google Colab, VSCode, etc.). Il suffit d'avoir les fichiers CSV dans le même dossier.

---

## 📚 Ressources complémentaires

- Guide des commandes : `INSTRUCTIONS_pandas.pdf`
- Documentation Pandas : https://pandas.pydata.org/docs/
- Tutoriels Pandas en français : https://openclassrooms.com/

---

**Bon TP ! 🎉**
