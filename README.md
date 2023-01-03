# Analyse_Donnee
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SMJB4015/Analyse_Donnee.git/main?labpath=index.ipynb)
### :file_folder: Projet : Forex DataSet (EURUSD Pair)
![Forex](Images/Forex.jpg)

Le marché des changes est un marché mondial décentralisé ou de gré à gré pour le commerce des devises. Ce marché détermine les taux de change pour chaque devise. Il comprend tous les aspects de l'achat, de la vente et de l'échange de devises à des prix courants ou déterminés
### EURUSD Pair

L'EUR/USD est le ticker forex qui indique aux traders combien de dollars américains sont nécessaires pour acheter un euro. La paire euro-dollar est populaire auprès des traders car ses constituants représentent les deux économies les plus importantes et les plus influentes du monde.
#### Install the requirements

> - Install the pandas library using command pip install pandas.
> - Install the numpy library using command pip install numpy.

```import pandas as pd```

```import numpy as np```

```import seaborn as sns```

```import matplotlib.pyplot as plt```

#### Importation de DataSet

| Date       	| open   	| high   	| low    	| close  	| volume 	|
|------------	|--------	|--------	|--------	|--------	|--------	|
| 1971-01-04 	| 0.5369 	| 0.5369 	| 0.5369 	| 0.5369 	| 1      	|
| 1971-01-05 	| 0.5366 	| 0.5366 	| 0.5366 	| 0.5366 	| 1      	|
| 1971-01-06 	| 0.5365 	| 0.5365 	| 0.5365 	| 0.5365 	| 1      	|
| 1971-01-07 	| 0.5368 	| 0.5368 	| 0.5368 	| 0.5368 	| 1      	|
| 1971-01-08 	| 0.5371 	| 0.5371 	| 0.5371 	| 0.5371 	| 1>     	|

:small_orange_diamond: Date = c'est la date de Debut de Bar de 4H.
:small_orange_diamond: Open = c'est le prix d'ouverture .
:small_orange_diamond: Close = c'est le prix de fermeture .
:small_orange_diamond: Low = c'est le prix le plus bas de la Bar .
:small_orange_diamond: Volume = c'est le Volume totale de bar .

Ensuite, on utilise ```.tail``` pour observer les 5 derniers lignes de DataSet, on obtient ceci:

| Date       	| open    	| high    	| low     	| close   	| volume 	|
|------------	|---------	|---------	|---------	|---------	|--------	|
| 2019-05-01 	| 1.12148 	| 1.12644 	| 1.11867 	| 1.11941 	| 52561  	|
| 2019-05-02 	| 1.11942 	| 1.12187 	| 1.11703 	| 1.11709 	| 59203  	|
| 2019-05-03 	| 1.11710 	| 1.13236 	| 1.11346 	| 1.13234 	| 62828  	|
| 2019-05-08 	| 1.11922 	| 1.11927 	| 1.11892 	| 1.11920 	| 698    	|
| 2019-05-09 	| 1.11902 	| 1.11985 	| 1.11860 	| 1.11903 	| 12844> 	|

Ensuite, on utilise ```.shape``` pour observer avoir les dimensions de DataSet, on obtient ceci:

((12115, 5))

12115 lignes et 5 colones
Puis, on utilise ```.info``` pour consulter les details de DataSet, on obtient ceci:

 #   Column  Non-Null Count  Dtype  
---  ------  --------------  -----  
 0   open    12115 non-null  float64
 1   high    12115 non-null  float64
 2   low     12115 non-null  float64
 3   close   12115 non-null  float64
 4   volume  12115 non-null  int64  
dtypes: float64(4), int64(1)
