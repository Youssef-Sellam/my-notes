
---

  
Funzioni principali:

- Trasmissione di bit grezzi su un mezzo fisico.
    
- Converte i dati digitali in segnali elettrici, ottici o radio e viceversa.
    
- Specifica caratteristiche hardware come:
    

- Tipi di cavi (rame, fibra ottica, wireless).
    
- Connettori e pinout.
    
- Standard di velocità (es: 10 Mbps, 100 Mbps, 1 Gbps).
    

Componenti chiave:

- Mezzi trasmissivi:
    

- Rame (UTP, STP): utilizzato per Ethernet (es. CAT5e, CAT6).
    
- Fibra ottica: per alte velocità e lunghe distanze.
    
- Wireless: segnali radio (es. Wi-Fi, Bluetooth).
    

- Dispositivi: Hub, ripetitori, antenne, transceiver.
    
- Standard:
    

- IEEE 802.3 (Ethernet).
    
- ITU-T per fibra ottica.
    
- IEEE 802.11 (Wi-Fi).
    

Parametri principali:

- Larghezza di banda: capacità massima del mezzo trasmissivo.
    
- Attenuazione: perdita di segnale su lunghe distanze.
    
- Crosstalk: interferenza tra cavi adiacenti.
    

---

Livello di Collegamento Dati (Data Link Layer)  
Funzioni principali:

- Fornisce un trasferimento dati affidabile tra nodi adiacenti.
    
- Gestisce gli indirizzi MAC per l'identificazione dei dispositivi.
    
- Implementa la rilevazione e la correzione degli errori.
    

Suddiviso in due sotto-livelli:

- LLC (Logical Link Control): gestione delle connessioni logiche, controllo del flusso e identificazione dei protocolli.
    
- MAC (Media Access Control): controllo dell'accesso al mezzo e gestione degli indirizzi fisici.
    

Componenti chiave:

- Protocolli:
    

- Ethernet (IEEE 802.3).
    
- Wi-Fi (IEEE 802.11).
    
- PPP (Point-to-Point Protocol).
    

- Indirizzo MAC: identificativo unico a 48 bit (es: 00:1A:2B:3C:4D:5E).
    
- Frame:
    

- Preambolo: sincronizzazione.
    
- Indirizzo MAC di destinazione e sorgente.
    
- Payload: dati da trasmettere.
    
- FCS (Frame Check Sequence): verifica degli errori.
    

Modalità di accesso:

- CSMA/CD (Carrier Sense Multiple Access with Collision Detection): Usato nelle reti cablate Ethernet.
    
- CSMA/CA (Carrier Sense Multiple Access with Collision Avoidance): Usato nelle reti wireless.
    

Dispositivi principali:

- Switch: lavora al livello 2, utilizza MAC address per inoltrare i frame.
    
- Bridge: collega due segmenti di rete filtrando il traffico.
    

Tipi di Errori:

- Errori singoli: un bit corrotto.
    
- Burst errors: errori consecutivi su più bit.
    

Tecniche di correzione:

- CRC (Cyclic Redundancy Check).
    
- ARQ (Automatic Repeat Request).
    

---

Differenze principali tra Livello Fisico e Livello di Collegamento Dati

|   |   |   |
|---|---|---|
|Caratteristica|Livello Fisico|Livello di Collegamento Dati|
|Funzione|Trasmette segnali grezzi|Trasmette frame con dati strutturati|
|Unità di dati|Bit|Frame|
|Indirizzo|N/A|Indirizzo MAC|
|Dispositivi|Hub, ripetitori|Switch, bridge|
|Protocolli|Standard fisici (es: IEEE 802.3)|Ethernet, Wi-Fi, PPP|

  

---

  

