Sviluppo Web
-----------

La realizzazione di un sito web professionale per un servizio della PA
prevede, come abbiamo visto, un iter di progettazione approfondito e
sistematico.

Oltre a questo, durante le fasi iniziali dello sviluppo, è fondamentale
dedicare tempo e risorse ad alcune attività molto importanti, che avranno
impatto sull'intero ciclo di vita del progetto:

* una analisi di **componenti** (librerie, linguaggi, documentazione, ecc.) e
  **best practices** già utilizzate e validate dalla comunità, che possano
  **semplificare e standardizzare** la realizzazione del servizio
* una revisione dei requisiti di progetto con lo scopo di ottenere un
  **documento di specifiche** condiviso, che possa anche definire **ruoli** e
  **responsabilità**
* la selezione di una metodologia di **sviluppo agile** ottimale per il team di
  lavoro, e una definizione precisa delle procedure di comunicazione, di
  testing e di rilascio

Contestualmente a questa fase di *kick-off* tecnico, è auspicabile avviare sin
da subito una fase di prototipazione avanzata, con la quale iniziare a
validare in modo iterativo ogni progresso raggiunto. Questo può essere
ottenuto sia con classici test manuali, che attraverso un’adeguata *continuous
integration* che faccia uso di test automatici.


Progressive Enhancement e Graceful Degradation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nel paragrafo dedicato al paradigma mobile first era stato introdotto
brevemente il principio di *progressive enhancement*, in quanto fondante per
uno sviluppo web flessibile e a prova di future evoluzioni di dispositivi e
browser. Tale principio è spesso associato a quello di *graceful degradation*,
che andremo a descrivere di seguito.

Per progressive enhancement si intende una pratica **raccomandabile** nello
sviluppo di una nuova applicazione web, con la quale si inizia da un nucleo
solido e irrinunciabile di contenuti che vengono **arricchiti** via via che il
dispositivo utilizzato dal cittadino è più performante e all’avanguardia.

Al contrario, nel caso della graceful degradation, con la programmazione ci
si fa carico di verificare che l’interfaccia, inizialmente pensata per i
dispositivi più moderni, rimanga navigabile e permetta comunque di accedere
alle sue funzioni fondamentali anche man mano che viene usata attraverso
tecnologie meno moderne o meno interattive.

In questo caso, si può pensare anche in termini di *tolleranza* del sito
all'assenza di alcune funzionalità.

Come si potrà notare, si tratta in fondo di due risposte diverse alla stessa
esigenza: rendere il contenuto **accessibile** su dispositivi con **diverse
caratteristiche e potenzialità**.


Supporto browser
~~~~~~~~~~~~~~~~

Come regola generale, per la realizzazione di un servizio web per la PA, è
necessario assicurare la compatibilità con versioni dei browser che abbiano
una penetrazione media tra la popolazione di almeno **1 persona ogni 100
abitanti**.
È importante analizzare regolarmente le statistiche sull’utilizzo dei
dispositivi e delle diverse risoluzioni che gli utenti adoperano per accedere
al sito, con lo scopo di abbracciare una base di utenti che copra più del
**95% delle versioni utilizzate in Italia**. Per fare questo, ci si può avvalere
di diverse sorgenti di dati: una delle più usate è
`StatCounter <http://gs.statcounter.com/browser-version-market-share/all/italy>`_.

Come ampiamente descritto nel paragrafo precedente, non è necessario che
l’interfaccia del sito sia assolutamente identica sui diversi dispositivi;
graceful degradation significa tuttavia garantire un’esperienza utente
**equivalente**, graficamente **coerente** e **completa** nelle sue
funzionalità. Vediamo come sia possibile farlo.


Feature Detection
~~~~~~~~~~~~~~~~~

Tecnicamente, l'approccio appena analizzato può essere realizzato attraverso
la cosiddetta feature detection: il sito web può rilevare una miriade di
proprietà che caratterizzano il metodo di accesso al sito da parte del
cittadino.

.. admonition:: Nota
   Si prega di non confondere la feature detection con la pratica, in passato
   molto diffusa, di utilizzare lo user-agent (ovvero quale browser e quale
   sistema operativo è connesso) per differenziare i servizi forniti. È
   infatti scoraggiato l'utilizzo di user-agent a tale scopo, in quanto
   impreciso e difficilmente mantenibile vista la quantità di diversi
   dispositivi in costante uscita sul mercato.

Attraverso una feature detection puntuale, è possibile sapere come indirizzare
ogni aspetto dell'informazione che si vuole trasmettere. Tali caratteristiche
possono spaziare dallo schermo utilizzato, in termini di dimensioni,
risoluzione e densità dei pixel, fino ai metodi di input (mouse, touch-screen,
tastiera, input vocale, ecc.); senza dimenticare le **opzioni per la stampa** e
le tecnologie di **ausilio per le persone con disabilità**.

Ad esempio, attraverso semplici media-queries nel CSS, è possibile mostrare
versioni diverse di una pagina web a seconda che il cittadino stia utilizzando
uno smartphone, un televisore o voglia stampare la pagina stessa con la
propria stampante.

Sia CSS che Javascript permettono quindi di rilevare la presenza puntuale di
determinate caratteristiche nei dispositivi usati.

Javascript permette di analizzare qualsiasi funzionalità presente tra le Web
API, oltre a poter conoscere praticamente **ogni dettaglio dell'utente** che è
collegato. Ad esempio, attraverso la geo-localizzazione di un dispositivo, è
possibile fornire un servizio più preciso a seconda della posizione dell'utente
nello spazio, a patto che tale *feature* sia disponibile nel dispositivo
utilizzato. Ecco come si può realizzare::

  if("geolocation" in navigator) {
    navigator.geolocation.getCurrentPosition(function(position) {
     // posso ottenere la posizione
    });
  } else {
    // il browser non può fornire la posizione
  }

CSS ha capacità più limitate, ma ad esempio attraverso la regola *@support*
(in modo simile a quanto avviene per la più conosciuta regola *@media*), può
verificare la corretta **interpretazione di proprietà CSS** da parte dei browser
su cui viene usata. Ecco, ad esempio, come si può verificare attraverso il
codice se il browser prevede il supporto della funzionalità CSS grid::

  @supports not (display: grid) {
    .nome-classe {
      float: right;
    }
  }

Esistono moltissimi strumenti per la feature detection e per le pratiche di
polyfill e shim (librerie o frammenti di codice che riescono ad arginare le
differenze tra i vari Browser nel pieno supporto di alcune funzionalità); di
seguito ne sono riportate alcuni.


Strumenti e risorse
~~~~~~~~~~~~~~~~~~~

Gli strumenti più curati per la realizzazione di interfacce coerenti con le
linee guida di design sono disponibili nella sezione
`Web Toolkit <https://designers.italia.it/kit/web-toolkit/>`_ della community di
*Designers Italia*.

Tra i progetti open-source disponibili in rete,
`Modernizr <https://modernizr.com/>`_ è la libreria
Javascript più usata per la feature detection, poiché può essere facilmente
personalizzata con le feature che si desidera verificare e aggiunge comode
classi al tag HTML per far sì che, in base alle *feature* identificate, si
riesca a modellare la pagina attraverso CSS.

Una fonte di dati molto utile invece per una verifica a monte delle feature
disponibili nei browser è `caniuse.com <https://caniuse.com/>`_. Tale strumento
permette di ricercare e verificare se per i browser supportati è necessaria
una gestione ad-hoc di determinate funzionalità oppure no.

Una volta individuati i dispositivi supportati e le feature da realizzare,
è buona norma scegliere uno stack di sviluppo che ottimizzi il lavoro.

In ambito CSS, è ormai pressoché d'obbligo l'utilizzo di **pre-processori**
(come `SASS <https://sass-lang.com/>`_, `LESS <http://lesscss.org/>`_,
`Stylus <http://lesscss.org/>`_ o `PostCSS <http://postcss.org/>`_, per citare i
principali), che migliorano drasticamente la leggibilità e la modularità del
codice sorgente, agevolando nel contempo l'applicazione di pratiche virtuose
quali l'utilizzo di `BEM <http://getbem.com/>`_, una metodologia per scrivere
classi CSS “parlanti”, o di `Autoprefixer <https://autoprefixer.github.io/>`_,
per la gestione automatica di prefissi CSS a supporto dei vari motori di
rendering presenti nei browser.

Per quanto riguarda Javascript invece, la scelta degli strumenti è talmente
ampia e mutevole che delineare uno scenario ottimale in termini di framework o
librerie non avrebbe senso senza un’analisi approfondita del progetto da
realizzare. In questo ambito è necessaria una formazione continua (le risorse
sul web non mancano, un paio su tutte sono la
`guida di MDN <https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics>`_
e `You don’t know JS <https://www.gitbook.com/book/maximdenisov/you-don-t-know-js/details>`_,
in inglese), e un'attenzione particolare a ciò che permetta di ottenere codice
**manutenibile**, **scalabile** e **performante**, senza appesantire
l'esecuzione e l'interfaccia utente.

Alcune pratiche sono comunque sempre auspicabili, come la **compressione** del
codice e il caricamento dei file Javascript stessi in modo **asincrono** oppure
al termine della pagina HTML, al fine di non bloccare il rendering della pagina
stessa; o ancora, l’utilizzo di strumenti di **analisi della sintassi** come
`ESLint <https://eslint.org/>`_ o `StyleLint <https://stylelint.io/>`_ per rendere
il codice leggibile e coerente con regole condivise dalla comunità degli
sviluppatori.

In caso di applicazioni complesse o di grandi dimensioni, è bene considerare
l’utilizzo di strumenti come `Rollup <https://rollupjs.org/>`_ o
`Webpack <https://webpack.js.org/>`_ per la gestione di codice modulare,
`Babel <https://babeljs.io/>`_ per l’uso di Ecmascript come codice sorgente, e
più in generale l’utilizzo dell’ecosistema node.js (attraverso *npm* o *yarn*)
per la gestione di dipendenze.

Per questo tipo di applicazioni con uso intensivo di Javascript, anche la
metodologia di lavoro è fondamentale: un approccio
`BDD <https://it.wikipedia.org/wiki/Behavior-driven_development>`_ per la stesura
delle funzionalità, e l’uso della stessa metodologia per l’applicazione di test
funzionali, unit test e test di integrazione, può essere elemento chiave per
il buon funzionamento e la solidità dell’applicazione.


Misurare le prestazioni
~~~~~~~~~~~~~~~~~~~~~~~

Così come avviene per il design di un sito, anche le sue prestazioni
concorrono ad una maggiore facilità di utilizzo. In questo senso, è bene
differenziare due principali ambiti che possono avere impatto determinante
sull'esperienza finale dell'utente: i **tempi di caricamento** della pagina e
le **performance di esecuzione** della pagina stessa.

Per analizzare i tempi di caricamento e *rendering* della pagina web si possono
utilizzare semplici strumenti online come `Google PageSpeed
Insights <https://developers.google.com/speed/pagespeed/insights/>`_,
`WebPagetest.org <http://www.webpagetest.org/>`_ o tool di integrazione più
avanzati come `sitespeed.io <https://www.sitespeed.io/>`_. Con questi strumenti,
è possibile verificare problemi di immediata risoluzione, come l’utilizzo di
immagini esageratamente grandi o poco ottimizzate, oppure calibrare altri
fattori, come sfruttare al meglio il caching del browser o dare priorità ai
contenuti immediatamente visibili.

Per ottenere invece informazioni più dettagliate riguardo eventuali
inefficienze di codice a *runtime*, si può fare riferimento agli strumenti di
analisi presenti sui principali browser, come gli ottimi tools per l’analisi
delle prestazioni presenti in
`Firefox <https://developer.mozilla.org/it/docs/Tools/Prestazioni>`_ e
`Chrome <https://developers.google.com/web/tools/chrome-devtools/evaluate-performance/>`_,
i quali possono dare indicazioni su eventuali problemi che avvengono durante
la navigazione stessa di una singola pagina.

.. note::
   Chrome developer tools può inoltre fornire un'analisi approfondita di una
   pagina web nella sua sezione *"Audits"*, permettendo di portare a galla
   problemi in ambito di *progressive web apps*, *performance*,
   *accessibilità*, e *utilizzo di best practices*.

In caso di progettazione di progressive web apps ideate per essere usate
principalmente su dispositivi mobili, è bene tenere a mente anche il concetto
di offline first, fornendo un'esperienza di base anche in caso di limitata
connettività.