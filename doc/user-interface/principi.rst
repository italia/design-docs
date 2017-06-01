Principi
--------

Mobile first
~~~~~~~~~~~~

L'approccio *mobile first* consiste nel **valutare in prima istanza la
resa sui dispositivi mobili**, per poi arricchire di elementi e
funzionalità la composizione della pagina mano a mano che la viewport
aumenta.

Responsive Web Design
^^^^^^^^^^^^^^^^^^^^^

.. admonition:: SI DEVE

   Il sito web deve essere progettato e sviluppato con un approccio *responsive*
   con l'obiettivo di rendere disponibile un'ottimale esperienza di visione all'utente,
   facilità di lettura e navigazione con minime necessità di ridimensionare, spostare o
   scorrere, su qualunque dispositivo indipendentemente dalla risoluzione e dalla
   dimensione dello schermo.

Nell'approccio mobile first si parte dall'essenziale.

Obbligarsi a progettare un'applicazione con ridotte disponibilità di
spazio, di interazione, di velocità di caricamento costringe a stabilire
delle priorità e a fare delle scelte che risulteranno utili
all'usabilità del prodotto.

Man mano che lo schermo si fa più grande e il collegamento più veloce, i
contenuti vengono arricchiti. Un utente seduto alla scrivania con un
computer ha probabilmente più tempo e più possibilità di approfondire e
navigare. Un utente collegato da smartphone ha forse l'urgenza di
cercare quel contenuto dal luogo in cui si trova, senza aspettare di
tornare a casa e arrivando all'essenziale il più velocemente possibile.

I contenuti e le funzionalità di un sito o un servizio devono poter
essere fruibili su tutti i dispositivi più utilizzati dagli utenti.

.. admonition:: SI DOVREBBE

   Analizzare regolarmente l'utilizzo dei dispositivi e delle diverse risoluzioni
   che gli utenti adoperano per accedere al sito.

È necessario assicurare la compatibilità con almeno i seguenti browser:

-  Internet Explorer 10+
-  Edge 12+
-  Safari 8+
-  Google Chrome (ultime versioni)
-  Opera (ultime versioni)
-  Mozilla Firefox (ultime versioni)
-  IE Mobile 10+
-  iOS Safari 8+ (versione del sistema operativo)
-  Android Browser 4+ (versione del sistema operativo)

La lista comprende più del 95% delle versioni utilizzate in Italia (e
nel mondo) secondo i dati raccolti da
`StatCounter <http://gs.statcounter.com/#browser-IT-monthly-201506-201606>`__

Non è necessario che l'aspetto del sito sia identico sui diversi
dispositivi; va tuttavia garantita un'esperienza utente equivalente.

Garantire la compatibilità
~~~~~~~~~~~~~~~~~~~~~~~~~~

Nel web design si sono adottati spesso gli approcci **graceful
degradation** (decadimento parziale) o **progressive enhancement**
(miglioramento progressivo). Si tratta di due risposte diverse alla
stessa esigenza: rendere il contenuto accessibile su dispositivi
diversi. Nel primo approccio ci si fa carico di verificare che il
progetto, inizialmente pensato per i dispositivi più completi, resti
navigabile anche man mano che si usano tecnologie più obsolete o meno
interattive. Nel secondo, si parte da un nucleo solido e irrinunciabile
di contenuti che vengono arricchiti via via che il dispositivo diventa
più potente e all'avanguardia.

Tecnicamente il sito web può rilevare quale dispositivo lo sta
navigando. È possibile capire: - lo **user agent**, ovvero quale browser
e quale sistema operativo è in collegamento - la **risoluzione** dello
schermo, ovvero quanti pixel abbiamo a disposizione - il **tipo di
media**, ovvero se stiamo andando in stampa o su schermo

Tecniche apposite come l'uso di **media queries** permettono di inserire
istruzioni nei CSS affinché la presentazione dei contenuti sia calibrata
sull'attuale dimensione della viewport.

Validazione dei fogli di stile CSS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Per compensare le incompatibilità dei diversi browser è spesso
necessario introdurre nei fogli di stile (CSS) codice non conforme; di
conseguenza i risutati del `test di validazione del
W3C <https://jigsaw.w3.org/css-validator/>`__ riportano degli errori.

La validazione è importante laddove tali errori pregiudicano una
funzionalità; oggi i browser sono più "resilienti" e spesso non si
verifica il caso.

Non è necessario pertanto che un CSS rientri perfettamente negli
standard.

La validazione del CSS non è inoltre sufficiente a garantire
l'`accessibilità <../service-design/accessibilita.html>`__.
