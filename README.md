# Creare un backup di un sito WordPress
Come creare un backup su WordPress con Duplicator


#### Indice
[Installazione plugin](#duplicator)  
[Creazione di un duplicato](#procedura)  
[Ripristinare il backup](#ripristinare)

<a name="duplicator"></a>
## Installazione del Plugin
1. Cliccare nella colonna di sinistra di WordPress su `Plugins` e dopo `Aggiungi nuovo`.
2. Cercare `Duplicator` e attendere che la ricerca sia conclusa.
3. Premere su `Installa ora` dopodiché `attiva`.

<a name="procedura"></a>
## Creazione di un duplicato
1. Cliccare nella colonna di sinistra di WordPress su `Duplicator` e in alto a destra premere su `Crea Nuovo`.
2. Vi si aprirà una procedura guidata con degli steps.
      * Il primo step può essere saltato, premete quindi su `successivo`
      * Duplicator effettuerà una scansione del sito. Dopodiché vi darà un resoconto. Se tutto va bene vedrete tutte le etichette in verde con la scritta `GOOD`. Può essere che ci sia qualche etichetta gialla con la scritta `WARN`, anche in questo caso potrete procedere. In caso di etichetta rossa con la scritta `FAIL` dovrete cercare su Google il problema.
      * Se è tutto verde premete pure su `CREA`. Effettuerà la compressione del sito. 
3. Se tutto è andato correttamente vedrete la digitura **Pacchetto completato** in verde.
4. Scaricate (cliccando sopra) sia l'**installer** sia il pacchetto chiamato **Archivio**.

<a name="ripristinare"></a>
## Ripristinare il duplicato
1. Posizioniamoci nella cartella del nostro sito (se abbiamo il sito installato in locale la cartella sarà `htdocs` [clicca qui per sapere dove trovarla](#htdocs).
2. <a name="back-to-chapter-4"></a>Cancellate il file `wp-config.php`, se presente.
3. Copiare e incollare i due file scaricati nel capitolo 2 (**archivio del sito in formato zip** e il file `installer.php`) nella cartella del nostro sito. 
4. *Opzionale* se il file `installer` ha come suffisso un numero aggiunto dal sistema operativo (esempio: `installer (1).php`) rinominatelo rimuovendo il suffisso (lasciando quindi `installer.php`).
5. Recatevi, con il vostro browser preferito, sulla pagina `localhost/nome_della_cartella_del_sito/installer.php`. Se la pagina carica correttamente vuol dire che avete fatto tutto bene, in caso contrario controllate i passi precedenti.

## Processo di ripristino del duplicato

1. Mettete la spunta su "I have read and ...." e premete su **NEXT**
2. Inserite `Database` (nome del database) `User` (utente del database) `Password` (password dell'utente del database) `host` lasciate localhost. Dopo averlo fatto cliccate su **Test database**. Pregate il Padre Eterno e, se vi avrà ascoltato, verranno due etichette verdi con scritto `GOOD`. Se entrambe le etichette sono verdi con scritto `GOOD` premete su **NEXT**.
3. Se tutto è andato correttamente vi apparirà una schermata dove potrete decidere il nuovo title del sito. Dopo che sarete pronti premete **NEXT**.
4. Se tutto va bene premete su **ADMIN LOGIN** in alto a sinistra e inserite i dati di accesso di WordPress.  

<a name="htdocs"></a>
### Come trovare la cartella HTDOCS
La cartella HTDOCS si trova all'interno del software per la gestione del web server e del database. In caso abbiate Windows probabilmente sarà **XAMPP** in caso fosse Mac probabilmente sarà **MAMP**.
1. **WINDOWS** avviate XAMPP e cliccate su `Explorer` nella colonna a destra. Questo vi porterà nella cartella principale di XAMPP, da qui potrete trovare facilmente la cartella HTDOCS.
2. **MAC** aprite `Spotlight` cliccando `CMD + SPACE` oppure cliccando sulla lente di ingrandimento in alto a destra. Dopodiché nel campo di ricerca che apparirà scrivete HTDOCS.
[Torna su a come Ripristinare il duplicato](#back-to-chapter-4)
