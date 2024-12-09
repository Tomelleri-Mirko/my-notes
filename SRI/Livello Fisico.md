  
Definizioni:

==campionamento:==  con campionamento si intende il convertire un segnale continuo, in un segnale discreto, misurando l’ampiezza del segnale a intervalli di tempo regolari.

Le ==caratteristiche== del campionamento sono:  la frequenza di campionamento, ovvero il numero di campioni estratti in un secondo dal segnale analogico; maggiore è la frequenza, maggiore è la precisione della cattura del segnale originale.

==Intervallo di campionamento==:  è il tempo che intercorre tra due misurazioni consecutive del segnale.

==Teorema di Nyquist e Shannon== : dice, che la frequenza di campionamento deve essere almeno il doppio della massima frequenza presente nel segnale analogico originale.

Ad esempio se la frequenza massima del segnale originale è 20 khz, la frequenza di campionamento deve essere 40 khz.

  

==quantizzazione==:  la quantizzazione è il passaggio successivo del campionamento, e consiste nella rappresentazione approssimata in bit di ogni segnale campionato.

I bit vengono presi da un sistema di n bit, es: un sistema di 8 bit avrà 256(0 - 255) livelli nel quale un campione può essere rappresentato.

Maggiore sono i bit utilizzati per la quantizzazione, maggiore è la precisione della rappresentazione del segnale.

  

==Codifica Manchester==:  intanto per codifica si intende il metodo di conversione del flusso di bit in uno schema che può essere riconosciuto sia dal mittente che dal destinatario.

Nella codifica manchester, un bit 0 equivale alla transizione da alta a bassa tensione, invece un bit 1 equivale alla transizione da bassa ad alta tensione.

Questa codifica viene utilizzata nei vecchi standard Ethernet, ad esempio 10BASE-T.

vantaggi: rilevamenti errori, transizione agisce come segnale di clock.

  

==DNS==:  è un protocollo, ( un insieme di regole prestabilite che permettono la comunicazione e definiscono l’ordine e il formato dei messaggi ) che traduce i nomi di dominio([www.esempio.it](http://www.esempio.it)) in indirizzi IP collegati ad una macchina.

Nella shell il comando per convertire i domini in IP è: nslookup url.

Processo di traduzione: il client fa richiesta al server DNS locale, che finché non trova risposta ovvero il dominio, inoltra la richiesta ad un server root dns che contiene una serie dii domini, ciascuno associato ad un indirizzo IP corrispondente ad un server DNS, il dominio utente viene confrontato ed una volta trovato il dominio giusto, si fornisce l’ip. 

  

==URI==:  è un identificatore di risorse e si divi in url, e urn.

- URL: è un uri che identifica una risorsa tramite la sua locazione in un grafo, ovvero in una rete geografica composta da archi e nodi (media di connessione e dispositivi di rete).

- URN: è un uri che identifica una risorsa tramite il nome, l’urn non cambia, e se la risorsa non c’è più lui rimane comunque lo stesso.

  
  

==RCF 894==: standard per realizzare comunicazioni con il cavo Ethernet.

  

==Livello fisico==:  è il livello più basso del modello ISO /OSI , che riceve dal livello data link un intero frame (un pacchetto di dati proveniente dal data link che contiene header, payload e crc ) e lo codifica in una serie di segnali che vengono trasmessi uno alla volta attraverso il mezzo trasmissivo.

  

==Larghezza di banda==:  misura la quantità di dati(bit) che possono essere trasmessi da un luogo ad un altro in un determinato periodo di tempo.

Se un cavo Ethernet supporta 10 Mbps ed un altro ne supporta 20, la velocità  non cambia, ma cambia la quantità di bit trasmessi.

  

==Latenza==:  è il tempo totale impiegato dai dati, per viaggiare da un punto ad un altro, comprendendo anche vari ritardi.

  

==Throughput==:  è la misura della velocità del trasferimento di bit attraverso i media in un periodo di tempo.

==Goodput==:  misura dei dati utilizzabili in un periodo di tempo, ed è sempre inferiore al throughput, che è a sua volta inferiore della larghezza di banda.

  

==Cavi di rame==:  i cavi di rame permettono la trasmissione di bit attraverso impulsi elettrici.

Ci sono 3 tipi:

- UTP:  tipo di cavo più comune, è intrecciato (per eliminare interferenze elettromagnetiche EMI, o interferenze da radiofrequenza RFI), ma non schermato(per la diafonia). Termina con un connettore RJ-45 ed è il meno costoso.
    
- STP:  è intrecciato e schermato, usa connettore RJ-45, ed è più costose dell’utp.
    
- Coassiale:  è un conduttore in rame circondato da uno strato isolante in plastica, a sua volta avvolto da una lamina metallica, a sua volta rivestita con una guaina per prevenire i danni fisici.I connettori possono essere BNC tipo N oppure tipo F.