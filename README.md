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
* etc
* pour notre fichier **csv**
<h3><code>df = pd.read_csv('titanic.csv')</code></h3>

## Quelques fonctions utiles

### La fonction head()
<h4><code>df.head()</code></h4>

cette fonction permet d'afficher les cinq prémières lignes d'un **dataframe** par defaut, mais on peut à fait indiquer le nombre de ligne qu'on affcicher si l'on souhaite.

### La fonction describe()
<h4><code>df.describe()</code></h4>
Celle-la est une fonction de statistique qui nous permet:

* d'afficher le nombre de ligne
* la moyenne des colonnes qui contiennent des valeurs discretes et continue
* le quartile
* la median
* la deviation
* etc

### La fonction drop

<h4><code>df.drop([colonne1, colonne2, ...])</code></h4>

Cette fonction permet d'éliminer les colonnes dont nous desirons exclure de notre analys.
Elle prend également le paramètre **inplace** qui a pour **True** ou **False** qui pour rôle de supprimer directement sans créer de nouvelle variable.

### La fonction dropna()

<h4><code>df.dropna(axis=0)</code></h4>

dropnan() permet de supprimer les valeurs manquant dans un dataset **dataframe**, le paramètre **axis** est obligatoire et il prend les valeurs **0** pour faire la suppression selon les lignes et **1** selon  les colonnes.

## La fonction value_counts()
elle compte le nombre de répétition de chaque valeurs dans une colonne.

## La fonction groupby()
Cette fonction, nous permet de faire des analyse par groupe 
## L'attribut shape
il permet de renvoyer le nombre de ligne et le nombre de colonne d'un **dataframe** sous forme d'un tuple

## L'attribut columns
cet attribut nous permet de lister toutes les colonnes d'un **dataframe**

## L'attribut plot
nous permet de générer les graphique sur un **dataframe**

* df.plot.scatter()
* df.plot.bar()
* df.plot.hist()
* etc

## DataFrame et Series
Dans pandas, il existe deux structures de données:

* DataFrame
* Serie

## Series
Une **Serie** est une colonne dans un **DataFrame** dont est associé un index à chaque valeur donc une sorte de dictionnaire **clée-valeur**

## DataFramme
Un **DataFrame** est un ensemble de **Series** donc un dataframe est un dictionnaire dont les clés sont les colonnes et les valeurs sont les **Series**

## Les opérations sur les dataframes
En pandas nous pouvous faire des **indexing** et du **boolean indexing** à travers **iloc** et **loc** 

* iloc: pour dire **index location**
* loc: pour dire **location**
