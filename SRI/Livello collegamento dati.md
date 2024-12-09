### *Metodi di controllo degli accessi al mezzo condiviso*

#### ==Comunicazioni half-duplex e full-duplex==

- Comunicazione half-duplex : I dispositivi possono trasmettere o ricevere segnali, ma non contemporaneamente. Questo tipo di comunicazione è tipico delle reti WLAN e delle topologie di bus legacy con hub Ethernet.
    
- Comunicazione full-duplex : consente di inviare e ricevere dati simultaneamente, una caratteristica fondamentale degli switch Ethernet moderni.
    

  

### ==Metodi di controllo degli accessi==

Le reti LAN Ethernet e WLAN utilizzano due approcci principali per gestire l'accesso ai mezzi condivisi:

- Accesso basato sulla contesa : Questa modalità, utilizzata in modalità half-duplex, consente la trasmissione a un solo dispositivo alla volta.
    

- CSMA/CD (Carrier Sense Multiple Access/Collision Detection) : Metodo usato nelle reti Ethernet legacy, in cui i dispositivi rilevano e gestiscono le collisioni.
    
- CSMA/CA (Collision Evitare) : Metodo adottato nelle LAN wireless, che si concentra sulla prevenzione delle collisioni.
    

- Accesso controllato : Sistema deterministico in cui ogni dispositivo ha un turno predefinito per la trasmissione. Un esempio storico è il protocollo Token Ring.
    

  

### ==Controllo di accesso al mezzo: CSMA/CD==

Lo standard IEEE 802.3 implementa il protocollo CSMA/CD per minimizzare le collisioni:

1. Rilevazione della portante : Prima di trasmettere, i dispositivi si verificano se il canale è libero.
    
2. Rilevazione delle collisioni : In caso di collisione, la trasmissione viene sospesa e riprogrammata dopo un intervallo di tempo casuale.
    

  

### ==Frame Ethernet==

- Dimensione del frame : Deve essere compresa tra un minimo di 64 byte e un massimo di 1518 byte.
    
- Validità dei frame : Frame troppo piccoli o troppo grandi vengono scartati.
    
- Ogni frame include indirizzi MAC, dati trasmessi e il campo FCS (Frame Check Sequence) per il controllo degli errori.
    

  

### ==Reti WLAN e standard IEEE 802.11==

Le reti WLAN, basate sullo standard IEEE 802.11, utilizzano Access Point (AP) per offrire connettività wireless con un raggio tipico di circa 100 metri. Gli AP aziendali si distinguono per una maggiore copertura e funzionalità avanzate rispetto a quelli domestici.

  

### ==Architettura 802.11==

- Connessione wireless ad-hoc : consiste in collegamenti diretti tra dispositivi, formando un IBSS (Independent Basic Service Set).
    
- Connessione con Access Point (AP) : Gli AP consentono il collegamento dei dispositivi wireless a una rete cablata, creando un BSS (Basic Service Set). Per estendere la copertura, è possibile collegare più AP, creando un ESS (Extended Service Set).
    

  

### ==Area di copertura Wi-Fi==

La copertura Wi-Fi può essere influenzata da ostacoli fisici. I materiali come cemento armato riducono significativamente il segnale, mentre legno e vetro hanno un impatto trascurabile. Inoltre, la velocità di trasmissione più elevata può causare maggiori interferenze.

  

### ==Protocollo CSMA/CA==

Il protocollo CSMA/CA, adottato nelle WLAN, evita le collisioni con un approccio proattivo:

- Prima di trasmettere, il dispositivo verifica che il canale sia libero.  

- Se il canale è occupato, il dispositivo attenderà un intervallo casuale prima di riprovare.                                                                                                                        
- Viene utilizzato il sistema RTS/CTS per coordinare la trasmissione e prevenire problemi.
    

  

### ==Problema del terminale nascosto: RTS e CTS==

Il meccanismo RTS (Request To Send) e CTS (Clear To Send) risolve il problema dei terminali nascosti, garantendo che un solo dispositivo alla volta possa trasmettere. Questo approccio evita collisioni e ottimizza l'utilizzo del canale.