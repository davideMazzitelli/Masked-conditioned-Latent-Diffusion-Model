# Generazione ed Editing di Immagini sull’Inquinamento Ambientale

Progetto di Tesi Magistrale – Facoltà di Informatica, Università degli Studi di Milano-Bicocca

## 📖 Descrizione

Questo progetto ha come obiettivo lo sviluppo di un modello generativo per la creazione e modifica di immagini nel dominio dell’inquinamento ambientale.

La generazione delle immagini è condizionata da maschere semantiche, permettendo un controllo preciso sui contenuti visivi. Sono previsti sviluppi futuri per integrare funzionalità di image editing, consentendo di aggiungere o modificare elementi in immagini già esistenti.

## 🧰 Tecnologie e Metodi

- Modelli generativi basati su reti neurali (Unet + diffusion model).
- Maschere semantiche per il conditioning.
- Dataset utilizzato: TACO (Trash Annotations in Context).
- servizi di calcolo GPU in cloud come Kaggle e Google Colab.

## 📊 Dataset: 

### > TACO (Trash Annotations in Context)

TACO è un dataset open-source dedicato al rilevamento e segmentazione dei rifiuti in contesto reale. È composto da immagini annotate di rifiuti raccolte in ambienti urbani e naturali, utili per applicazioni di computer vision legate all’inquinamento ambientale.

Dimensioni: 
-  Oltre 1.500 immagini ad alta risoluzione e più di 7.000 oggetti annotati.
-  3.000 immagini aggiuntive provenienti dalle annotazioni “unofficial” condivise dalla community TACO, per ampliare la varietà e robustezza del training.

Annotazioni: Fornisce segmentazioni poligonali dettagliate e bounding box, organizzate in supercategorie e classi specifiche (ad es. plastica, metallo, carta, ecc.).

Formato: Le annotazioni sono in formato COCO JSON

### > Plastopol — A Dataset for Litter Detection
Dataset progettato per rilevare “litter” (rifiuti) in vari tipi di ambiente (marino, strade, altri contesti naturali), per supportare studi e modelli automatici di rilevamento dei rifiuti.

Classe singola (one-class): tutti gli oggetti annotati appartengono alla superclasse “litter” (cioè non è diviso in categorie dettagliate come plastica, carta, metallo, etc.).

Dimensioni: 2.418 immagini, circa 5.300 istanze di “litter”.

Annotazioni: bounding box rettangolari per ogni istanza di rifiuto (“litter”).

### > Garbage Detection (Roboflow)
Dataset per il rilevamento automatico di rifiuti in vari contesti ambientali, utile per addestrare modelli di object detection.

Dimensioni: Parte del dataset originale di 10.000 immagini, selezionata per il training e la validazione.

Annotazioni: Fornisce bounding box per diverse categorie di rifiuti.
