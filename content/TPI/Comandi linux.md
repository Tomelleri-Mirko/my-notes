
# **Elenco dei comandi Linux - Lab 10**

  

## **1. Comandi di Redirect e Output**

- **`echo "Hello World"`** → Stampa una stringa sulla riga di comando.

- **`echo "Hello World" > mymessage`** → Reindirizza l'output in un file (sovrascrivendo il contenuto precedente).

- **`echo "Greetings" >> mymessage`** → Aggiunge l'output a un file senza sovrascrivere il contenuto.

- **`cat mymessage`** → Visualizza il contenuto di un file.

- **`find /etc -name hosts 2> err.txt`** → Reindirizza gli errori (`stderr`) in un file separato.

- **`find /etc -name hosts > std.out 2> std.err`** → Separa stdout e stderr in due file diversi.

- **`find /etc -name hosts > find.out 2>&1`** → Unisce stdout e stderr in un unico file.

  

## **2. Comandi di Ricerca e Filtraggio**

- **`find ~ -name "*bash*"`** → Cerca file che contengono la parola "bash" nella home directory.

- **`grep sshd passwd`** → Cerca la stringa "sshd" all'interno del file `passwd`.

- **`grep '^root' passwd`** → Cerca le righe che iniziano con "root".

- **`grep 'sync$' passwd`** → Cerca le righe che terminano con "sync".

- **`grep -E 'sshd|root|operator' passwd`** → Cerca una delle tre parole specificate nel file `passwd`.

- **`egrep 'no(b|n)' passwd`** → Usa un'espressione regolare per cercare le parole "nob" o "non".

- **`grep '[0-9]{3}' passwd`** → Cerca stringhe contenenti almeno tre numeri consecutivi.

  

## **3. Comandi per Manipolare il Contenuto di File**

- **`tr a-z A-Z`** → Converte il testo da minuscolo a maiuscolo.

- **`tr A-Z a-z > myfile`** → Converte il testo in minuscolo e lo salva in un file.

- **`tr a-z A-Z < myfile`** → Converte il contenuto di un file in maiuscolo.

  

## **4. Comandi per Visualizzare File di Testo**

- **`ls -l /etc | more`** → Mostra il contenuto di `/etc` una pagina alla volta.

- **`cut -d: -f1 /etc/passwd`** → Estrae la prima colonna del file `/etc/passwd`.

- **`cut -d: -f1 /etc/passwd | sort`** → Ordina l'output del comando precedente.

- **`cut -d: -f1 /etc/passwd | sort | more`** → Mostra l'output ordinato una pagina alla volta.

- **`cat /etc/passwd`** → Mostra l'intero contenuto del file `/etc/passwd`.

- **`more /etc/passwd`** → Mostra il contenuto del file una pagina alla volta.

- **`less /etc/passwd`** → Come `more`, ma con più funzioni di navigazione.

- **`head /etc/passwd`** → Mostra le prime 10 righe del file.

- **`tail /etc/passwd`** → Mostra le ultime 10 righe del file.

- **`head -2 /etc/passwd`** → Mostra solo le prime 2 righe.

- **`ls /etc | tail -5`** → Mostra gli ultimi 5 file nella directory `/etc`.

- **`head -n -20 /etc/passwd`** → Mostra tutte le righe tranne le ultime 20.