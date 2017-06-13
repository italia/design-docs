Accessibilità
-------------

.. admonition:: SI DEVE

   Le pubbliche amministrazioni devono rispettare i requisiti
   tecnici di accessibilità riportati nell'`Allegato A del Decreto
   Ministeriale 8 luglio 2005 <http://www.agid.gov.it/dm-8-luglio-2005-allegato-A>`__
   e successive modifiche.

Definizione
~~~~~~~~~~~

Lo sviluppo di soluzioni ICT, hardware, software, web-based per la PA ha
come requisito fondamentale l'accessibilità.

La normativa sancisce che tutte le persone devono poter usare
applicazioni software, siti Web, servizi on line, app, documenti
elettronici, indipendentemente da eventuali limitazioni, ad esempio
limitazioni fisiche, tecnologiche o ambientali.

Nessun utente deve essere discriminato, anche se si trova ad operare in
una situazione di particolare difficoltà fisica, e deve quindi poter
fruire di tutte le informazioni e i servizi digitali rilasciati da un
ente pubblico.

Creare un sito accessibile
~~~~~~~~~~~~~~~~~~~~~~~~~~

L’accessibilità è una qualità che riguarda più aspetti di un sito web e
di un software in generale, e va considerata in diversi momenti dello
sviluppo, da diverse figure professionali:

-  Aspetto e contenuto (`visual e content <https://www.w3.org/WAI/WCAG20/quickref/?currentsidebar=%23col_customize&levels=aaa&techniques=advisory>`__)
-  Struttura (`develop <https://www.w3.org/WAI/WCAG20/quickref/?currentsidebar=%23col_customize&levels=aaa&techniques=advisory>`__)
-  Comportamento (`interaction <https://www.w3.org/WAI/WCAG20/quickref/?currentsidebar=%23col_customize&levels=aaa&techniques=advisory>`__)

Il `Decreto Ministeriale del 20 marzo 2013 <http://www.agid.gov.it/dm-8-luglio-2005-allegato-A>`__
individua i 12 requisiti da rispettare che derivano da `principi internazionali
<https://www.w3.org/TR/WCAG20/>`__. Per essere a norma,
il sito web di una PA deve soddisfare tutti i `controlli WCAG 2.0 fino al
livello AA <https://www.w3.org/WAI/WCAG20/quickref/?currentsidebar=%23col_customize&levels=aaa>`__.
In questa pagina forniamo un elenco degli errori più comuni
che limitano o impediscono l’accesso alle informazioni in un determinato
contesto.

Aspetto
^^^^^^^

-  **Contrasto tra primo piano e sfondo**: il testo e il relativo sfondo
   (compreso il testo contenuto nelle immagini), devono rispettare un
   preciso rapporto di contrasto, basato su un algoritmo. I logotipi, il testo di grandi dimensioni (`18 punti
   o 14 grassetto <https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast.html#larger-scaledef>`__)
   e il testo volutamente reso poco visibile (es. azioni
   inattive) non rientrano in questo controllo.
-  **Forma e colore**: le informazioni che veicola una pagina non devono
   dipendere unicamente da aspetto, forma, colore, dimensione,
   ubicazione visiva, orientamento o suono. Di seguito esempi di alcuni
   tra i più comuni errori:
   
   -  `Identificare il contenuto solo dalla forma o dal colore
      <https://www.w3.org/TR/WCAG20-TECHS/F14.html>`__
   -  `Usare unicamente simboli grafici per veicolare informazioni
      <https://www.w3.org/TR/WCAG20-TECHS/F26.html>`__
   -  `Creare link che sono solamente di un colore diverso dal testo
      <https://www.w3.org/TR/WCAG20-TECHS/F73.html>`__
   -  Nei moduli online, la `segnalazione dei campi obbligatori mancanti
      <https://www.w3.org/TR/WCAG20-TECHS/F81.html>`__
      effettuata solo tramite il colore

-  **Tempo sufficiente**: deve essere possibile `rimuovere il limite di tempo
   di visualizzazione <https://www.w3.org/TR/WCAG20-TECHS/F16.html>`__ di un oggetto nella pagina, o regolarne la
   scadenza, o estenderla facilmente prima del termine. Ad esempio 
   attenzione a pubblicare un contenuto che “scorre” come un carousel di
   notizie.
-  **Oggetti lampeggianti**: le pagine Web non devono contenere nulla che
   lampeggi per più di tre volte al secondo.
-  **Contenuti audio**: se un contenuto audio all'interno di una pagina Web
   è eseguito automaticamente per più di tre secondi, allora deve essere
   fornita una funzionalità per metterlo in pausa o interromperlo.

Struttura
^^^^^^^^^

-  **Link e controlli**: il codice del contenuto Web (es: HTML) va usato
   secondo le specifiche (es. un titolo è un Hn) e vanno esplicitate le
   relazioni tra elementi (es. `i campi devono essere legati alle loro
   etichette <https://www.w3.org/TR/WCAG20-TECHS/H44.html>`__).
-  **Alternative a oggetti non testuali**: tutti gli elementi non testuali,
   come immagini, grafici, infografiche, video e audio, devono avere
   un’alternativa testuale equivalente quando veicolano un significato,
   un’informazione o una funzione, come ad esempio il testo presente in
   un banner o in un bottone. Fare attenzione soprattutto ai controlli
   di verifica antispam (es. `CAPTCHA <https://www.w3.org/TR/WCAG20/#CAPTCHAdef>`__.)
-  **Ingrandimento**: il testo si deve poter ingrandire del 200% senza
   perdita di contenuto o funzionalità, e quindi senza sovrapposizioni
   di elementi che lo rendano incomprensibile.

Comportamento
^^^^^^^^^^^^^

-  **Link e controlli**: tutti i componenti dell’interfaccia si devono poter
   utilizzare tramite comandi da tastiera analogamente a quanto si
   riesce a fare col mouse. Risulta quindi errato:
   
   -  `Permettere l’interazione con link, campi di un form, menu, bottoni
      solo tramite l’uso del mouse
      <https://www.w3.org/TR/WCAG20-TECHS/F54.html>`__
   -  `Spostare il focus della tastiera dagli elementi nella pagina quando
      questi lo ricevono, o si aggiornano
      <https://www.w3.org/TR/WCAG20-TECHS/F55.html>`__

-  **Valore, ruolo e stato**: è meglio utilizzare i componenti standard
   dell’HTML e rendere maggiormente “visibili” gli elementi che ricevono
   il focus. Se si utilizzano componenti non standard, verificare che
   valore, ruolo e stato degli elementi siano sempre resi disponibili
   all’utente, in particolare alle tecnologie assistive (vedi 
   `WAI ARIA <https://www.w3.org/WAI/intro/aria>`__).

Un esempio per capire: uso del colore
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Il colore non può essere usato come unico mezzo per veicolare
un’informazione. Quindi, ad esempio, è sbagliato indicare “in
rosso le informazioni obbligatorie, in verde quelle accessorie”, perché
non tutti potrebbero essere in grado di percepire la differenza di
colore in contesti di fruizione diversi ma molto frequenti, ad es.:

-  da smartphone o tablet, di giorno e all'aperto
-  una stampa in bianco e nero della pagina web
-  una pagina web videoproiettata
-  in caso di daltonismo (`5-8% popolazione maschile <https://it.wikipedia.org/wiki/Daltonismo#Diffusione>`__)

Per comunicare un’informazione quindi, oltre al colore, è necessario aggiungere
un elemento testuale o grafico, un simbolo o un bordo.

Normativa
~~~~~~~~~

La normativa completa e aggiornata sull’accessibilità è disponibile sul
sito dell’`Agenzia per l’Italia digitale
<http://www.agid.gov.it/agenda-digitale/pubblica-amministrazione/accessibilita/normativa>`__ .

Obiettivi accessibilità
~~~~~~~~~~~~~~~~~~~~~~~

Entro il 31 marzo di ogni anno le pubbliche amministrazioni devono
pubblicare nei propri siti web gli “Obiettivi di accessibilità per
l’anno corrente”. L’Agenzia per l’Italia digitale ha predisposto
un’`applicazione on line <https://accessibilita.agid.gov.it/>`__
per ricevere dalle amministrazioni gli Obiettivi
di accessibilità. Gli obiettivi vanno pubblicati sui siti delle PA nella
sezione “amministrazione trasparente/Altri contenuti/Accessibilità e
Catalogo di dati, metadati e banche dati”.
