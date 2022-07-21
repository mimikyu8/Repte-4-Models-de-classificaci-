# Repte #4- Models de classificació
La meva proposta com a solució al repte [Repte #4](https://nuwe.io/challenge/repte-4-models-de-classificacio) de Data Science

## Background i descripció del repte
El càncer de mama és el més comú entre les dones del món. Representa el 25% de tots els casos de càncer i va afectar més de 2,1 milions de persones només el 2015. Comença quan les cèl·lules de la mama comencen a créixer de manera descontrolada. Aquestes cèl·lules solen formar tumors que es poden veure mitjançant raigs X o sentir-se com embalums a la zona del pit.
El dataset, que consta de 31 columnes i 455 files, conté dades de dones sanes i dones diagnosticades amb càncer de mama, així com certes característiques de cèl·lules que s'han pres durant una punció-aspiració d'agulla fina (PAAF). Recull deu característiques mesurades als nuclis cel·lulars en imatges preses després de la PAAF, que són:
* El radi (la mitjana de les distàncies del centre als punts del perímetre)
* La textura (la desviació estàndar dels valors de la escala de grisos)
* El perímetre
* L'àrea
* L'uniformitat (variació local de les longituts del radi)
* Compacitat ($\frac{perímetre^2}{àrea - 1} \\ $)
* Concavitat (gravetat de les parts còncaves del contorn)
* Punts còncaus (número de parts còncaves del contorn)
* Simetria
* Dimensió fractal

D'aquestes característiques, es recullen al dataset la mitjana (columnes acabades en \_mean), l'error estàndar (columnes acabades en \_se), i el pitjor valor, o el més gran (columnes acabades en \_worst). També es recull el diagnosi, amb un 0 si és benigne, i amb un 1 si és maligne. 
[font](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29)

## Arxius del repositori

  * __main.ipynb__: Notebook que recull tot el procés de seleccionar i crear el model per predir les dades.
  * __predictions.csv__: Arxiu csv que conté les prediccions calculades amb el millor model estudiat.
  * __requirements.txt__: Requeriments de llibreries, mòduls i paquest
  
  ## Models 
S'han provat quatre algoritmes de classificació, que són Random Forest, Logistic Regression, K Neighbors y Support Vector Machine, amb un escalat previ amb Rebust Sclaer, així com aplicant en alguns casos PCA.
