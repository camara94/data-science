# data-science
Bienvenu dans ce tutorie, aucours duquel nous allons découvrir la librairie **pandas** qui est l'une des libraire les plus importantes en python, lorsque nous
voulons découvrir la data science.
Avec cette librairie nous pouvons faire tout ce dont nous pouvons imaginer en data science en python: 
* charger les données
    * csv
    * excel
    * text
    * *** 
* manipuler les les données
* combiner les datasets
* ...
* tout ceci grâce à une structure qu'on appelle le **DataFrame**

Dans ce tutoriel, nous allons illustrer l'utilisation de **pandas** grâce au **dataset** nommé **titanic.csv**

## Chargement d'un fichier CSV
pour un fichier, il faut d'abord importer le package, puis on fait appelle aux différentes methodes:
*importer le pacage
<h3><code>import pandas as pd</code></h3>
* pour charger un excel:
<h3><code>pd.read_excel('urlFichier')</code></h3>
* pour charger un fichier html:
<h3><code>pd.read_html('urlFichier')</code></h3>
* pour charger un sql:
<h3><code>pd.read_sql()</code></h3>
* ...
* pour notre fichier **csv**
<h3><code>df = pd.read_csv('titanic.csv')</code></h3>
