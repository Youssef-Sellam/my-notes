
La **gestione della memoria** è una funzione fondamentale del sistema operativo che si occupa di allocare, monitorare e gestire la memoria principale (RAM) per i programmi e i processi in esecuzione.

---

## Componenti e Funzionalità Chiave

1. **Program Counter**:  
   Mantiene l'offset del programma per eseguire il prossimo comando.

2. **MMU (Memory Management Unit)**:  
   Traduce indirizzi logici in indirizzi fisici, gestendo la memoria disponibile per i processi e la memoria occupata dal sistema operativo.

3. **Multiprogrammazione**:  
   Permette di avere più processi in memoria per ridurre i tempi di "context switching" (scambio dei registri dei processi tra CPU).

---

## Allocazione della Memoria

### Allocazione Contigua
- **Partizione Fissa**:  
  La memoria è divisa in partizioni di dimensioni fisse.  
  - **Frammentazione Esterna**: Spazi di memoria inutilizzati perché non abbastanza grandi per nuovi processi.  
  - **Frammentazione Interna**: Spazio inutilizzato all'interno delle partizioni, se troppo grandi rispetto ai processi.

### Allocazione Non Contigua
- **Segmentazione**:  
  Divide la memoria in segmenti logici, ciascuno rappresentante una struttura logica del programma.  
- **Paginazione**:  
  Divide la memoria in pagine fisiche e logiche di dimensione fissa, riducendo la frammentazione.

---

## Memoria Virtuale

- Permette di eseguire programmi più grandi della memoria fisica disponibile.
- Carica solo porzioni di programmi in memoria, mantenendo il resto su disco.
- **Page Fault**: Si verifica quando una pagina necessaria non è in memoria e deve essere caricata dal disco.

---

## Mapping tra Indirizzi Logici e Fisici

1. **Rilocazione Dinamica**:  
   Gli indirizzi logici generati dal processo vengono tradotti dalla MMU in indirizzi fisici al momento dell’esecuzione.

---

## Compilazione e Linking

1. **Compilazione**:  
   Trasforma il codice sorgente in codice eseguibile.  
2. **Linking**:  
   Combina vari moduli compilati in un singolo eseguibile.  
   - **Static Linking**: Gli indirizzi sono fissati prima dell’esecuzione.  
   - **Dynamic Linking**: Gli indirizzi vengono risolti durante l’esecuzione.

---

## Tecniche di Ottimizzazione della Memoria

1. **Swapping**:  
   I processi inattivi vengono spostati su disco per liberare spazio nella RAM.  
2. **Overlay**:  
   I programmatori dividono il codice in moduli caricati solo al bisogno.  
3. **Caricamento Dinamico**:  
   Le porzioni di programma vengono caricate solo quando necessarie.

---

## Sistemi Ibridi: Segmentazione con Paginazione
- Combina segmentazione e paginazione per ridurre la frammentazione interna ed esterna. se ne parla anche nelle [[tecniche di gestione della memoria]] ci sono anche paginazione  e segmentazione 
- Indirizzi logici organizzati come tripla `(s, p, d)`:
  - `s`: Segmento.  
  - `p`: Pagina.  
  - `d`: Offset.  

- Indirizzi fisici risultanti: coppia `(f, d)`:
  - `f`: Frame.  
  - `d`: Offset.  

Questa combinazione garantisce maggiore efficienza e flessibilità nella gestione della memoria.

---