
Tecniche di gestione della memoria CI SONO TRE TECHINICHE DI GESTIONE CE LA PAGINAZIONE LA SEGMENTAZIONE E PAGINAZIONE CON SEGMENTAZIONE ognuno di questo ha i suoi vantaggi e svantaggi
## 1. Paginazione
La memoria è divisa in blocchi di dimensione fissa chiamati **pagine** (memoria logica) e **frame** (memoria fisica).

### **Vantaggi**
- **Elimina la frammentazione esterna**: La memoria è suddivisa in blocchi di dimensioni uguali.
- **Facilita l'allocazione**: Blocchi di memoria fissa sono più semplici da gestire.
- **Supporta il multitasking**: Pagine di processi diversi possono coesistere nella memoria.

### **Svantaggi**
- **Frammentazione interna**: Se un processo non utilizza completamente una pagina, si spreca spazio.
- **Traduzione complessa**: Richiede una tabella delle pagine e calcoli aggiuntivi per la conversione logica-fisica.
- **Overhead nella gestione**: La tabella delle pagine può occupare molta memoria.

---

## 2. Segmentazione
La memoria è divisa in blocchi logici chiamati **segmenti**, ciascuno corrispondente a una parte specifica di un programma (es., codice, dati, stack).

### **Vantaggi**
- **Separazione logica**: Ogni segmento ha un significato specifico, facilitando l’organizzazione del programma.
- **Supporto alla modularità**: Segmenti possono essere sviluppati e gestiti indipendentemente.
- **Protezione e condivisione**: Segmenti possono essere protetti o condivisi tra processi.

### **Svantaggi**
- **Frammentazione esterna**: Segmenti di dimensioni variabili possono lasciare spazi inutilizzati nella memoria.
- **Overhead di gestione**: È necessario mantenere una tabella dei segmenti per ciascun processo.
- **Traduzione lenta**: Ogni accesso alla memoria richiede una traduzione tramite la tabella dei segmenti.

---

## 3. Segmentazione con paginazione
Combina le due tecniche: ogni segmento è ulteriormente diviso in pagine di dimensioni fisse.

### **Vantaggi**
- **Riduzione della frammentazione esterna**: Le dimensioni fisse delle pagine eliminano il problema della frammentazione esterna.
- **Separazione logica**: I segmenti mantengono la semantica logica del programma.
- **Maggiore efficienza**: La paginazione all'interno dei segmenti ottimizza l’uso della memoria.

### **Svantaggi**
- **Complessità elevata**: Richiede sia una tabella dei segmenti sia una tabella delle pagine, aumentando l’overhead.
- **Overhead di traduzione**: La traduzione degli indirizzi è più complessa e richiede più passaggi.
- **Maggiore consumo di memoria**: Le tabelle occupano ulteriore spazio nella memoria.

per vare più dettagli della gestione memoria ce la pagina [[gestione memoria]], se vuoi informarti anche sui precessi ce [[gestione dei processi]]


---
