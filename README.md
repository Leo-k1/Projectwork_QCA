# Project Work QCA

## Massimizzazione domanda e offerta
Il problema riguarda la massimizzazione del valore netto delle transazioni (acquisto – vendita) con la conseguente realizzazione del prezzo di equilibrio in un sistema di aste che potrebbe abbracciare diversi settori di mercato. Nel caso in cui l’acquisto o la vendita dovesse riguardare utility, si dovrebbe considerare anche la variabile relativa al costo del trasporto. 

## Funzione Obiettivo
Per la determinazione di un prezzo di equilibrio tra domanda ed offerta, la funzione obiettivo dovrà massimizzare le differenze tra le quantità di buy e di sell considerando le penalità dovute alle distanze tra le aree. Non tutte le aree sono relazionate tra di loro ed i canali di comunicazione tra aree sono monodirezionali. L’eventuale collegamento bidirezionale tra A e B potrebbe essere realizzabile con due canali monodirezionali che potenzialmente potrebbero avere capacità differenti come mostrato nell’esempio di seguito: <p align="center"> <img alt="1" src="https://github.com/Leo-k1/ProjectWork_QCA/blob/main/Schema.png?raw=true" width="30%"> </p>

## Vincoli:
-  Le quantità relative alle offerte di acquisto e di vendita di ogni area dovranno essere
positive e limitate ad una quantità massima.
-  La somma complessiva delle quantità di acquisto deve essere uguale alla somma delle quantità di vendita $$\sum_{a=1}^{n_a} \left[\sum_{ob=1}^{n_{ob,a}} Q_{ob,z}^{buy} - \sum_{os=1}^{n_{os,a}} Q_{os,z}^{sell}\right]$$
- Ciascuna interconnessione avrà una capacità limitata: $$0 \leq t_{ij} \leq T_{ij}$$

Dove:
- A rappresenta l’insieme delle interconnessioni 
- $T_{ij}$ rappresenta la capacità massima di transito relativa all’interconnessione tra le aree $i$ e $j$ 
- $n_a$ il numero complessivo di aree di riferimento 
- $a$ è l’area che si sta considerando
- $n_{ob}$ numero complessivo di offerta di acquisto
- $b$ specifica offerta di acquisto
- $n_{os}$ numero complessivo di offerta di vendita
- $s$ specifica offerta di vendita 
