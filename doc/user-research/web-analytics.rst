Web analytics
-------------

Premessa
~~~~~~~~

Questa guida ha l’obiettivo di aiutare chi si occupa a vario titolo del
sito web di una pubblica amministrazione a:

-  comprendere il funzionamento di una piattaforma di web analytics
-  capire come collezionare i principali indicatori di performance di un
   sito
-  capire come interpretare determinati set di dati per trarre
   informazioni utili rispetto al comportamento degli utenti e il loro
   livello di soddisfazione
-  comprendere quali azioni migliorative applicare ai contenuti, ai
   metadati e alla struttura del sito in base ai risultati dell’analisi
   dei dati
-  comprendere come configurare una piattaforma di web analytics su uno
   o più siti
-  comprendere come produrre e distribuire un report di analytics, per
   condividere i dati di utilizzo con gli stakeholder e il team di
   lavoro interno
-  comprendere come una lettura sistematica dei dati possa influenzare
   positivamente la comprensione dei comportamenti online degli utenti e
   consentire l’avvio di azioni migliorative dei servizi digitali

Introduzione
~~~~~~~~~~~~

L’analisi delle performance di un ambiente web è un’attività cruciale
per comprendere in che maniera un sito (o un servizio digitale di altro
tipo) rispondono in maniera adeguata ai bisogni informativi e/o di
servizio degli utenti.

Questa tipologia di analisi consente di rispondere, ad esempio, in modo
puntuale alle seguenti domande:

-  Quanti utenti visitano il sito, per quanto tempo e quali e quante
   pagine visitano?
-  Quali sono le principali città da cui provengono i visitatori del
   sito? Quanti utenti che visitano il sito provengono dall’Italia e
   quanti eventualmente dall’ estero?
-  Quali sono i contenuti più visitati dagli utenti in un dato
   intervallo di tempo?
-  In quale momento della settimana o dell’anno il sito registra il
   maggiore o il minore numero di visite? Queste oscillazioni sono
   causate da un’eventuale stagionalità delle tematiche trattate o
   coincidono con la pubblicazione di nuovi contenuti?
-  Quali sono i termini tramite cui gli utenti arrivano al sito tramite
   un motore di ricerca? Rappresentano per la maggior parte il
   nome/dominio del sito oppure fanno riferimento a informazioni/servizi
   trattati al suo interno?
-  Quali sono i principali termini di ricerca digitati nel motore di
   ricerca interno del sito, se presente?
-  In che percentuale gli utenti che visitano il sito lo fruiscono da
   dispositivi mobili?

Le risposte a tali domande derivano dall’analisi continuativa di
indicatori di performance che offrono ad esempio informazioni su quali
siano volumi di traffico del sito, quale il comportamento degli utenti,
quale la qualità dei contenuti pubblicati o quale l’efficienza
tecnologica del sito nel suo complesso.

Metriche e Dimensioni
~~~~~~~~~~~~~~~~~~~~~

I dati generati dalle piattaforme di web analytics sono il frutto di
combinazioni eterogenee di metriche (dati quantitativi) e dimensioni
(attributi qualitativi dei dati). Si precisa che il numero reale dei visitatori conteggiati per un dato intervallo di tempo è soggetto a distorsioni — per eccesso o per difetto — dovute al fatto che il calcolo degli utenti in web analytics è basato su cookies e tende quindi a generare più o meno utenti unici al variare di determinate circostanze (accesso al sito da dispositivi diversi, browser diversi, cancellazione dei cookies). Di seguito una panoramica esplicativa
delle principali metriche e dimensioni utilizzate nella web analysis. Si
precisa che la nomenclatura di metriche e dimensioni può variare a
seconda della piattaforma di analytics utilizzata.

Principali Metriche (dati quantitativi)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Visite**
   *Definizione:* numero totale di visite al sito in un dato intervallo
   di tempo (anche da parte dello stesso utente)
   
   *A cosa serve:* rappresenta il volume di traffico che il sito riceve
   in un determinato lasso temporale. È una delle metriche più usate per
   costruire uno storico dei volumi di traffico del sito, su cui basare
   comparazioni e/o proiezioni

**Visite uniche**
   *Definizione:* numero di singoli individui (o singoli IP) che ha
   effettuato almeno una visita al sito
   
   *A cosa serve:* è la metrica che restituisce in maniera accurata il
   numero di singoli individui che ha interagito con il sito in un dato
   lasso di tempo

**Visualizzazioni di pagina**
   *Definizione:* numero totale di pagine visitate, anche da parte dello
   stesso utente, in un dato intervallo di tempo. Comprende
   visualizzazioni ripetute della stessa pagina
   
   *A cosa serve:* indica il volume complessivo dei contenuti del sito
   acceduti dagli utenti

**Pagine visitate per visita**
   *Definizione:* media aritmetica del numero di pagine visitate per
   visita al sito. Comprende le visualizzazioni ripetute della stessa
   pagina
   
   *A cosa serve:* offre indicazioni sulla “profondità” delle visite al
   sito e sul livello di coinvolgimento dei contenuti. Tale metrica deve
   essere interpretata a seconda della natura del sito e dei suoi
   obiettivi (es. rispetto al numero minimo di pagine desiderate per
   visita)

**Durata delle visite**
   *Definizione:* media aritmetica della durata di una singola visita al
   sito
   
   *A cosa serve:* indica il tempo medio trascorso dai visitatori sul
   sito. Tale metrica deve essere interpretata a seconda della natura
   del sito e dei suoi obiettivi

**Tempo sulla pagina**
   *Definizione:* media aritmetica del tempo trascorso dagli utenti su
   una determinata pagina (o un insieme di pagine)
   
   *A cosa serve:* determina l’efficacia di un contenuto, a seconda
   della sua tipologia e dei suoi obiettivi

**Frequenza di rimbalzo**
   *Definizione:* percentuale di visitatori che ha abbandonato il sito
   dopo una pagina
   
   *A cosa serve:* misura la quota di utenti che arrivano al sito e lo
   abbandonano subitaneamente. La percentuale di frequenza di rimbalzo
   può essere interpretata in maniera opposta a seconda della natura del
   sito: ad esempio una frequenza di rimbalzo alta per un sito
   informativo è indice del fatto che le pagine potrebbero essere
   scarsamente utili/interessanti, mentre può essere considerata un dato
   positivo per un sito o una pagina che hanno il semplice scopo di
   direzionare gli utenti altrove

**Nuove visite**
   *Definizione:* percentuale delle prime visite al sito sul totale
   delle visite
   
   *A cosa serve:* metrica utile in particolare quando l’obiettivo del
   sito è quello di accrescere i volumi di traffico provenienti da nuove
   tipologie di visitatori

**Nuovi utenti/utenti di ritorno**
   *Definizione:* rapporto fra prime visite al sito e utenti che hanno
   già visitato il sito precedentemente, in un dato intervallo di tempo
   
   *A cosa serve:* a seconda degli obiettivi del sito, serve a
   comprendere in che misura i volumi di traffico si suddividono fra
   nuovi utenti e utenti fidelizzati

**Velocità di caricamento del sito**
   *Definizione:* quantità di tempo media (espressa in secondi)
   impiegato da una pagina del sito per caricarsi, dall’avvio della
   visualizzazione nel browser alla fine del suo caricamento
   
   *A cosa serve:* metrica fondamentale per monitorare l’efficienza del
   sito in termini di velocità, anche e soprattutto per la fruizione da
   dispositivi mobili

Principali Dimensioni (attributi qualitativi dei dati)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Tempo**
   intervallo di tempo su cui impostare una rilevazione (giorno,
   settimana, mese, anno, intervallo personalizzato)

**Provenienza geografica e lingua**
   luogo da cui provengono le visite
   degli utenti (paese, città, continente, subcontinente); impostazioni
   relative alle preferenze di lingua

**Tecnologia utilizzata**
   strumenti tecnologici utilizzati dagli utenti
   per la navigazione sul sito (tipologia di dispositivo, browser, sistema
   operativo, provider di rete)

**Contenuti**
   le pagine, le pagine di entrata e di uscita, gli “eventi”
   compiuti sul sito (es. download di documenti, click su link outbound)

**Canali di acquisizione del traffico**
   canali web tramite cui gli
   utenti arrivano al sito. Il raggruppamento di canali principali
   comprende: traffico diretto, ricerca organica (cioè traffico non a
   pagamento proveniente dai motori di ricerca), siti referenti, social.
   Altri canali - se attivi - sono ad esempio: email marketing, digital
   advertising, affiliazioni

**Ricerca su sito**
   monitora la funzione di search del motore interno
   di un sito web, restituendo i termini di ricerca immessi dagli utenti,
   il numero di ricerche per termine e altri indicatori

**Obiettivi**
   per tracciare il completamento di determinate azioni
   eseguite degli utenti sul sito (es. compilazione di un form, durata
   minima di una visita, numero minimo di pagine per visita)

Analizzare le ricerche degli utenti
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Le ricerche degli utenti sono quasi sempre il più ampio vettore di
traffico verso i contenuti web. Per questa ragione, non soltanto è
fondamentale fare in modo che le pagine di un sito siano `“ottimizzate”
per essere trovate dagli utenti attraverso i motori di
ricerca <../content-design/seo.html>`__, ma è altrettanto importante
analizzare i dati di web analytics provenienti dalle ricerche interne ed
esterne al sito per avere contezza delle performance dei singoli
contenuti e del livello di soddisfazione-utente che generano.

Ecco i principali indicatori da tenere in considerazione quando si
analizzano le ricerche degli utenti e le relative azioni migliorative
che si possono intraprendere:

Ricerca esterna al sito
^^^^^^^^^^^^^^^^^^^^^^^

**Top motori di ricerca referenti**
   *Definizione:* Principali motori di ricerca (Google, Bing, Yahoo…)
   che portano traffico al sito
   
   *Azione:* Usa i relativi webmaster tools (es. `Google Search
   Console <../content-design/seo.html>`__) per ottimizzare i contenuti
   e la struttura del sito e renderli così più facilmente scansionabili
   dai crawler dei motori e “trovabili” dagli utenti

**Top termini/frasi di ricerca**
   *Definizione:* Le principali parole e frasi digitate nei motori di
   ricerca tramite cui gli utenti arrivano al sito
   
   *Azione:* Verifica che i termini utilizzati dagli utenti coincidano o
   siano simili a quelli utilizzati nel sito. Puoi prendere spunto da
   parole e frasi utilizzate dagli utenti per migliorare la terminologia
   che usi nei titoli, nei metadati, nelle URL e in generale all’interno
   dei contenuti, in modo da favorirne l’ottimizzazione sui motori di
   ricerca

**Top termini di ricerca con basso CTR (click through rate)**
   *Definizione:* Parole e frasi digitate nei motori di ricerca che
   portano la minore quota di traffico al sito
   
   *Azione:* Revisiona e aggiorna i contenuti che gli utenti visitano
   dopo aver cercato tali termini, per renderli più appetibili e utili

Ricerca su sito
^^^^^^^^^^^^^^^

**Top termini/frasi di ricerca**
   *Definizione:* Le principali parole e frasi digitate dagli utenti nel
   motore di ricerca interno del sito
   
   *Azione:* Crea nuovi contenuti o aggiorna quelli già presenti,
   incorporando la terminologia degli utenti nei metadati, negli
   eventuali tag e nel testo stesso, in modo da aiutare i visitatori a
   trovare le informazioni più aderenti ai bisogni espressi nella
   ricerca

**Top ricerche che non generano risultati**
   *Definizione:* Parole e frasi digitate dagli utenti nel motore
   interno del sito che non restituiscono risultati, per mancanza di
   contenuti associati o non rappresentati nella maniera corretta
   
   *Azione:* Analizza i contenuti per capire se è il caso di aggiornarli
   o di pubblicarne di nuovi che rappresentino il bisogno espresso
   dall’utente nella ricerca

**Top termini di ricerca con basso CTR (click through rate)**
   *Definizione:* Parole e frasi digitate nel motore di ricerca interno
   che restituiscono il più basso numero di visualizzazioni di pagina
   
   *Azione:* Incorpora la terminologia valida nei testi e nei metadati
   per rendere le pagine più rilevanti rispetto a quei termini

**Principali oscillazioni nelle top ricerche**
   *Definizione:* Macro cambiamenti nel ranking dei termini più cercati
   nel motore di ricerca interno del sito
   
   *Azione:* Cerca di analizzare le ragioni per cui alcuni termini
   diventano meno ricercati di altri e viceversa; assicurati che per i
   nuovi termini di ricerca diventati popolari siano presenti contenuti
   che soddisfano i nuovi bisogni espressi dai visitatori

**Utenti che utilizzano la ricerca su sito**
   *Definizione:* Percentuale dei visitatori unici del sito che utilizza
   la funzione di ricerca interna
   
   *Azione:* Ti aiuta a capire se è il caso di ottimizzare le
   funzionalità di ricerca e l’architettura informativa del sito,
   facendo in modo che i contenuti più ricercati siano il più possibile
   visibili
   
La segmentazione
~~~~~~~~~~~~~~~~
La segmentazione in web analytics consiste nell'isolare dal traffico web aggregato sottoinsiemi di visite (o di utenti unici) che condividono attributi (qualitativi e/o quantitativi) comuni. La segmentazione del traffico in sottogruppi, ha l’obiettivo di far emergere il “valore” di uno specifico insieme di utenti rispetto al traffico aggregato - che è tipicamente quello più rappresentato nei report, ma meno rappresentativo delle specificità dei singoli gruppi di utenza. 

Nelle principali piattaforme di web analytics la segmentazione può essere applicata utilizzando segmenti preimpostati (laddove disponibili) oppure creando dei segmenti di utenza ad hoc. Si possono creare segmenti sulla base di attributi demografici dei visitatori, delle tecnologie utilizzate per navigare il sito, del comportamento, della data di prima visita dell’utente, delle sorgenti di traffico, e così via. 

Il traffico "segmentato" può essere poi quindi comparato nei rapporti e nelle configurazioni dashboard. 

Per maggiori dettagli sulla segmentazione utenti si rimanda al `Kit Web Analytics <https://designers.italia.it/kit/analytics/>`__.


Cosa fare per adempiere alla normativa sui cookie
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------------------------------------------------------------------------+-----------------------------+---------------------------------------------------------+------------------------------------------------------------+
| Tipo di cookie                                                                           | Segnalarli nell'informativa | Inserire il banner e chiedere il consenso ai visitatori | Notificare al Garante                                      |
+==========================================================================================+=============================+=========================================================+============================================================+
| Nessun cookie                                                                            | No                          | No                                                      | No                                                         |
+------------------------------------------------------------------------------------------+-----------------------------+---------------------------------------------------------+------------------------------------------------------------+
| Tecnici/analitici di prima parte                                                         | Si                          | No                                                      | No                                                         |
+------------------------------------------------------------------------------------------+-----------------------------+---------------------------------------------------------+------------------------------------------------------------+
| Analitici terze parti (con strumenti che riducono il potere identificativo dei cookie)   | Si                          | No                                                      | No                                                         |
+------------------------------------------------------------------------------------------+-----------------------------+---------------------------------------------------------+------------------------------------------------------------+
| Analitici terze parti (senza strumenti che riducono il potere identificativo dei cookie) | Si                          | Si                                                      | Si                                                         |
+------------------------------------------------------------------------------------------+-----------------------------+---------------------------------------------------------+------------------------------------------------------------+
| Di profilazione prima parte                                                              | Si                          | Si                                                      | Si                                                         |
+------------------------------------------------------------------------------------------+-----------------------------+---------------------------------------------------------+------------------------------------------------------------+
| Di profilazione terze parti                                                              | Si                          | Si                                                      | No* (la notificazione è a carico del soggetto terza parte) |
+------------------------------------------------------------------------------------------+-----------------------------+---------------------------------------------------------+------------------------------------------------------------+

Per approfondimenti si rimanda al sito del `Garante della Privacy <http://www.garanteprivacy.it/cookie>`__.

La reportistica
~~~~~~~~~~~~~~~

Un’analisi sistematica dei dati statistici di performance e
soddisfazione utente è fondamentale per decidere quali azioni
migliorative intraprendere su un servizio digitale.

È altrettanto fondamentale la creazione di una reportistica ad hoc che
abbia la finalità di essere condivisa all’interno di un team di lavoro
(o con altri stakeholder). In linea generale è possibile creare e
inviare report customizzati direttamente dalle principali piattaforme di
web analytics.

Per un approfondimento sul tema, si rimanda al `Kit Web Analytics <https://designers.italia.it/kit/analytics/>`__.

Gli strumenti (Matomo/Piwik e Google Analytics)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Di seguito proponiamo una serie di link di approfondimento per
comprendere come installare/configurare nella maniera corretta due fra
le principali piattaforme di web analytics gratuite, **Matomo/Piwik**
(piattaforma open source) e **Google Analytics** (piattaforma
commerciale).

Matomo/Piwik
^^^^^^^^^^^^

-  `Installazione e configurazione di Matomo/Piwik
   <https://piwik.org/docs/installation/>`__
-  `Aggiungere un sito a Matomo/Piwik
   <https://piwik.org/docs/manage-websites/>`__
-  `Implementare il tracciamento del motore di ricerca interno al sito
   <https://piwik.org/docs/site-search/>`__
-  `Impostare un obiettivo
   <https://piwik.org/docs/tracking-goals-web-analytics/>`__
-  `La segmentazione
   <https://matomo.org/docs/segmentation/>`__
-  `Creazione ed invio di report customizzati
   <https://piwik.org/docs/email-reports/>`__
-  `Importare dati da GA a Matomo/Piwik
   <https://piwik.org/blog/2012/08/google-analytics-to-piwik/>`__

Google Analytics
^^^^^^^^^^^^^^^^

-  `Configurazione di Google Analytics
   <https://support.google.com/analytics/answer/1102154>`__
-  `Implementare il codice di tracciamento
   <https://support.google.com/analytics/topic/1726910?hl=it&ref_topic=3544906>`__
-  `Implementazione del codice per app
   <https://support.google.com/analytics/topic/2587085?hl=it&ref_topic=3544906>`__
-  `Implementare il tracciamento del motore di ricerca interno al sito
   <https://support.google.com/analytics/answer/1012264?hl=it>`__
-  `Collegare la Search Console a Google Analytics
   <https://support.google.com/analytics/answer/1308621?hl=it>`__
-  `Impostare un obiettivo
   <https://support.google.com/analytics/answer/1012040?hl=it&ref_topic=6150889>`__
-  `La segmentazione
   <https://support.google.com/analytics/answer/3123951>`__
-  `Export ed invio via email dei dati
   <https://support.google.com/analytics/answer/1038573?hl=it>`__
