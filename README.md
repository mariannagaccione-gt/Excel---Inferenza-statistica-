#  Luggnagg Population Simulation & Statistical Analysis Suite

[![Excel](https://img.shields.io/badge/Microsoft%20Excel-Interactive%20Workbook-green?logo=excel)](https://microsoft.com/excel)
[![Status](https://img.shields.io/badge/Status-Completed-success)]()
[![Domain](https://img.shields.io/badge/Domain-Applied%20Statistics%20&%20Data%20Analytics-blue)]()

##  Panoramica del Progetto
Questo repository contiene un workbook Excel avanzato e interamente dinamico, sviluppato come progetto finale per il Master in Data Analytics. 

L'obiettivo del progetto è la creazione di un **ambiente di apprendimento e simulazione statistica autoprodotto** (privo di dati reali o sensibili) destinato al rinnovamento del modulo introduttivo di *Statistica Applicata* di un'Academy. Il file simula la popolazione immaginaria di **"Luggnagg"** e permette ai docenti e agli studenti di testare in tempo reale l'impatto della variazione dei parametri statistici sulle distribuzioni e sui modelli.

---

##  Architettura del Workbook
Il file Excel è strutturato in **6 schede interconnesse**, progettate per garantire che ogni cella contenga esclusivamente formule vive (nessun valore statico incollato), permettendo il ricalcolo automatico in tempo reale:

1. **Parameters** 
   * *Funzione:* Pannello di controllo centralizzato.
   * *Contenuto:* Input utente per la configurazione dinamica di probabilità, medie e deviazioni standard che alimentano l'intero modello.
2. **Data** 
   * *Funzione:* Generazione della popolazione sintetica.
   * *Contenuto:* Dataset di **250 individui**. In Colonna A sono generate le età tramite distribuzione normale; in Colonna B è associato casualmente un gruppo di appartenenza (valori interi da 1 a 4).
3. **Sample** 
   * *Funzione:* Campionamento condizionale.
   * *Contenuto:* Estrazione di un sotto-campione mirato tramite funzioni logiche (`SE` e filtri condizionali) basate sullo specifico gruppo di appartenenza.
4. **Statistical Insight** 
   * *Funzione:* Cruscotto di analisi descrittiva e inferenziale.
   * *Contenuto:* Calcolo di deviazione standard, valore atteso (media), conteggio, livello di confidenza, stima del parametro $p$ e relativo intervallo di confidenza. Include una cella di testo dinamica per il commento automatico dei risultati.
5. **(Un)correlated Variables** 
   * *Funzione:* Analisi bivariata e correlazione.
   * *Contenuto:* Affiancamento dei dati del campione a due variabili casuali simulate (numero di gatti posseduti ed età del partner), con calcolo dei coefficienti di correlazione e relativo commento analitico.
6. **Linear Regression** 
   * *Funzione:* Modellazione predittiva.
   * *Contenuto:* Analisi di regressione lineare tra la variabile dipendente $Y$ (età) e indipendente $X$ (ordine di censimento). Il foglio include uno scatterplot con retta di regressione interpolata e la stima puntuale riferita al partecipante 160.

---

##  Linee Guida di Formattazione Didattica
Oltre al rigore statistico, il workbook pone una particolare attenzione alla **data literacy e alla leggibilità visiva** (best practice di data visualization):
* **Intestazioni:** Righe e colonne di intestazione formattate uniformemente (Font personalizzato, colore blu, bordi doppi) per una chiara gerarchia visiva.
* **Griglia Dati:** Celle dei valori racchiuse da bordi sottili per facilitare la lettura tabellare.

---

##  Come Utilizzare il File
1. Clona il repository o scarica il file Excel (`.xlsx`) dalla root.
2. Apri il file in Microsoft Excel (o in un software compatibile che supporti le formule avanzate).
3. Naviga nel foglio **Parameters** e modifica i valori di input (media, deviazione standard, probabilità).
4. Osserva come l'intero sistema (dalle distribuzioni alla regressione lineare) si aggiorni istantaneamente grazie alle formule dinamiche.

---

##  Competenze e Strumenti Dimostrati
* **Statistica Descrittiva e Inferenziale:** Teoria dei campioni, intervalli di confidenza, stima di parametri.
* **Modellazione in Excel:** Funzioni logiche avanzate (`SE`), gestione dei parametri dinamici, correlazione e regressione lineare con grafici scatter.
* **Data Storytelling & UX:** Struttura modulare orientata alla didattica e alla leggibilità professionale dei dati.
