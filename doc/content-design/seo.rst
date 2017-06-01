SEO
---

Premessa
~~~~~~~~

Questa guida ha lo scopo di aiutare chi si occupa del sito web di una
pubblica amministrazione a capire come ottimizzare i contenuti
pubblicati e la struttura del sito nel suo complesso in ottica SEO, con
l’obiettivo finale di rendere informazioni e servizi più idonei a
soddisfare i bisogni degli utenti e più visibili sui motori di ricerca.

Introduzione
~~~~~~~~~~~~

Con il termine search engine optimization (SEO) - o ottimizzazione per i
motori di ricerca - si intende un insieme di tecniche iterative
applicabili al contenuto delle pagine web e alla struttura dei siti che
hanno lo scopo di migliorare il posizionamento di un contenuto web nel
ranking dei risultati dei motori di ricerca.

I fattori di ottimizzazione vengono generalmente suddivisi in 2
categorie:

-  fattori on-page, cioè eseguibili all’interno del sito
-  fattori off-page, cioè eseguibili al di fuori del sito

I fattori on-page
~~~~~~~~~~~~~~~~~

Titolo del contenuto
^^^^^^^^^^^^^^^^^^^^

Un titolo dovrebbe descrivere in modo semplice quanto esposto nella
pagina, utilizzando di preferenza la terminologia più simile a quella
che userebbero gli stessi utenti per descriverne il contenuto.

È consigliabile creare titoli univoci, il più possibile pertinenti
rispetto al contenuto della pagina:
un titolo dovrebbe essere composto da poche parole o una frase,
evitando di superare i 60/70 caratteri (spazi inclusi).

**Markup**: Il metatag title deve essere posizionato all’interno del tag
head nel codice HTML della pagina. Appare come prima linea testuale del
risultato dei motori di ricerca:

-  aiuta gli utenti a comprendere con immediatezza se il risultato in
   questione sia pertinente al bisogno espresso durante la ricerca web;
-  e’ uno fra i principali elementi che i crawler dei motori analizzano
   per indicizzare un contenuto e assegnargli un rank nei risultati di
   ricerca.

Description del contenuto
^^^^^^^^^^^^^^^^^^^^^^^^^

È consigliabile la redazione di description univoche per ogni
contenuto, che sintetizzino gli elementi salienti della pagina.

**Markup**: Il metatag **description** deve essere posizionato
all’interno del tag **head** nel codice HTML della pagina. Appare come
terza linea testuale (dopo la URL della pagina) del risultato dei motori
di ricerca:

-  come il titolo aiuta gli utenti a comprendere con immediatezza se il
   risultato in questione sia pertinente al bisogno espresso durante la
   ricerca;
-  la description può essere di qualsiasi lunghezza, ma generalmente i
   motori di ricerca troncano testi più lunghi di 160 caratteri (spazi
   inclusi).
   
Le parole chiave
^^^^^^^^^^^^^^^^

La scelta delle parole chiave più
strategiche e salienti rispetto ai contenuti di un sito è uno fra i
fattori che concorrono al buon posizionamento di un sito web fra i
risultati dei motori di ricerca.

Il lavoro di identificazione delle keyword più idonee a rappresentare i
contenuti di un servizio digitale è un lavoro iterativo che deve tenere
conto di:

-  quali sono le parole che meglio potrebbero descrivere le informazioni
   presenti nel sito
-  quali sono i loro volumi di ricerca
-  in che maniera i concetti espressi nel sito potrebbero potenzialmente
   essere cercati dagli utenti sui motori di ricerca

Di seguito alcuni metodi per iniziare ad identificare un set di keywords
salienti:

.. figure:: images/SEO-google-suggest.png
   :alt: google suggest
   
   Google suggest

.. figure:: images/SEO-google-ricerche-correlate.png
   :alt: google suggest

   Google ricerche correlate

-  `Google Trends <https://trends.google.it/trends/>`__

-  `Ubersuggest <https://ubersuggest.io/>`__

-  `Adwords
   keywordplanner <https://adwords.google.com/home/tools/keyword-planner/>`__

Originalità del contenuto
^^^^^^^^^^^^^^^^^^^^^^^^^

È sempre consigliabile redigere contenuti originali, possibilmente
centrati sui bisogni dell’utente, con un linguaggio il più possibile
chiaro.

Aggiornamento del contenuto
^^^^^^^^^^^^^^^^^^^^^^^^^^^

È necessario procedere regolarmente ad un aggiornamento dei contenuti pubblicati per evitare di
fornire agli utenti informazioni obsolete. Gli algoritmi dei motori di
ricerca considerano inoltre la data di aggiornamento di un contenuto web
come fattore di rilevanza nel ranking dei risultati di ricerca.

Paragrafazione e paginazione
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Per una maggiore leggibilità dei testi è
`consigliabile paragrafare <../user-interface/stile.html#formattazioni-consigliate>`__
i contenuti di una pagina, soprattutto se di
lunghezza importante. È utile inoltre titolare gli eventuali
sottoparagrafi secondo i medesimi principi applicabili al titolo
principale della pagina.

Nel caso ci sia la necessità di suddividere il contenuto in più pagine,
è consigliabile:

-  specificare quale sia la pagina principale di visualizzazione
   (visualizza tutto) attraverso l’attributo
   `rel="canonical" <#duplicazione-dei-contenuti>`__
-  utilizzare gli attributi HTML rel="next" e rel="prev", per
   specificare la relazione di consequenzialità fra URL

`Ulteriori informazioni sulla paginazione
<https://support.google.com/webmasters/answer/1663744?hl=it&ref_topic=4617741>`__

Grassetto
^^^^^^^^^

Può essere utile impiegare lo stile grassetto per evidenziare - senza
esagerare - i termini salienti di un contenuto.

Immagini
^^^^^^^^

È necessario nominare i file immagine in maniera pertinente al contenuto
della pagina ove sono collocati.

**Markup**: Utilizzare il **tag** alt per fornire una descrizione
testuale dell’immagine. Questo attributo è utile nel caso in cui questa
non possa essere visualizzata nel browser per motivi legati ad esempio
al mancato supporto di alcune tipologie di file da parte del browser o
all’\ `utilizzo di tecnologie
assistive <../service-design/accessibilita.html>`__.

È possibile generare ed utilizzare una `sitemap XML ad hoc per le
immagini <#mappa-del-sito>`__ per fornire ai crawler maggiori
informazioni rispetto all’organizzazione dei file immagini presenti nel
sito.

Anchor Text dei link
^^^^^^^^^^^^^^^^^^^^

Per “anchor text” si intende la porzione
di testo di un contenuto che funge da “ancora” verso un collegamento
ipertestuale, sia esso rivolto all’interno (link interno) o all’esterno
del sito (link outbound).

È consigliabile scegliere porzioni di testo brevi, chiare e pertinenti
rispetto alla pagina di destinazione del link:

-  il testo cliccabile - così come lo stile grassetto - fornisce tanto
   agli utenti quanto ai crawler dei motori di ricerca informazioni
   aggiuntive rispetto al contenuto della pagina linkata;
-  è bene evitare di linkare espressioni povere di significato come
   “clicca qui” e simili.

Struttura logica dei contenuti
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Una struttura dei contenuti semplice e “leggera” è necessaria per
garantire una migliore esperienza utente sul sito e per agevolare il
lavoro di scansione dei crawler dei motori di ricerca.

È consigliabile mantenere la struttura dei contenuti del sito
gerarchica - dal generale al particolare - semplificandone il più
possibile la struttura logica e utilizzando non più di tre livelli di
profondità.

URL delle pagine
^^^^^^^^^^^^^^^^

La URL di una pagina web appare come
seconda linea testuale del risultato di ricerca (fra title e
description). È buona regola semplificarne il più possibile la
struttura:

-  impostare le URL in modo che contengano parole salienti e pertinenti
   rispetto ai contenuti della pagina che ospitano
-  utilizzare i trattini (-) invece che gli underscore (\_) per la
   punteggiatura
-  cercare di ridurre il più possibile la lunghezza delle URL
-  valutare l’utilizzo del `file robots.txt <#file-robots-txt>`__ per
   bloccare la scansione da parte dei crawler dei motori di ricerca
   delle URL con parametri dinamici (referral, ordinamenti, calendari…)

`Ulteriori informazioni sulla struttura delle URL
<https://support.google.com/webmasters/answer/76329?hl=it&ref_topic=4617741>`__

Duplicazione dei contenuti
^^^^^^^^^^^^^^^^^^^^^^^^^^

È importante evitare la presenza di contenuti duplicati nel sito. Dal
punto di vista SEO si intendono “contenuti duplicati” contenuti molto
simili - o identici - nell’ambito dello stesso sito ma associati a URL
differenti.

In alcuni casi la duplicazione di un contenuto è generata da situazioni
particolari quali ad esempio:

-  la presenza di una pagina in versione web e versione per la stampa
-  la presenza di una tabella dinamica che genera viste dello stesso
   contenuto ma URL dinamiche diverse

In questi e altri casi è possibile inviare a Google l’informazione di
quale sia la pagina “master”, o “canonica” da prendere in considerazione
per l’indicizzazione. Questa tecnica è detta canonicalizzazione: per
implementarla è necessario inserire un elemento link che contenga
l’attributo rel=”canonical” (seguito dal link cui si vuole applicare la
canonicalizzazione), nel tag **head** della pagina.

`Approfondimenti sui contenuti duplicati
<https://support.google.com/webmasters/answer/66359?hl=it>`__

`Approfondimenti sulla canonicalizzazione
<https://support.google.com/webmasters/answer/139066>`__

Mappa del sito
^^^^^^^^^^^^^^

Oltre ad una mappa del sito in HTML destinata agli
utenti, è consigliabile creare un file sitemap XML destinato ai motori
di ricerca.

`Informazioni sulle sitemap
<https://support.google.com/webmasters/answer/156184?hl=it&ref_topic=4581190>`__

Una sitemap è un file che ha lo scopo di elencare le pagine web di un
sito per comunicare a Google e altri motori di ricerca l'organizzazione
dei contenuti. I crawler dei motori leggono questo file per eseguire una
scansione più efficiente del sito. Una sitemap ha quindi l’obiettivo
ultimo di migliorare la scansione di un sito da parte dei motori di
ricerca.

All’interno di un file sitemap è possibile non soltanto elencare le URL
di un sito web ma anche alcuni metadati più specifici rispetto
all’organizzazione dei singoli nodi, ad esempio:

-  informazioni sull’aggiornamento della pagina
-  importanza della pagina rispetto ad altre URL dello stesso sito
-  informazioni relative a video e immagini
-  informazioni relative all’organizzazione dei documenti

`Come generare e inviare una sitemap a Google
<https://support.google.com/webmasters/answer/183668?hl=it&ref_topic=4581190>`__

È possibile inviare una sitemap a Google anche tramite il tool `Search
Console <#webmaster-tools-search-console-di-google>`__ È possibile
inoltre generare sitemap XML per:

-  `le pagine in lingue alternative <https://support.google.com/webmasters/answer/2620865?hl=it&ref_topic=6080646>`__
-  `i video <https://support.google.com/webmasters/answer/80471?hl=it&ref_topic=6080646>`__
-  `le immagini <https://support.google.com/webmasters/answer/178636?hl=it&ref_topic=6080646>`__

File robots.txt
^^^^^^^^^^^^^^^

Per ottimizzare i processi di scansione dei crawler dei motori di
ricerca è possibile utilizzare il file robots.txt. Un file robots.txt è
un file di testo memorizzato nella directory principale del sito che ha
la finalità di indicare ai crawler dei motori di ricerca quali parti del
sito non sono accessibili e quindi controllare il traffico di scansione.

Non si deve utilizzare il file robots.txt per nascondere le pagine web
dai risultati di ricerca.

`Informazioni sui file robots.txt
<https://support.google.com/webmasters/answer/6062608?hl=it>`__

`Come impedire la visualizzazione di una pagina del sito sui motori di
ricerca <https://developers.google.com/webmasters/control-crawl-index/docs/robots_meta_tag>`__

Tempi di caricamento delle pagine
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

La rapidità di caricamento di una pagina web è presa in considerazione
dai crawler dei motori di ricerca come elemento che concorre ad un
migliore posizionamento del contenuto nel ranking dei risultati di
ricerca.

È consigliabile effettuare controlli periodici sulle velocità di
caricamento delle pagine e i tempi di risposta del server, soprattutto
da dispositivi mobili.

`Risorse per lo sviluppo di pagine ottimizzate per i dispositivi
mobili <https://support.google.com/webmasters/answer/72462?hl=it&ref_topic=2370586>`__

Approfondimento: le pagine AMP (Accelerated Mobile Pages) per i contenuti di tipo “news”
''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''

Per determinate tipologie di contenuto - in particolare le news - è
possibile implementare il formato AMP (Accelerated Mobile Pages) di
Google. Il formato AMP è stato lanciato nel 2015 per migliorare le
prestazioni del mobile web, riducendo la velocità di caricamento delle
pagine.

`Linee guida di Google Search per le pagine AMP
<https://support.google.com/webmasters/answer/6340290?hl=it>`__

`Il progetto AMP <https://www.ampproject.org/it/>`__

`Guida all'implementazione di pagine AMP
<https://developers.google.com/search/docs/guides/use-AMP-HTML>`__

Dati strutturati
^^^^^^^^^^^^^^^^

Il markup con dati strutturati è una tecnica che consente di
personalizzare l’aspetto di un sito nella ricerca di Google o di altri
motori di ricerca. Includendo dei dati strutturati all’interno dei
contenuti è possibile inserire informazioni aggiuntive e/o strumenti di
interazione con il sito nell’aspetto standard dei risultati di ricerca,
ad esempio:

-  contatti e indirizzo dell’amministrazione
-  rating delle pagine
-  box di search in stile sitelink
-  breadcrumbs

Il markup con dati strutturati si basa sul vocabolario
http://schema.org/

`Guida di Google all’implementazione dei dati strutturati
<https://developers.google.com/search/docs/guides/intro-structured-data>`__

`Strumento per testare la corretta implementazione dei dati strutturati
<https://search.google.com/structured-data/testing-tool?hl=it>`__

Migrazione SEO di un sito
^^^^^^^^^^^^^^^^^^^^^^^^^

Quando si pianifica la migrazione di un sito è necessario fare in modo
di non perdere la rilevanza acquisita sui motori di ricerca e di
indirizzare gli utenti verso le nuove pagine nella maniera meno
problematica possibile.

Si consiglia quindi di:

-  realizzare una mappatura di tutte le URL del sito, che includa anche
   il linking interno
-  associare alle vecchie URL le nuove URL, per poter in seguito
   preparare i redirect
-  per le URL alle quali non verrà associata alcuna nuova URL, preparare
   una pagina 404 personalizzata, che aiuti l’utente a proseguire la
   navigazione nel nuovo sito
-  configurare il server impostando dei redirect di tipo 301
-  modificare la sitemap XML del sito
-  laddove possibile, aggiornare i backlinks ricevuti dal sito
-  comunicare ai crawler di Google un eventuale cambiamento del dominio
   tramite la Search Console

`Ulteriori informazioni sui redirect 301
<https://support.google.com/webmasters/answer/93633>`__

I fattori off-page
~~~~~~~~~~~~~~~~~~

Link building
^^^^^^^^^^^^^

In ottica di ottimizzazione SEO di un sito, è necessario curare e
monitorare iterativamente il processo di costruzione della rete di link
che il sito riceve dall’esterno (inbound links).

I motori di ricerca valutano la natura, la provenienza e la qualità di
tali link più che la loro quantità, considerandoli un elemento di
autorevolezza del sito soprattutto se questi provengono da siti
altrettanto autorevoli e se il loro processo di acquisizione è
considerato spontaneo.

I motori di ricerca penalizzano infatti le pratiche volte ad
incrementare massivamente il numero di link in ingresso (acquisti,
scambi di link forzosi…)

Per capire quali sono i link inbounds di un sito web è possibile:

-  utilizzare la `Search Console di
   Google <#webmaster-tools-search-console-di-google>`__
-  utilizzare tools ad hoc come `Open Site
   Explorer <https://moz.com/researchtools/ose/>`__ o `Ahrefs Site
   Explorer <https://ahrefs.com/site-explorer>`__
-  utilizzare l’operatore *link:sitoweb.it* nella `ricerca
   Google <https://support.google.com/webmasters/answer/35256?hl=it>`__

Webmaster tools: Search Console di Google
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Search Console è una risorsa online offerta gratuitamente da Google che
consente di monitorare, gestire e ottimizzare la presenza di un sito o
di un’applicazione mobile nei risultati di ricerca.

Search Console consente ad esempio di ottenere indicazioni sull’aspetto
di un sito web nei risultati di ricerca Google o informazioni rispetto
al traffico di ricerca; permette di verificare lo stato di
indicizzazione delle pagine così come di monitorare e correggere
problemi di varia natura legati al sito.

Con Search Console è possibile:

-  verificare lo stato di indicizzazione dei contenuti del sito
-  verificare lo stato della scansione dei crawler di Google sulle
   pagine del sito ed eventuali errori
-  testare i file robots.txt
-  testare la sitemap del sito, se presente
-  gestire i parametri URL durante la scansione dei crawler
-  rimuovere temporaneamente gli URL di un sito dai risultati di ricerca
-  informare Google rispetto al cambiamento di dominio di un sito
-  informare Google di un eventuale passaggio del sito da protocollo
   http a https
-  sapere per quali query è stato visualizzato il sito nei risultati di
   ricerca Google
-  conoscere i backlinks del sito e relativi anchor
-  monitorare i link interni
-  monitorare il corretto funzionamento del tag hreflang nel caso di
   siti multilingua
-  monitorare e correggere i problemi di usabilità del sito su
   dispositivi mobili
-  verificare la corretta implementazione di eventuali dati strutturati
   e schede informative (`rich
   cards <https://support.google.com/webmasters/answer/6381755>`__)
-  rilevare criticità nell’HTML per favorire e migliorare l’esperienza
   utente sul sito
-  rilevare e correggere eventuali criticità correlate alle pagine AMP
   (accelerated mobile pages)
-  monitorare e risolvere i problemi di malware o spam per tenere pulito
   il tuo sito

Approfondimenti
^^^^^^^^^^^^^^^

`Come configurare un sito web in Search Console
<https://support.google.com/webmasters/answer/34592?hl=it&ref_topic=3309469>`__

`Centro assistenza Search Console
<https://support.google.com/webmasters#topic=3309469>`__

`Come collegare Search Console a Google Analytics
<https://support.google.com/analytics/answer/1308621?hl=it>`__

Utile da sapere
^^^^^^^^^^^^^^^

*Una app Android deve essere pubblicata in Google Play per poter essere
aggiunta a Search Console.*

`Come configurare una app in Search Console
<https://support.google.com/webmasters/answer/6178088>`__
