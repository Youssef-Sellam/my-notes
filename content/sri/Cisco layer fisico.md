



## **4.1 - Ruolo del Livello di Trasporto**
### Funzioni principali
- **Segmentazione e riassemblaggio**: I dati vengono divisi in segmenti e riassemblati alla destinazione.
- **Identificazione delle applicazioni**: Utilizza numeri di porta per distinguere le applicazioni.
- **Affidabilità**: Fornisce meccanismi per garantire la consegna dei dati (opzionale).

### Servizi principali
- **Affidabilità (TCP)**: Conferme di ricezione e ritrasmissioni.
- **Velocità (UDP)**: Nessun controllo di consegna, adatto per applicazioni in tempo reale.

---

## **4.2 - Protocolli del Livello di Trasporto**
### **Transmission Control Protocol (TCP)**
- Orientato alla connessione.
- Garantisce l'ordinamento e la consegna completa dei dati.
- Utilizza:
  - **Handshake a tre vie**: Stabilisce una connessione sicura.
  - **Controllo del flusso**: Gestisce il volume dei dati inviati.
  - **Ritrasmissioni**: Corregge gli errori.

### **User Datagram Protocol (UDP)**
- Senza connessione e non affidabile.
- Adatto per:
  - DNS
  - Streaming video
  - Applicazioni VoIP
- **Ridotto overhead**: Maggiore velocità ma senza garanzie.

---

## **4.3 - Multiplexing e Numeri di Porta**
### Multiplexing
- Permette la comunicazione simultanea di più applicazioni su una rete.
- Identifica le applicazioni tramite i numeri di porta.

### Classificazione dei numeri di porta
- **Porte conosciute (0-1023)**: Per servizi standard (es. HTTP, HTTPS).
- **Porte registrate (1024-49151)**: Per applicazioni personalizzate.
- **Porte dinamiche (49152-65535)**: Utilizzate temporaneamente durante una sessione.

---

## **4.4 - Gestione delle Connessioni TCP**
### Fasi della connessione TCP
1. **Handshake a tre vie**:
   - Stabilisce una connessione affidabile tra mittente e destinatario.
   - Sequenza:
     1. SYN
     2. SYN-ACK
     3. ACK
2. **Trasferimento dati**:
   - Garantisce l'ordinamento dei segmenti.
   - Verifica l'integrità con gli ACK.
3. **Terminazione**:
   - Chiude la connessione con una sequenza di FIN e ACK.

### Controllo del flusso
- Previene il sovraccarico del destinatario.
- Regola la quantità di dati trasmessi tramite la **finestra di ricezione**.

---

## **4.5 - Applicazioni che utilizzano UDP**
- **Vantaggi**:
  - Velocità.
  - Ridotto overhead.
- **Svantaggi**:
  - Nessuna garanzia di consegna o di ordine.
- **Applicazioni tipiche**:
  - DNS: Traduzione di nomi di dominio.
  - Streaming: Video e audio in tempo reale.
  - VoIP: Chiamate vocali.

---
