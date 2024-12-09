*==Installazione e configurazione di Fedora.==*

  
  

Tomelleri Mirko 4 FI

  
  
  

1. ==scaricare iso di Fedora server==
    
Dopo aver fatto l’accesso sul sito di fedora, ho installato il file ISO di Fedora (40) server.

  
2. ==verificare l’integrità dell’immagine scaricata, usando esclusivamente comandi a riga di powershell==


![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfuVDu81ANQzvS2OgWqtssJLVntMysVHu0APaVNYic3eOAoLzX2TEXHgdKxa09676RqCoAbl80VzQyVrSrioiFItOTQpL6ZCh9sqX4aTVLgLI08MTxx27KPjD2AHBFlVwq4KTDq-hBK0pAeaoRTb4JiiSFV?key=dtm-wrGnLXpr98L4boVUMQ)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe-yCFcm56jP0Sl1Ggc7VmqkEUgUr1BfBFeAFRrs1TO-FhRYJGi3Hb8EC59YAZJxdpa5OrOkiql6gK_hXasbuFq4xq1TD6jtS0R87a5ASk6KoSE-7JzaO5tv61WU-_ozSjIsRWDU0uhF8sHQl5HcWzQ-bX2?key=dtm-wrGnLXpr98L4boVUMQ)

  
In questo passaggio ho verificato tramite la PowerShell di Windows che il file scaricato precedentemente non fosse corrotto.

Se il risultato dell’algoritmo dà lo stesso risultato, il file è sicuro.

  

3. ==cercare requisiti di sistema sul sito ufficiale di Fedora==
    
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd8ulKWx20DiFkV3RKs0bfNyFaSH3UGL0uNdJVj-tXUuPcsUvjaIQSHQCur-Rebs-1t5nxg23mtEvlVETcEfqngXENzjgdDW9rbEMnaxVeMKyzIKtzUi3oxsAd9Y6GwFQGzSphMSzZzSU8HtjIrLQ5ufY_J?key=dtm-wrGnLXpr98L4boVUMQ)


4. ==pianificare le caratteristiche HW della macchina virtuale (2 * CPU min; 1,5 * RAM min; 2,5 * HDD min)==
    

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdcH9QZBPwXdzFC5TEy38RvzUotNmEdlUb7JW35A-a0-FUJkOciBpSCO-bRc4x_lDs8B_DzAu7wBIqHL6_jiAJ8nlJtYhAhOqQo9_PlF_KhOrE_GnXUqKOuS96x3YABbEnsoCHUpymZScluD8KPR-pf6o4M?key=dtm-wrGnLXpr98L4boVUMQ)

  
  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeptPe3dhIxdXDW7UhyjXyy8QcVaH5xp5cjMLCoJnBmWREoiVhF8i7jZztbx6cdlYXfWh9SRT7syOOTuFBNEeqEvsmB45tYBr4NEpHxVHXTzcp2RKr2ywtAYrh5W2njFyX0qeOWVi7WtHrSgPPOTSKZ-Sg?key=dtm-wrGnLXpr98L4boVUMQ)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfAXqx8Wrcrg10WzJHX-QBC8U06dudvX_gQsX6DyzBH77OKfoOx8Uh1KJTg5r-nU8jJvZlXZ2XG5qwPzoMVyG5BSd8LWt-dyDTl7j2nEBArB6DAHhcqoZUS4XK37ST8zswMJ25U5LBVcJjg2m48hkQFPhU5?key=dtm-wrGnLXpr98L4boVUMQ)

  
Qui sono andato a configurare le caratteristiche hardware della macchina virtuale, in base ai requisiti minimi richiesti.


5. ==usare lo schema di partizioni del disco GPT==

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXciDIgJXcEzSixr_zy8A_6ps5EoOzVOF8SwLaD0QLoeIzTPjUd7XEu3FWYiWbJ_hqY-4GKOZb0c_mSYTkli4ZDTDlY04osEX0OpBS_Is2uY0-XfU0CcfBBPZ_J_aNkV_nlhhU5EXFcEYOj7DeQWXc1TrAvy?key=dtm-wrGnLXpr98L4boVUMQ)

  
  

Nel mio caso, con il computer personale, l’unico disco disponibile è ATA VBOX HARD DISK, nei computer scolastici dovrebbe essere presente il disco GPT.
  

6. ==creare tante partizioni quanti sono i punti di mount essenziali e fare il fine fitting==
    
7. ==prevedere una partizione aggiuntiva per lo swap==
    

8. ==formattare ogni partizione in BTRFS==
    
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcjhllUHWqE6eaM95bLL38Dce_ovt1qppmWwJkqyaWJOtc5xaXsaS518Oko0q2t613Vk4fUGiqTmUm8glW_1Xb0Vcr8LQ4QxHoFl63D6KiKYmQRewkxDJVvlBrhA0RPO9AqHhnca4RI1Iz3os2Jwr-PvoE?key=dtm-wrGnLXpr98L4boVUMQ)

  
In questo passaggio ho creato delle partizioni per quanti sono i punti di mount essenziali.

  
  

9. ==installare il SO Fedora scaricato==
    
Dopo aver configurato la macchina virtuale (creazione user, password….), ho effettuato l'installazione del sistema operativo.

  
  
  
  

10. ==fare aggiornamenti del Packet Manager==
    
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcFMyt6q_s9GgZkVzyWA3YFemA8zw9ULqPwsT-zMJS4iLhAMecWT6BnUnBgDoLdGgAzYudDJOmxGlIUim4cyJvZJkT1oB87usUEm2PUg5icpsEe3Z6QRu_ogHyo3A8K_GkksZRgUIvn9JO0xnAlY5RtjCwt?key=dtm-wrGnLXpr98L4boVUMQ)

  

In questo ultimo passaggio, ho effettuato gli aggiornamenti del Packet Manager, utilizzando il comando: sudo dnf update.