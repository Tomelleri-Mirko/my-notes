
==Programma vs Processo==

- *Programma*:  insieme di istruzioni, memorizzato su memoria di massa
- *Processo*:  istanza di programma in esecuzione, risiede in RAM

==Sistemi Operativi Multitasking==

- *Scheduling dei job*:  strategie per scelgliere i programmi da caricare in RAM
- *Scheduling della CPU*:  strategie per assegnare o sospendere l'utilizzo della CPU

==Processi==

- *Codice*
- *Dati del programma*

L'insieme di tutti i dati si chiama ***contesto del processo**.*

- *Indipendenti:*  evolvono senza scambio di dati
- *Cooperanti:*  evolvono scambiandosi dati a vicenda
- *Competitori:*  si ostacolano l'evoluzione a vicenda

==Stati di un processo==

- *New*: appena creato
- *Ready:* ha tutte le risorse tranne la CPU
- *Running*: quando viene eseguito
- *Waiting*: gli manca una risorsa occupata
- T*erminated*: ha concluso

==Descrittore di processo==

Traccia le operazione che svolge un processo ed è chiamato PD oppure PCB.
Contiene:
- *PID*
- *Program Counter*
- *Registri*
- *Priorità*
- *Puntatori alla memoria del processo*
- *Puntatori  alle risorse allocate al processo*