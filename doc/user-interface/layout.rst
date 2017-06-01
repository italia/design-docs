Layout
------

.. admonition:: SI DOVREBBE
   
   Utilizzare un layout essenziale.

L'impaginazione dei contenuti tramite un layout lineare (una o due
colonne) favorisce la **rapida scansione delle informazioni** e ne
agevola la consultazione soprattutto su *touchscreen*, dove il pattern
di interazione più funzionale è lo scorrimento verticale della pagina.

Casi d’uso validi per l’utilizzo di **una colonna laterale** (
``<nav>``, ``<aside>``) sono tutti e solo quelli dove sussiste
un’immediata correlazione semantica con il contenuto principale:

-  menu contestuale della sezione del sito correntemente visualizzata
-  elenco di sezioni / contenuti / documenti correlati

.. admonition:: SI PUÒ

   Elenchi di contenuti omogenei (ad esempio: anteprime di notizie o eventi)
   possono essere presentati tramite **card** o liste posizionate in una
   `griglia responsive <#griglie>`_.

L'utilizzo di card favorisce la consultazione dei contenuti sugli
schermi più piccoli.

Più in generale, laddove i dati non hanno una struttura prevalentemente
tabulare, è consigliato l'utilizzo di card o liste al posto che di
tabelle (``table``) che risultano più difficili da rendere fruibili in
maniera efficace sui dispositivi mobili.

Gerarchia dei contenuti
~~~~~~~~~~~~~~~~~~~~~~~

.. admonition:: SI DEVE
   
   Per una corretta definizione della struttura gerarchica dei contenuti,
   la suddivisione in parti deve essere espressa attraverso l’uso dei tag
   semantici disponibili in HTML5, quali ``<article>, <aside>, <figcaption>,
   <header>, <footer>``, ecc., al posto del generico divisore ``<div>``.

Griglie
~~~~~~~

All’interno dello spazio a disposizione l’organizzazione del contenuto
deve essere strutturata seguendo un sistema di **griglie responsive**
per mantenere una efficace esperienza utente trasversalmente ai
dispositivi utilizzati.

La griglia rappresenta la struttura invisibile che permette di
organizzare i contenuti della pagina. Una griglia di impaginazione
consiste in **colonne** di testo (e/o immagini) separate da spazi
intercolonna e contornate dai margini della pagina.

Le dimensioni delle colonne vanno adattate ai cambiamenti della
viewport: ogni colonna occuperà una percentuale di spazio specifica a
seconda che sia visualizzata su dispositivi desktop, tablet, o
smartphone. La ridisposizione dei contenuti,a seconda delle dimensione
dello schermo, garantisce che i testi siano leggibili anche sugli
schermi più piccoli e l'interazione utente (es. form, controlli
dinamici) rimanga agevole.

Impostazioni della griglia di costruzione consigliata
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

-  Larghezza massima del contenitore: 1440 px
-  Spazio intercolonna (*gutter*): 16 px a tutte le risoluzioni.

+----------------------------------------+------------------+
| Breakpoint                             | Padding laterale |
+========================================+==================+
| Smartphone (< 768 px)                  | 16 px            |
+----------------------------------------+------------------+
| Tablet (< 992 px)                      | 16 px            |
+----------------------------------------+------------------+
| Desktop (< 1366 px)                    | 24 px            |
+----------------------------------------+------------------+
| Desktop (< 1366 px)                    | 24 px            |
+----------------------------------------+------------------+

Impostazione della home page
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. admonition:: SI DOVREBBE

   Il corpo della home page dovrebbe privilegiare una **struttura
   modulare orizzontale** con sezioni che comprendono contenuti omogenei.

Tale struttura

-  costituisce una guida visuale per l’utente messo in grado di
   riconoscere e distinguere agevolmente le diverse sezioni autonome e
   ben identificate
-  non presenta problematiche legate alla riorganizzazione gerarchica
   dei contenuti su mobile
-  favorisce la flessibilità poiché, all’occorrenza, i singoli blocchi
   possono essere nascosti o spostati senza impatti sull’armonia
   generale della pagina
-  costringe a un’analisi approfondita riguardo i contenuti da
   considerare prioritari, scoraggiando quindi l'affollamento di
   informazioni non essenziali

Le sezioni della home page
^^^^^^^^^^^^^^^^^^^^^^^^^^

-  **devono avere un titolo** che le identifica in modo chiaro (es.
   servizi, notizie, eventi, ...)
-  possono esser distinte tramite **colori di sfondo differenti**
   (appartenenti a una `palette coerente <#>`__) eventualmente alternati
-  qualora vi fossero ulteriori contenuti da mostrare, deve esser
   presente un **link** collegato alla pagina contenente l’elenco
   completo
