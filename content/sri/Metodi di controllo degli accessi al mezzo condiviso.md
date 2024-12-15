

- Accesso basato sul meccanismo di contesa:  
    Tutti i nodi della rete operano in half-duplex, in competizione per l'uso del supporto.  
    Esempi:
    

- CSMA/CD (Ethernet).
    
- CSMA/CA (WLAN).
    

- Accesso controllato: Ogni nodo ha il proprio tempo per utilizzare il mezzo. Esempio: Token Ring.
    

---

Controllo di accesso al mezzo: CSMA/CD  
Lo standard IEEE 802.3 utilizza il protocollo CSMA/CD, che prevede la contesa del mezzo per l'accesso:

1. Fase 1 - CSMA: Una stazione ascolta prima di trasmettere. Se il canale è libero, trasmette.
    
2. Fase 2 - CD: Se si verifica una collisione, la stazione smette di trasmettere, attende un tempo casuale e riprova.
    

---

Frame Ethernet

- La dimensione minima è 64 byte, la massima è 1518 byte.
    
- I frame più piccoli di 64 byte sono considerati frammenti di collisione e vengono scartati.
    
- I frame più grandi di 1500 byte sono "jumbo" e vengono scartati se non supportati.
    

---

Reti WLAN e standard IEEE 802.11

- Una WLAN usa dispositivi radio (Access Point - AP) per trasmettere segnali.
    
- BSS: Basic Service Set, composto da uno o più AP.
    
- ESS: Extended Service Set, formato da più BSS per aumentare la copertura.
    
- SSID: Identifica una rete WLAN.
    

Protocollo CSMA/CA:

- Le stazioni ascoltano prima di trasmettere e si astengono se il canale è occupato.
    
- Utilizza i messaggi RTS (Request To Send) e CTS (Clear To Send) per evitare collisioni.
    
