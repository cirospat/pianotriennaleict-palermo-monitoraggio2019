
.. _h3b9431e3a511972f35d463f382d2:

Definizione Standard per il paniere di dataset degli Enti Locali
################################################################


.. toctree::  
    :maxdepth: 4
    :caption: Definizione standard paniere

    index


.. toctree::  
    :maxdepth: 4
    :caption: Privacy

    privacy

L’obiettivo del documento è quello di \ |STYLE0|\  relativo ai contenuti minimi che ciascun dataset deve contenere.

Definire uno standard è un lavoro preliminare importante per:

#. Migliorare il livello di \ |STYLE1|\  dei dataset

#. Favorire la \ |STYLE2|\  delle informazioni

#. Permettere il \ |STYLE3|\  tra i dati di enti diversi

#. Facilitare la \ |STYLE4|\  dei dati

.. _h1f7b7e213a5f3135174d2478541f3671:

METODO DI LAVORO
****************

Il documento è suddiviso in paragrafi che rappresentano le 10 categorie di dataset presenti nel paniere:

#. Ambiente

#. Commercio

#. Cultura

#. Energia

#. Mobilità e trasporti

#. Sicurezza

#. Statistica

#. Territorio

#. Trasparenza

#. Turismo

Per ogni dataset è presente una tabella contenente una \ |STYLE5|\ , sulla base delle esperienze raccolte provenienti da diverse amministrazioni.

I contenuti minimi contengono dei \ |STYLE6|\  e dei \ |STYLE7|\  nella colonna “Obbligo” di ciascuna tabella (es. dataset #36 Provvedimenti dei dirigenti). Perchè il dataset possa essere considerato completo, è necessario inserire sia le colonne relative alle informazioni mandatorie compilate (M) sia le colonne, anche non compilate, relative alle informazioni opzionali (O). 

Gli Enti partecipanti possono utilizzare i commenti per proporre di:

* modificare i campi 

* inserire nuovi campi

* compilare i campi vuoti

* fare commenti aperti in cui inserire dubbi, suggerimenti, ecc.  

Il Team Open Data Lombardia si occuperà di raccogliere i commenti, di integrare il documento e di rispondere a eventuali dubbi espressi dagli Enti.

.. _h455c1263337b5d692f635d441e78625c:

FORMATO DEI DATI
****************

\ |STYLE8|\ 

* Numero

* Testo

* Web URL

* Booleano (spunta)

* Data

* Valuta (sconsigliato)

* Percentuale

* Coppia di coordinate geografiche (location)

\ |STYLE9|\ 

La piattaforma \ |LINK1|\  ingloba una serie di funzionalità avanzate sui dataset di tipo tabellare (Datasets), che permette di aggiungere funzionalità fruibili direttamente on-line, quali ad esempio l’ordinamento crescente/decrescente, link ad un elemento esterno e altro.

Per permettere l’\ |STYLE10|\ , è necessario scegliere un formato «ordinabile» (numero,data).

Per una \ |STYLE11|\ , occorre scegliere un numero con il punto come separatore dei decimali

Per una \ |STYLE12|\ , occorre inserire una coppia di dati, in formato numerico e con \ |STYLE13|\  (ad es. 46.4039704°, 9.3668236°), dove i numeri dovranno avere un punto come separatore. Un campo conterrà la latitudine e l’altro la longitudine: questi due campi popoleranno una colonna di tipo “location” che verrà usata per creare una vista derivata di tipo «mappa».

\ |STYLE14|\ ”

La piattaforma \ |LINK2|\  è costruita con tutti i tipi di formattazione di date e numeri in uso negli USA secondo le specifiche ISO 8601.

Per ovviare ad inconvenienti di rappresentazione, è importante che i numeri contenuti nel dataset non presentino separatori delle migliaia e che i decimali vengano inseriti con il punto come segno separatore.

La visualizzazione finale potrà comunque essere modificata dall’interfaccia utente.

.. _h2c1d74277104e41780968148427e:




\ |STYLE15|\ 

Per la rappresentazione geografica, è possibile:

#. caricare uno shapefile come allegato

#. importare uno shapefile. Questa opzione consente di:

* visualizzare i dati su mappa

* scaricare i dati in diversi formati

* utilizzare le API

Per la specifica degli shapefile fare riferimento a \ |LINK3|\ 

\ |STYLE16|\  Se si utilizza un sistema di coordinate diverso dal WGS-84, occorre specificare questa informazione e includere il sistema utilizzato nello shapefile.

.. _h2591956d562d53487858431c49e1f:

FREQUENZA DI AGGIORNAMENTO TEMPESTIVA
*************************************

\ |STYLE17|\ 

Anche se i dati non cambiano, occorre quindi specificare nei metadati che i dati pubblicati sono ancora validi: in questo caso, \ |STYLE18|\ . 

Per modificare la data di ultimo aggiornamento dei metadati occorre cliccare su "Modifica Metadata" e modificare la "Data di aggiornamento" presente nella sezione "Frequenza di aggiornamento".


|REPLACE1|


+------------------------------------------------------------------------------------------------------------------+
|Per ulteriori informazioni consultare la pagina dedicata all’evento formativo del 22 marzo scorso: “\ |LINK4|\ ”. |
+------------------------------------------------------------------------------------------------------------------+

 


.. _hb2252384d6f2d652c47455b4f755c4:

1.     AMBIENTE
===============

.. _h613337737e83b26d2f785122671612:

#1     Carta degli incendi (DEFINITIVO)
---------------------------------------

\ |STYLE19|\  Mappa e scheda delle aree percorse da incendi 

\ |STYLE20|\  Dataset geografico (Shapefile)

\ |STYLE21|\  Mensile

Obblighi normativi: \ |LINK5|\ , in particolare art. 10 c. 1 e 2

Interessante il progetto civico: \ |LINK6|\ 

Sono possibili 2 opzioni di pubblicazione:

#. Tabella con informazioni catastali dell’area percorsa dal fuoco (obbligatoria) + shapefile dell’area (opzionale)

#. Inserire nello zip dello shapefile 2 layer: uno con le particelle catastali dell’area percorsa dal fuoco e uno con l’area completa (soluzione con GIS)

+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                                                                                                                                                                                   |Tipo  |Obbligo|
+===================+==============================================================================================================================================================================================================================================================================================+======+=======+
|Data_Inc           |Data dell’incendio                                                                                                                                                                                                                                                                            |Data  |M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE22|\       |Foglio in cui è presente la particella percorsa dal fuoco nella sua totalità o solo parzialmente                                                                                                                                                                                              |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE23|\       |Mappale in cui è presente la particella percorsa dal fuoco nella sua totalità o solo parzialmente                                                                                                                                                                                             |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE24|\       |Particella catastale della zona interessata                                                                                                                                                                                                                                                   |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE25|\       |Area della particella percorsa dal fuoco (mq)                                                                                                                                                                                                                                                 |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE26|\       |Area totale della particella (mq)                                                                                                                                                                                                                                                             |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE27|\       |Indicare se esiste il vincolo (15 anni) che impone il mantenimento della destinazione d’uso preesistente all’incendio impedendone la modifica (SI/NO)                                                                                                                                         |Testo |O      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE28|\       |Indicare se è vietata (vincolo 10 anni) la realizzazione di edifici nonché di strutture e infrastrutture finalizzate ad insediamenti civili ed attività produttive e il divieto di pascolo e di caccia per 10 anni, limitatamente ai soprassuoli delle zone boscate percorsi dal fuoco (SI/NO)|Testo |O      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE29|\       |Indicare se esiste il divieto (vincolo 5 anni) di attività di rimboschimento e di ingegneria ambientale sostenute con risorse finanziarie pubbliche (SI/NO)                                                                                                                                   |Testo |O      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+

.. _h73633d4a4c4c22737a3215b39c2b3b:

#17     Aree Verdi (DEFINITIVO)
-------------------------------

\ |STYLE30|\  Elenco delle aree verdi del territorio 

\ |STYLE31|\  Dataset geografico (Shapefile)

\ |STYLE32|\  Tempestiva

Esempio 1: \ |LINK7|\ 

Esempio 2: \ |LINK8|\  


+-------------------+-------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                      |Tipo  |Obbligo|
+===================+=================================================+======+=======+
|Denom              |Nome dell’area o descrizione                     |Testo |M      |
+-------------------+-------------------------------------------------+------+-------+
|\ |STYLE33|\       |Via/piazza, ecc.                                 |Testo |M      |
+-------------------+-------------------------------------------------+------+-------+
|\ |STYLE34|\       |Nome della via/piazza                            |Testo |M      |
+-------------------+-------------------------------------------------+------+-------+
|\ |STYLE35|\       |Superficie dell’area (espressa in metri quadrati)|Numero|M      |
+-------------------+-------------------------------------------------+------+-------+

.. _h534b1577195b553752123805a281950:

#18     Aree Verdi Informazioni (DEFINITIVO)
--------------------------------------------

\ |STYLE36|\  Informazioni sulle aree verdi

\ |STYLE37|\  Dataset tabellare

\ |STYLE38|\  Tempestiva

NOTA: In seguito alle segnalazioni degli Enti è stato creato un tracciato che contiene informazioni relative alle aree verdi comunali e sovracomunali.


+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo  |Obbligo                      |
+===================+==========================================================================================================================================+======+=============================+
|Anno               |Anno di riferimento                                                                                                                       |Numero|M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE39|\       |Nome dell’area o descrizione                                                                                                              |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE40|\       |Tipologia di area (Comunale/Sovracomunale)                                                                                                |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE41|\       |Codice catastale del comune o dei comuni in cui è ubicata l’area, inserendo tra l’uno e l’altro il separatore pipe                        |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE42|\       |Nome del comune o dei comuni in cui è ubicata l’area, inserendo tra l’uno e l’altro il separatore pipe                                    |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE43|\       |Superficie dell’area (espressa in metri quadrati)                                                                                         |Numero|M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE44|\       |Superficie a prato (espressa in metri quadrati)                                                                                           |Numero|O                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE45|\       |Presenza di recinzione (SI/NO/Non applicabile)                                                                                            |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE46|\       |Presenza di aree giochi per bambini (SI/NO/Non applicabile)                                                                               |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE47|\       |Permesso di introdurre animali (SI/NO/Non applicabile)                                                                                    |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE48|\       |Numero di fontanelle presenti                                                                                                             |Numero|O                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE49|\       |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo |M (se presente la recinzione)|
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h6c466e2d2d97084e145847153214d:

#34 Elenco degli impianti di depurazione (DEFINITIVO)
-----------------------------------------------------

\ |STYLE50|\  Elenco degli impianti di depurazione pubblici di competenza, georeferenziati 

\ |STYLE51|\  Dataset tabellare

\ |STYLE52|\  Mensile

Esempio: \ |LINK9|\  


+-------------------+--------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                             |Tipo  |Obbligo|
+===================+========================================================+======+=======+
|ID_Impianto        |Codice identificativo dell’impianto                     |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE53|\       |Nome dell’impianto                                      |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE54|\       |Codice identificativo del comune                        |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE55|\       |Comune di riferimento                                   |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE56|\       |Comuni serviti dall’impianto                            |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE57|\       |Indicare il corpo idrico recettore (es. nome “fiume x”) |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE58|\       |Altezza espressa in mslm                                |Numero|M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE59|\       |Via in cui si trova l’impianto                          |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE60|\       |Longitudine                                             |Numero|M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE61|\       |Latitudine                                              |Numero|M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE62|\       |Data di avvio                                           |Data  |O      |
+-------------------+--------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h43321d10544d6f71592d465d7a1f3b4d:

#35 Quantità rifiuti prodotta (DEFINITIVO)
------------------------------------------

\ |STYLE63|\  Quantità di rifiuti prodotti dalla raccolta differenziata e non differenziata, specificandone categoria e modalità di raccolta. 

\ |STYLE64|\  Dataset tabellare

\ |STYLE65|\  Mensile

Esempio 1: \ |LINK10|\ 

Esempio 2: Comune di Isso -  \ |LINK11|\ 


+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                               |Tipo  |Obbligo|
+===================+==========================================================================================================================+======+=======+
|Anno               |Anno di riferimento                                                                                                       |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE66|\       |Indicare se si tratta di rifiuti non differenziati, raccolta differenziata o Inerti e rifiuti da costruzione e demolizione|Testo |M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE67|\       |Indicare la categoria di rifiuti (es. carta e cartone, vetro, ecc.)                                                       |Testo |M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE68|\       |Codice della Categoria rifiuti                                                                                            |Testo |O      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE69|\       |Indicare la modalità di raccolta (es. meccanizzata, porta a porta, area attrezzata)                                       |Testo |M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE70|\       |Indicare il mese di riferimento in numero                                                                                 |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE71|\       |Indicare la quantità in kg                                                                                                |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h5a82773c2c5d1dc685335262c4f51:

2.     COMMERCIO
================

.. _h4a55719171347357e636635565315a:

#20        Pratiche SUAP (DEFINITIVO)
-------------------------------------

\ |STYLE72|\  Elenco pratiche gestite dallo Sportello Unico Attività Produttive

\ |STYLE73|\  Dataset tabellare

\ |STYLE74|\  Mensile

Esempio 1: \ |LINK12|\  

Esempio 2: \ |LINK13|\  


+-------------------+-----------------------------------+-------+-------+
|Denominazione Campo|Descrizione                        |Tipo   |Obbligo|
+===================+===================================+=======+=======+
|Anno               |Anno di riferimento                |Numero |M      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE75|\       |Codice identificativo della pratica|Testo  |O      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE76|\       |Ragione sociale del richiedente    |Testo  |M      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE77|\       |Numero di protocollo               |Testo  |M      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE78|\       |Indicare l’oggetto della richiesta |Testo  |O      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE79|\       |Data della richiesta               |Data   |M      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE80|\       |Link alla pratica                  |Web URL|O      |
+-------------------+-----------------------------------+-------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h65512721d471161b6456c5353295:

#45        Servizi alla persona (DEFINITIVO)
--------------------------------------------

\ |STYLE81|\  Elenco e informazioni relative ai servizi alla persona

\ |STYLE82|\  Dataset tabellare

\ |STYLE83|\  Tempestiva

Esempio: \ |LINK14|\  

+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo  |Obbligo|
+===================+==========================================================================================================================================+======+=======+
|Denominazione      |Denominazione attività                                                                                                                    |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE84|\       |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                                                                           |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE85|\       |Breve descrizione del tipo di servizio offerto (ad esempio parrucchiere, estetista, ecc.)                                                 |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE86|\       |Superficie destinata all’esercizio dell’attività (espressa in metri quadrati)                                                             |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE87|\       |Superficie destinata ad altri usi (espressa in metri quadrati)                                                                            |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE88|\       |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE89|\       |Longitudine                                                                                                                               |Numero|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE90|\       |Latitudine                                                                                                                                |Numero|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h192d703349757a442f2040344a7476f:

#47    Pubblici esercizi (DEFINITIVO)
-------------------------------------

\ |STYLE91|\ : Informazioni sugli esercizi pubblici con dati georeferenziati

\ |STYLE92|\  Dataset tabellare

\ |STYLE93|\ : Tempestiva

+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo  |Obbligo|
+===================+==========================================================================================================================================+======+=======+
|Denominazione      |Denominazione esercizio                                                                                                                   |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE94|\       |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                                                                           |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE95|\       |Tipologia di esercizio (ad esempio bar, ristorante ecc.)                                                                                  |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE96|\       |Tipologia di somministrazione (ad esempio bevande, pasti ecc.)                                                                            |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE97|\       |Modalità di somministrazione (ad esempio al banco, al tavolo ecc.)                                                                        |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE98|\       |Superficie destinata alla somministrazione (espressa in metri quadrati)                                                                   |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE99|\       |Presenza di WiFi pubblico (Si/No)                                                                                                         |Testo |O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE100|\      |Longitudine                                                                                                                               |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE101|\      |Latitudine                                                                                                                                |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE102|\      |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo |O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+

.. _h1216263d3b30172471575b782e2e3b7a:

3.       CULTURA
================

.. _h1e1aa304264214b219785d425e70:

#48   Eventi (DEFINITIVO)
-------------------------

\ |STYLE103|\ : Informazioni su eventi e manifestazioni 

\ |STYLE104|\  Dataset tabellare

\ |STYLE105|\ : Tempestiva

+-------------------+---------------------------------------------------------------+--------+---------------------------+
|Denominazione Campo|Descrizione                                                    |Tipo    |Obbligo                    |
+===================+===============================================================+========+===========================+
|Ubicazione         |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE106|\      |Anno di riferimento                                            |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE107|\      |Denominazione evento                                           |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE108|\      |Tipologia evento                                               |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE109|\      |Numero edizione dell’evento                                    |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE110|\      |Descrizione dell’evento                                        |Testo   |O                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE111|\      |Data di inizio dell’evento                                     |Data    |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE112|\      |Ora di inizio dell’evento                                      |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE113|\      |Data di conclusione dell’evento                                |Data    |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE114|\      |Ora di conclusione dell’evento                                 |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE115|\      |Link al sito web dell’evento                                   |Link Web|M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE116|\      |Link al programma dell’evento                                  |Link Web|M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE117|\      |Nome dell’ente che organizza l’evento                          |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE118|\      |Indirizzo email dell’ente organizzatore                        |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE119|\      |Telefono dell’ente organizzatore                               |Testo   |O                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE120|\      |Evento gratuito (SI/NO)                                        |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE121|\      |Prezzo biglietto                                               |Testo   | M (se evento non gratuito)|
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE122|\      |Longitudine                                                    |Numero  |O                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE123|\      |Latitudine                                                     |Numero  |O                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h161c2f3833454e4976932653c2b775:

#50 Beni artistici e architettonici (DEFINITIVO)
------------------------------------------------

\ |STYLE124|\ : Beni artistici e architettonici del territorio

\ |STYLE125|\  Dataset tabellare

\ |STYLE126|\ : Tempestiva

Esempio: \ |LINK15|\  

+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|Denominazione Campo|Descrizione                                                                               |Tipo   |Obbligo|
+===================+==========================================================================================+=======+=======+
|ID_Bene            |Codice identificativo del bene artistico o architettonico                                 |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE127|\      |Denominazione del bene artistico o architettonico                                         |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE128|\      |Descrizione del bene                                                                      |Testo  |O      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE129|\      |Inserire la tipologia di bene (es. Museo, villa, parco…come classificato qui \ |LINK16|\ )|Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE130|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                           |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE131|\      |Indirizzo email per richiedere informazioni                                               |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE132|\      |Recapito telefonico a cui richiedere informazioni                                         |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE133|\      |Link al sito web                                                                          |Web URL|M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE134|\      |Eventuali ulteriori informazioni                                                          |Testo  |O      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE135|\      |Longitudine                                                                               |Numero |O      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE136|\      |Latitudine                                                                                |Numero |O      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h405b7c14e20627c163b5a181f5126:

4.       ENERGIA
================

.. _h31437f1420597a45737174704a683466:

#30 Albo provinciale manutentori impianti termici (DEFINITIVO)
--------------------------------------------------------------

\ |STYLE137|\ : Elenco manutentori impianti termici abilitati

\ |STYLE138|\  Dataset tabellare

\ |STYLE139|\ : Tempestiva

Esempio: \ |LINK17|\  

+-------------------+---------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                    |Tipo  |Obbligo|
+===================+===============================================================+======+=======+
|Nome               |Nome o ragione sociale del manutentore                         |Testo |M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE140|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo |M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE141|\      |Numero telefonico del manutentore                              |Numero|O      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE142|\      |Indirizzo email del manutentore                                |Testo |O      |
+-------------------+---------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h496c7f2d61647381a4a4c53306f344a:

5.       MOBILITÀ E TRASPORTI
=============================

.. _h71376c30591b534c645e1d4c7b187:

#3 Orario Trasporto Pubblico (DEFINITIVO)
-----------------------------------------

\ |STYLE143|\ : Il dataset contiene i dati relativi alle corse, agli orari e alle fermate del trasporto pubblico urbano ed extra-urbano (pianificato). 

\ |STYLE144|\  Dataset tabellare

\ |STYLE145|\ : Tempestiva

Si tratta di uno Zip file. Lo standard di riferimento è il GTFS. \ |LINK18|\ 

Esempio 1: \ |LINK19|\   

Esempio 2: \ |LINK20|\  

Esempio 3: \ |LINK21|\  

.. _h3761631274d34195427717075576131:

#8 Mappa ZTL (DEFINITIVO)
-------------------------

\ |STYLE146|\ : Mappa Zona a Traffico Limitato 

\ |STYLE147|\  Dataset geografico (Shapefile)

\ |STYLE148|\ : Tempestiva

Esempio: \ |LINK22|\  


+-------------------+--------------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                                   |Tipo |Obbligo|
+===================+==============================================================+=====+=======+
|Nome_ZTL           |Denominazione della ZTL                                       |Testo|M      |
+-------------------+--------------------------------------------------------------+-----+-------+
|\ |STYLE149|\      |Indicare il periodo di riferimento (es. annuale, estivo, ecc.)|Testo|M      |
+-------------------+--------------------------------------------------------------+-----+-------+
|\ |STYLE150|\      |Informazioni aggiuntive (es. orari)                           |Testo|M      |
+-------------------+--------------------------------------------------------------+-----+-------+

.. _h2c1d74277104e41780968148427e:




.. _h794ab20525873f625363207210359:

#9 Varchi ZTL (DEFINITIVO)
--------------------------

\ |STYLE151|\ : Informazioni sui  varchi della ZTL, georeferenziati

\ |STYLE152|\  Dataset tabellare

\ |STYLE153|\ : Tempestiva

Esempio: \ |LINK23|\  

+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo   |Obbligo|
+===================+==========================================================================================================================================+=======+=======+
|Via                |Nome della via in cui è posizionato il varco                                                                                              |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE154|\      |Tipologia del varco (es. videosorvegliato)                                                                                                |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE155|\      |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo  |O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE156|\      |Eventuali deroghe all’accesso (ad esempio velocipedi)                                                                                     |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE157|\      |Longitudine                                                                                                                               |Numero |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE158|\      |Latitudine                                                                                                                                |Numero |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE159|\      |Link alla pagina informativa, se presente sul sito web dell’ente                                                                          |Web URL|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h477818b50292f6c2d1821685f246:

#10 Parcheggi (DEFINITIVO)
--------------------------

\ |STYLE160|\ : Posizione e informazioni sui Parcheggi

\ |STYLE161|\  Dataset tabellare

\ |STYLE162|\ : Tempestiva

Esempio: \ |LINK24|\  

+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo  |Obbligo|
+===================+==========================================================================================================================================+======+=======+
|ID_Parcheggio      |Codice identificativo del parcheggio                                                                                                      |Testo |O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE163|\      |Tipologia del parcheggio (es. aperto, coperto)                                                                                            |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE164|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                                                                           |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE165|\      |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE166|\      |Longitudine                                                                                                                               |Numero|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE167|\      |Latitudine                                                                                                                                |Numero|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE168|\      |Indicare se il parcheggio è gratuito (SI/NO)                                                                                              |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+

.. _h7a387f69313ca44387272731b5f2b50:

#11   Piste ciclabili (DEFINITIVO)
----------------------------------

\ |STYLE169|\ : Tracciato delle piste ciclabili  piste ciclabili

\ |STYLE170|\  Dataset geografico (Shapefile)

\ |STYLE171|\ : Tempestiva

Esempio 1: \ |LINK25|\ 

Esempio 2: \ |LINK26|\ 

+-------------------+-------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                            |Tipo  |Obbligo|
+===================+=======================================================+======+=======+
|ID                 |Identificativo pista ciclabile                         |Testo |M      |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE172|\      |Breve descrizione                                      |Testo |M      |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE173|\      |Tipologia percorso, scegliendo tra le seguenti opzioni:|Testo |M      |
|                   |                                                       |      |       |
|                   |* ciclabile                                            |      |       |
|                   |                                                       |      |       |
|                   |* ciclopedonale                                        |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE174|\      |Indicare una delle seguenti opzioni:                   |Testo |M      |
|                   |                                                       |      |       |
|                   |* sede propria                                         |      |       |
|                   |                                                       |      |       |
|                   |* sede promiscua veicolare                             |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE175|\      |Tipo di fondo, scegliendo tra:                         |Testo |M      |
|                   |                                                       |      |       |
|                   |* asfaltato                                            |      |       |
|                   |                                                       |      |       |
|                   |* sterrato                                             |      |       |
|                   |                                                       |      |       |
|                   |* ciottolato                                           |      |       |
|                   |                                                       |      |       |
|                   |* pavimentato (es. resina)                             |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE176|\      |Lunghezza del percorso (espressa in metri)             |Numero|M      |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE177|\      |Larghezza del percorso (espressa in metri)             |Numero|O      |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE178|\      |Specificare una delle seguenti opzioni:                |Testo |M      |
|                   |                                                       |      |       |
|                   |* monodirezionale                                      |      |       |
|                   |                                                       |      |       |
|                   |* bidirezionale                                        |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE179|\      |Indicare una delle seguenti opzioni:                   |Testo |O      |
|                   |                                                       |      |       |
|                   |* aperta                                               |      |       |
|                   |                                                       |      |       |
|                   |* chiusa                                               |      |       |
|                   |                                                       |      |       |
|                   |* in costruzione                                       |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE180|\      |Ambito del percorso (es. stradale, fluviale, parco)    |Testo |O      |
+-------------------+-------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h4673596e42433c23372f496042157a48:

#12 Aree di sosta (DEFINITIVO)
------------------------------

\ |STYLE181|\ : Aree di sosta 

\ |STYLE182|\  Dataset geografico (Shapefile)

\ |STYLE183|\ : Tempestiva

Esempio: \ |LINK27|\  

+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                                                                                                                |Tipo |Obbligo|
+===================+===========================================================================================================================================+=====+=======+
|ID_Area            |Codice identificativo dell’area                                                                                                            |Testo|M      |
+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+
|\ |STYLE184|\      |Indicare la tipologia di area per soggetto interessato (es. disabili, sosta libera, bici, autobus, autocarri,ecc.) come da tabella seguente|Testo|M      |
+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+
|\ |STYLE185|\      |Via, Piazza, ecc                                                                                                                           |Testo|M      |
+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+
|\ |STYLE186|\      |Nome Via, Piazza, ecc.                                                                                                                     |Testo|M      |
+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+


+-----------------------------------------------------+-----+
|Tipo_Area                                            |Sigla|
+=====================================================+=====+
|Autorizzati                                          |A    |
+-----------------------------------------------------+-----+
|Azienda Sanitaria                                    |AS   |
+-----------------------------------------------------+-----+
|Autobus                                              |B    |
+-----------------------------------------------------+-----+
|Carabinieri                                          |CC   |
+-----------------------------------------------------+-----+
|Camera di Commercio Industria Artigianato Agricoltura|CCIAA|
+-----------------------------------------------------+-----+
|Clienti (privato)                                    |CL   |
+-----------------------------------------------------+-----+
|Condomini (privato)                                  |CN   |
+-----------------------------------------------------+-----+
|Croce Rossa Italiana                                 |CRI  |
+-----------------------------------------------------+-----+
|Car sharing                                          |CSh  |
+-----------------------------------------------------+-----+
|Divieto diurno                                       |DD   |
+-----------------------------------------------------+-----+
|Dipendenti (privato)                                 |DP   |
+-----------------------------------------------------+-----+
|Guardia di Finanza                                   |GF   |
+-----------------------------------------------------+-----+
|Disabili                                             |H    |
+-----------------------------------------------------+-----+
|Sosta libera                                         |L    |
+-----------------------------------------------------+-----+
|Bici motocicli ciclomotori                           |BM   |
+-----------------------------------------------------+-----+
|Carico                                               |CS   |
+-----------------------------------------------------+-----+
|Bici                                                 |Bici |
+-----------------------------------------------------+-----+
|Motocicli                                            |M    |
+-----------------------------------------------------+-----+
|Sosta a pagamento                                    |P    |
+-----------------------------------------------------+-----+
|Protezione Civile                                    |PC   |
+-----------------------------------------------------+-----+
|Polizia Locale                                       |PL   |
+-----------------------------------------------------+-----+
|Polizia di Stato                                     |PS   |
+-----------------------------------------------------+-----+
|Residenti                                            |R    |
+-----------------------------------------------------+-----+
|Sosta a tempo                                        |T    |
+-----------------------------------------------------+-----+
|Taxi                                                 |TAXI |
+-----------------------------------------------------+-----+

.. _h74377a1f30156255c70574b4a62b69:

#13 Aree pedonali (DEFINITIVO)
------------------------------

\ |STYLE187|\ : Aree pedonali

\ |STYLE188|\  Dataset geografico (Shapefile)

\ |STYLE189|\ : Tempestiva

Esempio: \ |LINK28|\  

+-------------------+-------------------------------+-----+-------+
|Denominazione Campo|Descrizione                    |Tipo |Obbligo|
+===================+===============================+=====+=======+
|ID_Area            |Codice identificativo dell’area|Testo|M      |
+-------------------+-------------------------------+-----+-------+
|\ |STYLE190|\      |Via, Piazza, ecc               |Testo|M      |
+-------------------+-------------------------------+-----+-------+
|\ |STYLE191|\      |Nome Via, Piazza, ecc.         |Testo|M      |
+-------------------+-------------------------------+-----+-------+

.. _h413751694948146ea793c3974582760:

#15 Bike sharing (DEFINITIVO)
-----------------------------

\ |STYLE192|\ : Postazioni di Bike sharing

\ |STYLE193|\  Dataset geografico (Shapefile)

\ |STYLE194|\ : Tempestiva

Esempio: \ |LINK29|\  

+-------------------+-------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                  |Tipo  |Obbligo|
+===================+=============================================================+======+=======+
|ID_Staz            |Codice identificativo della stazione di bike sharing         |Numero|M      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE195|\      |Per le informazioni di ubicazione vedere Allegato 1 Tabella 1|Testo |M      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE196|\      |Latitudine                                                   |Numero|M      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE197|\      |Longitudine                                                  |Numero|M      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE198|\      |Numero di biciclette disponibile per stazione                |Numero|O      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE199|\      |Ulteriore descrizione dell’area                              |Testo |O      |
+-------------------+-------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h781030632f513187a587241745959:

#31 Autoscuole (DEFINITIVO)
---------------------------

\ |STYLE200|\ : Elenco delle Autoscuole autorizzate nel territorio

\ |STYLE201|\  Dataset tabellare

\ |STYLE202|\ : Tempestiva

Esempio: \ |LINK30|\  

L’esempio si riferisce alla tipologia di informazioni da inserire nel dataset. Per quanto riguarda la suddivisione delle informazioni in campi, occorre fare riferimento alla tabella seguente. In particolare, per l’indirizzo occorre inserire tutti i campi previsti per l’ubicazione come indicati nell’Allegato 1 Tabella 1. 

+-------------------+---------------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                                    |Tipo |Obbligo|
+===================+===============================================================+=====+=======+
|Nome               |Nome dell’autoscuola                                           |Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE203|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE204|\      |Numero di telefono dell’autoscuola                             |Testo|O      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE205|\      |Indirizzo email dell’autoscuola                                |Testo|O      |
+-------------------+---------------------------------------------------------------+-----+-------+

.. _h2c1d74277104e41780968148427e:




.. _h29173c11c44516963343b7a352726b:

#33 Aree di sosta per disabili (DEFINITIVO)
-------------------------------------------

\ |STYLE206|\ : Elenco delle Aree di sosta per disabili presenti nel territorio

\ |STYLE207|\  Dataset tabellare

\ |STYLE208|\ : Tempestiva

Esempio: \ |LINK31|\  

+-------------------+---------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                    |Tipo  |Obbligo|
+===================+===============================================================+======+=======+
|ID_Area            |Codice identificativo dell’area                                |Testo |M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE209|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo |M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE210|\      |Numero stalli dell’area di sosta                               |Numero|M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE211|\      |Longitudine                                                    |Numero|O      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE212|\      |Latitudine                                                     |Numero|O      |
+-------------------+---------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h7f1d5c471796a7032617255597b173a:

#44 Punti di ricarica veicoli (DEFINITIVO)
------------------------------------------

\ |STYLE213|\ : Dataset con coordinate geografiche dei punti di ricarica dei veicoli elettrici, con indicazione del tipo di presa e KW

\ |STYLE214|\  Dataset tabellare

\ |STYLE215|\ : Tempestiva

Esempio: \ |LINK32|\  

+-------------------+--------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                     |Tipo  |Obbligo|
+===================+================================================================================+======+=======+
|ID_Sito            |Codice identificativo del sito in cui è possibile ricaricare i veicoli elettrici|Numero|O      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE216|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                 |Testo |M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE217|\      |Potenza della ricarica                                                          |Numero|M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE218|\      |Indicare la modalità di utilizzo del servizio (es. tramite CRS)                 |Testo |M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE219|\      |Indicare la tipologia di presa (es. universale)                                 |Testo |M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE220|\      |Indicare le tipologie di veicoli per le quali è disponibile la ricarica         |Testo |M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE221|\      |Data di attivazione del sito                                                    |Data  |O      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE222|\      |Longitudine                                                                     |Numero|M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE223|\      |Latitudine                                                                      |Numero|M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+

.. _h127c74681e53786e536b765a2f6647e:

6.       SICUREZZA
==================

.. _h824122d55a315e452768e7f292a6e:

#7 Incidenti stradali (DEFINITIVO)
----------------------------------

\ |STYLE224|\ : Dataset contenente gli incidenti stradali con data, ora, coordinate geografiche, mezzi coinvolti, eventuali morti e feriti

\ |STYLE225|\ : Dataset tabellare

\ |STYLE226|\ : Mensile

Esempio 1: \ |LINK33|\ 

Esempio 2: \ |LINK34|\  

+-------------------+----------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                       |Tipo  |Obbligo|
+===================+==================================================================================+======+=======+
|Anno               |Anno di riferimento                                                               |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE227|\      |Data dell’incidente                                                               |Data  |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE228|\      |Ora dell’incidente                                                                |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE229|\      |Descrizione del punto preciso dell’incidente (es. via...all’intersezione con via…)|Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE230|\      |Tipologia di incidente (es. scontro frontale)                                     |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE231|\      |Numero delle persone illese                                                       |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE232|\      |Numero delle persone ferite                                                       |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE233|\      |Numero dei morti                                                                  |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE234|\      |Indicare se sono stati coinvolti pedoni (SI/NO)                                   |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE235|\      |Indicare se sono stati coinvolti velocipedi (SI/NO)                               |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE236|\      |Indicare se sono stati coinvolti ciclomotori o motocicli (SI/NO)                  |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE237|\      |Indicare se sono stati coinvolti mezzi pesanti (SI/NO)                            |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE238|\      |Longitudine                                                                       |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE239|\      |Latitudine                                                                        |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h4760d266a547666543d45223781653:

#41  Principali infrazioni al Codice della Strada (DEFINITIVO)
--------------------------------------------------------------

\ |STYLE240|\ : Elenco, tipologia e anno di riferimento delle principali infrazioni al Codice della Strada.

\ |STYLE241|\  Dataset tabellare

\ |STYLE242|\ : Mensile

Esempio: \ |LINK35|\ 

+-------------------+--------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                         |Tipo  |Obbligo|
+===================+====================================================================+======+=======+
|Anno               |Anno di riferimento                                                 |Numero|M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE243|\      |Tipo di infrazione (es. limite velocità, sensi unici, sosta, ecc.)  |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE244|\      |Normativa di riferimento dell’infrazione (es. Legge)                |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE245|\      |Art. di legge o altra norma che regola il tipo di infrazione        |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE246|\      |Data infrazione                                                     |Data  |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE247|\      |Tipologia di veicolo: autovettura, motoveicolo, ciclomotore         |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE248|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1     |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE249|\      |Inserire il numero delle sanzioni erogate per l’infrazione specifica|Numero|M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE250|\      |Longitudine                                                         |Numero|O      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE251|\      |Latitudine                                                          |Numero|O      |
+-------------------+--------------------------------------------------------------------+------+-------+

.. _h6f396320344978474c3f7b4d6b7e531c:

#42 Provvedimenti adottati dalla Polizia Locale in materia di commercio (DEFINITIVO)
------------------------------------------------------------------------------------

\ |STYLE252|\ : Elenco e tipologia dei provvedimenti adottati in materia di commercio dalla Polizia Municipale

\ |STYLE253|\  Dataset tabellare

\ |STYLE254|\ : Mensile

Esempio: \ |LINK36|\  

+-------------------+---------------------+------+-------+
|Denominazione Campo|Descrizione          |Tipo  |Obbligo|
+===================+=====================+======+=======+
|Anno               |Anno di riferimento  |Numero|M      |
+-------------------+---------------------+------+-------+
|\ |STYLE255|\      |Tipo di provvedimento|Testo |M      |
+-------------------+---------------------+------+-------+
|\ |STYLE256|\      |Numero di controlli  |Numero|M      |
+-------------------+---------------------+------+-------+
|\ |STYLE257|\      |Numero di verbali    |Numero|M      |
+-------------------+---------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h04573713141737316103050642c523f:

#49 Controlli in cantiere effettuati dalla Polizia Locale (DEFINITIVO)
----------------------------------------------------------------------

\ |STYLE258|\ : Elenco, tipologia e anno di riferimento dei controlli effettuati nei cantieri dalla Polizia locale

\ |STYLE259|\  Dataset tabellare

\ |STYLE260|\ : Mensile

+-------------------+----------------------+------+-------+
|Denominazione Campo|Descrizione           |Tipo  |Obbligo|
+===================+======================+======+=======+
|Anno               |Anno di riferimento   |Numero|M      |
+-------------------+----------------------+------+-------+
|\ |STYLE261|\      |Tipologia di controllo|Testo |M      |
+-------------------+----------------------+------+-------+
|\ |STYLE262|\      |Numero di controlli   |Numero|M      |
+-------------------+----------------------+------+-------+
|\ |STYLE263|\      |Numero di verbali     |Numero|M      |
+-------------------+----------------------+------+-------+

.. _h6a50711f57485b63626e405f165261:

7.      STATISTICA
==================

Per quanto riguarda i risultati delle elezioni, in seguito ad un’analisi ulteriore è stata individuata una soluzione alternativa alla pubblicazione dei 3 dataset distinti (#38, #39 e #40): pubblicare un unico dataset che comprenda sia i risultati delle elezioni sia i dati statistici sull’affluenza (vedere tabella #38#39#40BIS Risultati elezioni). Questo consentirebbe di mantenere sempre uguale la struttura del dataset (campi) rendendo più facilmente confrontabili i dati. 

Ai fini del co-finanziamento, la pubblicazione del dataset #38#39#40BIS viene equiparata alla pubblicazione dei 3 dataset relativi alle elezioni (#38 + #39 + #40). 

.. _h47274b145479547445336f771b35280:

#38 Risultati elezioni comunali (DEFINITIVO)
--------------------------------------------

\ |STYLE264|\ : Risultati elettorali delle elezioni amministrative del proprio comune o provincia

\ |STYLE265|\  Dataset tabellare

\ |STYLE266|\ : Tempestiva

+-------------------+-----------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                        |Tipo  |Obbligo|
+===================+===================================================================================+======+=======+
|Data               |Data elezione (giorno, mese, anno)                                                 |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE267|\      |Indicare se si tratta di:                                                          |Testo |M      |
|                   |                                                                                   |      |       |
|                   |* 1° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* 2° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* turno unico                                                                      |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE268|\      |Collegio elettorale o circoscrizione                                               |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE269|\      |Numero della sezione                                                               |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE270|\      |Consiglio comunale o Sindaco                                                       |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE271|\      |Inserire in questa colonna una riga per ciascuna delle seguenti informazioni:      |Testo |M      |
|                   |                                                                                   |      |       |
|                   |* Nome della lista o del singolo candidato (es. nel caso dell’elezione del sindaco)|      |       |
|                   |                                                                                   |      |       |
|                   |* Schede valide                                                                    |      |       |
|                   |                                                                                   |      |       |
|                   |* Schede nulle                                                                     |      |       |
|                   |                                                                                   |      |       |
|                   |* Schede bianche                                                                   |      |       |
|                   |                                                                                   |      |       |
|                   |* Schede contestate                                                                |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale elettori (totale aventi diritto iscritti alla sezione)                    |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale elettori maschi                                                           |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale elettori femmine                                                          |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale votanti                                                                   |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale votanti maschi                                                            |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale votanti femmine                                                           |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE272|\      |Inserire una riga per ciascuna delle seguenti informazioni:                        |Numero|M      |
|                   |                                                                                   |      |       |
|                   |* N. voti ottenuti dalla lista o dal singolo candidato (voti validi)               |      |       |
|                   |                                                                                   |      |       |
|                   |* N. schede valide                                                                 |      |       |
|                   |                                                                                   |      |       |
|                   |* N. schede nulle                                                                  |      |       |
|                   |                                                                                   |      |       |
|                   |* N. schede bianche                                                                |      |       |
|                   |                                                                                   |      |       |
|                   |* N. schede contestate                                                             |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale elettori (totale aventi diritto iscritti alla sezione)                 |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale elettori maschi                                                        |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale elettori femmine                                                       |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale votanti                                                                |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale votanti maschi                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale votanti femmine                                                        |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h6e64461642c1b5e501d5d104b713c1d:

#39 Risultati elezioni regionali (DEFINITIVO)
---------------------------------------------

\ |STYLE273|\ : Risultati elettorali delle elezioni regionali nel proprio comune o provincia

\ |STYLE274|\  Dataset tabellare

\ |STYLE275|\ : Tempestiva

+-------------------+-----------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                        |Tipo  |Obbligo|
+===================+===================================================================================+======+=======+
|Data               |Data elezione (giorno, mese, anno)                                                 |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE276|\      |Indicare se si tratta di:                                                          |Testo |M      |
|                   |                                                                                   |      |       |
|                   |* 1° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* 2° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* turno unico                                                                      |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE277|\      |Collegio elettorale o circoscrizione                                               |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE278|\      |Numero della sezione                                                               |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE279|\      |Consiglio regionale o Presidente della Regione                                     |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE280|\      |Inserire in questa colonna una riga per ciascuna delle seguenti informazioni:      |Testo |M      |
|                   |                                                                                   |      |       |
|                   |* Nome della lista o del singolo candidato (es. nel caso dell’elezione del sindaco)|      |       |
|                   |                                                                                   |      |       |
|                   |* Schede valide                                                                    |      |       |
|                   |                                                                                   |      |       |
|                   |* Schede nulle                                                                     |      |       |
|                   |                                                                                   |      |       |
|                   |* Schede bianche                                                                   |      |       |
|                   |                                                                                   |      |       |
|                   |* Schede contestate                                                                |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale elettori (totale aventi diritto iscritti alla sezione)                    |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale elettori maschi                                                           |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale elettori femmine                                                          |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale votanti                                                                   |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale votanti maschi                                                            |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale votanti femmine                                                           |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE281|\      |Inserire una riga per ciascuna delle seguenti informazioni:                        |Numero|M      |
|                   |                                                                                   |      |       |
|                   |* N. voti ottenuti dalla lista o dal singolo candidato (voti validi)               |      |       |
|                   |                                                                                   |      |       |
|                   |* N. schede valide                                                                 |      |       |
|                   |                                                                                   |      |       |
|                   |* N. schede nulle                                                                  |      |       |
|                   |                                                                                   |      |       |
|                   |* N. schede bianche                                                                |      |       |
|                   |                                                                                   |      |       |
|                   |* N. schede contestate                                                             |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale elettori (totale aventi diritto iscritti alla sezione)                 |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale elettori maschi                                                        |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale elettori femmine                                                       |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale votanti                                                                |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale votanti maschi                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale votanti femmine                                                        |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+

.. _h61f79121f287221467271742a444f:

#40 Risultati elezioni nazionali (DEFINITIVO)
---------------------------------------------

\ |STYLE282|\ : Risultati elettorali delle elezioni nazionali nel proprio comune o provincia

\ |STYLE283|\  Dataset tabellare

\ |STYLE284|\ : Tempestiva

+-------------------+-----------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                        |Tipo  |Obbligo|
+===================+===================================================================================+======+=======+
|Data               |Data elezione (giorno, mese, anno)                                                 |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE285|\      |Indicare se si tratta di:                                                          |Testo |M      |
|                   |                                                                                   |      |       |
|                   |* 1° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* 2° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* turno unico                                                                      |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE286|\      |Collegio elettorale o circoscrizione                                               |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE287|\      |Numero della sezione                                                               |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE288|\      |Camera dei deputati o Senato della Repubblica                                      |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE289|\      |Inserire in questa colonna una riga per ciascuna delle seguenti informazioni:      |Testo |M      |
|                   |                                                                                   |      |       |
|                   |* Nome della lista o del singolo candidato (es. nel caso dell’elezione del sindaco)|      |       |
|                   |                                                                                   |      |       |
|                   |* Schede valide                                                                    |      |       |
|                   |                                                                                   |      |       |
|                   |* Schede nulle                                                                     |      |       |
|                   |                                                                                   |      |       |
|                   |* Schede bianche                                                                   |      |       |
|                   |                                                                                   |      |       |
|                   |* Schede contestate                                                                |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale elettori (totale aventi diritto iscritti alla sezione)                    |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale elettori maschi                                                           |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale elettori femmine                                                          |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale votanti                                                                   |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale votanti maschi                                                            |      |       |
|                   |                                                                                   |      |       |
|                   |* Totale votanti femmine                                                           |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE290|\      |Inserire una riga per ciascuna delle seguenti informazioni:                        |Numero|M      |
|                   |                                                                                   |      |       |
|                   |* N. voti ottenuti dalla lista o dal singolo candidato (voti validi)               |      |       |
|                   |                                                                                   |      |       |
|                   |* N. schede valide                                                                 |      |       |
|                   |                                                                                   |      |       |
|                   |* N. schede nulle                                                                  |      |       |
|                   |                                                                                   |      |       |
|                   |* N. schede bianche                                                                |      |       |
|                   |                                                                                   |      |       |
|                   |* N. schede contestate                                                             |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale elettori (totale aventi diritto iscritti alla sezione)                 |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale elettori maschi                                                        |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale elettori femmine                                                       |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale votanti                                                                |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale votanti maschi                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* N. Totale votanti femmine                                                        |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+

.. _h36154c2b39757647157f5b44c6a313:

#38#39#40BIS Risultati elezioni (DEFINITIVO)
--------------------------------------------

\ |STYLE291|\ : Risultati elettorali e dati sull’affluenza 

\ |STYLE292|\  Dataset tabellare

\ |STYLE293|\ : Tempestiva

+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                                                                                                                                                |Tipo  |Obbligo|
+===================+===========================================================================================================================================================================================================================================================+======+=======+
|Data               |Data elezione (giorno, mese, anno)                                                                                                                                                                                                                         |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE294|\      |In caso di più tornate elettorali, specificare il turno o indicare se turno unico (1° turno, 2° turno, turno unico)                                                                                                                                        |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE295|\      |Tipologia di elezione (es. Camera, Senato, Comunali, Circoscrizionali, Provinciali, Regionali, Europee, Referendum 1, Referendum 2, ecc.)                                                                                                                  |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE296|\      |Es. Camera dei Deputati, Senato della Repubblica, Consiglio comunale, Sindaco, Consiglio provinciale, Presidente della Provincia, Consiglio regionale, Presidente della Regione, Parlamento europeo, oppure l’oggetto del referendum (es. energia nucleare)|Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE297|\      |Collegio elettorale o Circoscrizione                                                                                                                                                                                                                       |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE298|\      |Numero della sezione                                                                                                                                                                                                                                       |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE299|\      |Inserire in questa colonna una riga per ciascuna delle seguenti informazioni:                                                                                                                                                                              |Testo |M      |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* Nome della lista o del singolo candidato (es. nel caso dell’elezione del sindaco)                                                                                                                                                                        |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* Schede valide                                                                                                                                                                                                                                            |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* Schede nulle                                                                                                                                                                                                                                             |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* Schede bianche                                                                                                                                                                                                                                           |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* Schede contestate                                                                                                                                                                                                                                        |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* Totale elettori (totale aventi diritto iscritti alla sezione)                                                                                                                                                                                            |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* Totale elettori maschi                                                                                                                                                                                                                                   |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* Totale elettori femmine                                                                                                                                                                                                                                  |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* Totale votanti                                                                                                                                                                                                                                           |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* Totale votanti maschi                                                                                                                                                                                                                                    |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* Totale votanti femmine                                                                                                                                                                                                                                   |      |       |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE300|\      |Inserire una riga per ciascuna delle seguenti informazioni:                                                                                                                                                                                                |Numero|M      |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* N. voti ottenuti dalla lista o dal singolo candidato (voti validi)                                                                                                                                                                                       |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* N. schede valide                                                                                                                                                                                                                                         |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* N. schede nulle                                                                                                                                                                                                                                          |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* N. schede bianche                                                                                                                                                                                                                                        |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* N. schede contestate                                                                                                                                                                                                                                     |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* N. Totale elettori (totale aventi diritto iscritti alla sezione)                                                                                                                                                                                         |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* N. Totale elettori maschi                                                                                                                                                                                                                                |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* N. Totale elettori femmine                                                                                                                                                                                                                               |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* N. Totale votanti                                                                                                                                                                                                                                        |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* N. Totale votanti maschi                                                                                                                                                                                                                                 |      |       |
|                   |                                                                                                                                                                                                                                                           |      |       |
|                   |* N. Totale votanti femmine                                                                                                                                                                                                                                |      |       |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h492e3345c6f1555f5b19363179137c:

#46 Condizione lavorativa (DEFINITIVO)
--------------------------------------

\ |STYLE301|\ : Informazioni sulla condizione lavorativa dei residenti (ad esempio occupato, in cerca di occupazione ecc.)

\ |STYLE302|\  Dataset tabellare

\ |STYLE303|\ : Trimestrale

Esempio: \ |LINK37|\  

+-------------------+-------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                              |Tipo  |Obbligo|
+===================+=========================================================================+======+=======+
|Anno               |Anno di riferimento                                                      |Numero|M      |
+-------------------+-------------------------------------------------------------------------+------+-------+
|\ |STYLE304|\      |Condizione lavorativa (ad esempio occupato, in cerca di occupazione ecc.)|Testo |M      |
+-------------------+-------------------------------------------------------------------------+------+-------+
|\ |STYLE305|\      |Numero di maschi                                                         |Numero|M      |
+-------------------+-------------------------------------------------------------------------+------+-------+
|\ |STYLE306|\      |Numero di femmine                                                        |Numero|M      |
+-------------------+-------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h47325942212741500d25226c3727f:

8.      TERRITORIO
==================

.. _h784465346686a592127d1e14157730:

#4 Rete viaria - Dataset geografico (DEFINITIVO)
------------------------------------------------

\ |STYLE307|\ : Rete viaria 

\ |STYLE308|\  Dataset geografico (Shapefile)

\ |STYLE309|\ : Tempestiva

+-------------------+------------------------+-----+-------+
|Denominazione Campo|Descrizione             |Tipo |Obbligo|
+===================+========================+=====+=======+
|Toponimo           |Toponimo della strada   |Testo|M      |
+-------------------+------------------------+-----+-------+
|\ |STYLE310|\      |Nome del toponimo       |Testo|M      |
+-------------------+------------------------+-----+-------+
|\ |STYLE311|\      |Località                |Testo|M      |
+-------------------+------------------------+-----+-------+
|\ |STYLE312|\      |Senso di marcia (U/D/A):|Testo|M      |
|                   |                        |     |       |
|                   |* U - Unico             |     |       |
|                   |                        |     |       |
|                   |* D - Doppio            |     |       |
|                   |                        |     |       |
|                   |* A - Alternato         |     |       |
+-------------------+------------------------+-----+-------+
|\ |STYLE313|\      |Primo numero civico     |Testo|M      |
+-------------------+------------------------+-----+-------+
|\ |STYLE314|\      |Ultimo numero civico    |Testo|M      |
+-------------------+------------------------+-----+-------+

.. _h5457273b5f6970146f702b17c7f3550:

#5 Rete viaria - Toponimi stradali (DEFINITIVO)
-----------------------------------------------

\ |STYLE315|\ : Elenco Toponimi stradali

\ |STYLE316|\  Dataset tabellare

\ |STYLE317|\ : Tempestiva

Esempio: \ |LINK38|\  

+-------------------+----------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                               |Tipo |Obbligo|
+===================+==========================================================+=====+=======+
|Classe_Toponimo    |Indicare la classe toponimo (es. Via, Piazza, Largo, ecc.)|Testo|M      |
+-------------------+----------------------------------------------------------+-----+-------+
|\ |STYLE318|\      |Nome di Via, Piazza, Largo, ecc.                          |Testo|M      |
+-------------------+----------------------------------------------------------+-----+-------+
|\ |STYLE319|\      |Codice del toponimo                                       |Testo|M      |
+-------------------+----------------------------------------------------------+-----+-------+
|\ |STYLE320|\      |Inserire se si tratta di un dato storico (SI/NO)          |Testo|M      |
+-------------------+----------------------------------------------------------+-----+-------+

.. _h2c1d74277104e41780968148427e:




.. _h563b1f5f11515e35374069365613121:

#6 Rete viaria - Numeri civici (DEFINITIVO)
-------------------------------------------

\ |STYLE321|\ : Numeri civici georeferenziati

\ |STYLE322|\  Dataset tabellare

\ |STYLE323|\ : Tempestiva

Esempio: https://www.dati.lombardia.it/Territorio/Comune-Bergamo-Numerazione-civica/pcif-9jj7

+-------------------+------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                           |Tipo  |Obbligo|
+===================+======================================================+======+=======+
|Classe_Toponimo    |Indicare la classe toponimo (Via, Piazza, Largo, ecc.)|Testo |M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE324|\      |Nome di Via, Piazza, Largo, ecc.                      |Testo |M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE325|\      |Numero del civico                                     |Numero|M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE326|\      |Componente alfabetica del civico (es. A, Bis, ecc.)   |Testo |M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE327|\      |CAP                                                   |Numero|M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE328|\      |Sezione di censimento ISTAT                           |Numero|O      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE329|\      |Longitudine                                           |Numero|M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE330|\      |Latitudine                                            |Numero|M      |
+-------------------+------------------------------------------------------+------+-------+

.. _h32623c3510287d7f3af50466d4e60:

#14      Cantieri stradali (DEFINITIVO)
---------------------------------------

\ |STYLE331|\ : Cantieri stradali attivi 

\ |STYLE332|\  Dataset geografico (Shapefile)

\ |STYLE333|\ : Tempestiva


+-------------------+--------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                 |Tipo |Obbligo|
+===================+============================================+=====+=======+
|Toponimo           |Via, Piazza, ecc.                           |Testo|M      |
+-------------------+--------------------------------------------+-----+-------+
|\ |STYLE334|\      |Nome della via, piazza, ecc.                |Testo|M      |
+-------------------+--------------------------------------------+-----+-------+
|\ |STYLE335|\      |Breve descrizione dei lavori in svolgimento |Testo|M      |
+-------------------+--------------------------------------------+-----+-------+
|\ |STYLE336|\      |Data di inizio lavoro                       |Data |M      |
+-------------------+--------------------------------------------+-----+-------+
|\ |STYLE337|\      |Data prevista di fine lavoro                |Data |M      |
+-------------------+--------------------------------------------+-----+-------+

.. _h2c1d74277104e41780968148427e:




.. _h1a736c403f6676679673a673f60363a:

#16 HotSpot Wifi (DEFINITIVO)
-----------------------------

\ |STYLE338|\ : Elenco hotspot wifi pubblici, georeferenziati o dataset geografico

\ |STYLE339|\  Dataset tabellare

\ |STYLE340|\ : Tempestiva

Esempio: \ |LINK39|\  

+-------------------+--------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                           |Tipo  |Obbligo|
+===================+======================================================================================+======+=======+
|Rete               |Nome della rete (SSID)                                                                |Testo |O      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE341|\      |Codice identificativo del punto di accesso (singolo HotSpot Wifi) attribuito dall’ente|Testo |M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE342|\      |Indicare la tipologia del punto di accesso (HotSpot/Dispositivo estensione)           |Testo |O      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE343|\      |Nome del sito dove si trova il punto di accesso (es. denominazione Biblioteca…)       |Testo |M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE344|\      |Punto di accesso attivo (si, no)                                                      |Testo |M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE345|\      |Codice accesso                                                                        |Testo |O      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE346|\      |Longitudine                                                                           |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE347|\      |Latitudine                                                                            |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE348|\      |Indicare il raggio di copertura in metri                                              |Numero|O      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+

 

.. _h5a2161623f35403f62b4f305243726a:

#19 Area per sgambatura cani (DEFINITIVO)
-----------------------------------------

\ |STYLE349|\ : Mappa aree per sgambatura cani

\ |STYLE350|\  Dataset geografico (Shapefile)

\ |STYLE351|\ : Tempestiva

+-------------------+----------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                     |Tipo  |Obbligo|
+===================+================================================================+======+=======+
|ID_Area            |Codice identificativo dell’area                                 |Numero|M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE352|\      |Comune in cui è ubicata l’area                                  |Testo |M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE353|\      |Via, Piazza, ecc.                                               |Testo |M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE354|\      |Nome della via, piazza, ecc.                                    |Testo |M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE355|\      |Indicare la superficie dell’area (mq)                           |Numero|M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE356|\      |Indicare se sono presenti fontanelle (SI/NO)                    |Testo |O      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE357|\      |Indicare se sono presenti attrezzature per addestramento (SI/NO)|Testo |O      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE358|\      |Indicare se sono presenti panchine(SI/NO)                       |Testo |O      |
+-------------------+----------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2ca5320503f5437a26b171269386a:

#21 Pratiche edilizie (DEFINITIVO) 
-----------------------------------

\ |STYLE359|\ : Elenco Pratiche edilizie gestite dallo Sportello Unico per l’Edilizia

\ |STYLE360|\  Dataset tabellare

\ |STYLE361|\ : Mensile

Esempio: \ |LINK40|\  

+-------------------+--------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                             |Tipo  |Obbligo|
+===================+========================================================+======+=======+
|Anno               |Anno di riferimento                                     |Numero|M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE362|\      |Tipologia istanza (es. SCIA, PDC, ecc.)                 |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE363|\      |Codice identificativo dell’istanza                      |Testo |O      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE364|\      |Data di presentazione dell’istanza                      |Data  |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE365|\      |Numero di protocollo dell’istanza                       |Numero|O      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE366|\      |Numero del provvedimento (nel caso di PDC)              |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE367|\      |Data del provvedimento (nel caso di PDC)                |Data  |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE368|\      |Nominativo o Ragione sociale dell’istante \ |STYLE369|\ |Testo |O      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE370|\      |Descrizione dell’intervento oggetto dell’istanza        |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE371|\      |Codice ecografico del fabbricato                        |Testo |O      |
+-------------------+--------------------------------------------------------+------+-------+

\* Ciascun ente valuta la pubblicazione del dato in base al principio del bilanciamento tra l’interesse pubblico a conoscere dati, informazioni e documenti per tutelare i diritti dei cittadini e l’interesse pubblico alla tutela dei diritti delle persone e delle organizzazioni private che potrebbero essere lesi dalla disponibilità di dati, informazioni e documenti.

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h752c462f6e4e4179353571873311521:

#22 Elenco beni confiscati (DEFINITIVO) 
----------------------------------------

\ |STYLE372|\ : Elenco beni confiscati alla mafia e assegnati al comune

\ |STYLE373|\  Dataset tabellare

\ |STYLE374|\ : Mensile

+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                              |Tipo  |Obbligo|
+===================+=========================================================================================+======+=======+
|ID_Bene            |Codice identificativo del bene confiscato                                                |Testo |O      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE375|\      |Tipologia del bene confiscato (es. appartamento, villa, ecc.)                            |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE376|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                          |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE377|\      |Superficie del bene confiscato (mq)                                                      |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE378|\      |Nominativo o ragione sociale dell’assegnatario del bene                                  |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE379|\      |Breve descrizione del progetto in funzione del quale il bene confiscato è stato assegnato|Testo |O      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE380|\      |Destinazione d’uso del bene confiscato                                                   |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE381|\      |Riferimenti all’atto di concessione                                                      |Testo |O      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE382|\      |Data dell’atto di concessione                                                            |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE383|\      |Numero di anni della concessione                                                         |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h1534f311220496307c39787c131e20:

#29 Centri revisione auto (DEFINITIVO)
--------------------------------------

\ |STYLE384|\ : Centri revisione auto autorizzati dalla Provincia

\ |STYLE385|\  Dataset tabellare

\ |STYLE386|\ : Tempestiva

Esempio: \ |LINK41|\ 


+-------------------+---------------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                                    |Tipo |Obbligo|
+===================+===============================================================+=====+=======+
|Nome               |Nome del centro di revisione                                   |Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE387|\      |Tipologia di revisione (es. auto, moto, ecc.)                  |Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE388|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE389|\      |Numero di telefono del centro di revisione                     |Testo|O      |
+-------------------+---------------------------------------------------------------+-----+-------+

.. _h5e126927772356f4b3651622c12502f:

9.  TRASPARENZA 
================

.. _h6a113f1a7b5a1f2e7d29274624462967:

#2 Contributi e sussidi (DEFINITIVO)
------------------------------------

\ |STYLE390|\ : Dati relativi agli atti di concessione di sovvenzioni, contributi, sussidi ed ausili finanziari alle imprese e comunque di vantaggi economici di qualunque genere a persone ed enti pubblici e privati

\ |STYLE391|\  Dataset tabellare

\ |STYLE392|\ : Tempestiva

Obblighi normativi: D. lgs. 33/2013, in particolare artt. 26-27.

Vedi \ |LINK42|\  (FAQ N. 13) 


+-------------------+-------------------------------------------------------------------------------+-------+-------+
|Denominazione Campo|Descrizione                                                                    |Tipo   |Obbligo|
+===================+===============================================================================+=======+=======+
|Anno               |Anno di riferimento                                                            |Numero |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE393|\      |Codice identificativo del provvedimento                                        |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE394|\      |Data del provvedimento                                                         |Data   |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE395|\      |Nominativo o Ragione sociale del soggetto beneficiario del provvedimento       |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE396|\      |Indicare se si tratta di amministrazione pubblica, privato, Onlus o altro ente |Testo  |O      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE397|\      |Codice fiscale del soggetto beneficiario del provvedimento                     |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE398|\      |Partita IVA del soggetto beneficiario del provvedimento                        |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE399|\      |Oggetto del provvedimento                                                      |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE400|\      |Riferimenti della norma o titolo a base dell’attribuzione                      |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE401|\      |URL norma o titolo                                                             |Web URL|O      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE402|\      |Ufficio responsabile del provvedimento.                                        |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE403|\      |Cognome del responsabile del procedimento                                      |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE404|\      |Nome del responsabile del procedimento                                         |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE405|\      |Modalità di individuazione del soggetto beneficiario (es. aggiudicazione bando)|Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE406|\      |Importo del vantaggio economico corrisposto                                    |Numero |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE407|\      |Breve descrizione progetto allegato al provvedimento                           |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE408|\      |URL progetto                                                                   |Web URL|O      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE409|\      |Link al curriculum del soggetto beneficiario                                   |Web URL|O      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+

.. _h7782e36e316052235761422844d44:

#23 Elenco canoni di locazione (DEFINITIVO)
-------------------------------------------

\ |STYLE410|\ : Elenco canoni di locazione o di affitto percepiti

\ |STYLE411|\  Dataset tabellare

\ |STYLE412|\ : Mensile

Obblighi normativi: D. lgs. 33/2013, in particolare art. 30.

+-------------------+---------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                            |Tipo  |Obbligo|
+===================+=======================================================================================+======+=======+
|Anno               |Anno di riferimento                                                                    |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE413|\      |Indicare la tipologia di locazione (Attiva/Passiva)                                    |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE414|\      |Nominativo o Ragione sociale del locatario                                             |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE415|\      |Nominativo o Ragione sociale del locatore                                              |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE416|\      |Per le informazioni relative all’ubicazione dell’immobile vedere Allegato 1 - Tabella 1|Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE417|\      |Destinazione dell’immobile (es. uffici)                                                |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE418|\      |Data di decorrenza del contratto                                                       |Data  |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE419|\      |Data di scadenza del contratto                                                         |Data  |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE420|\      |Canone annuale di affitto percepito al netto delle spese                               |Numero|M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE421|\      |Altre spese non inserite nel canone annuale                                            |Numero|M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE422|\      |Canone annuale di affitto versato                                                      |Numero|M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h6326371021e1b65335f1b3a15d202c:

#24 Elenco immobili di proprietà (DEFINITIVO)
---------------------------------------------

\ |STYLE423|\ : Elenco informazioni identificative degli immobili posseduti

\ |STYLE424|\  Dataset tabellare

\ |STYLE425|\ : Mensile

Obblighi normativi: D. lgs. 33/2013, in particolare art. 30.

+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                         |Tipo  |Obbligo|
+===================+====================================================================================================+======+=======+
|Ubicazione         |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                                     |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE426|\      |Denominazione dell’unità immobiliare (es. Palazzo Pirelli) o descrizione area (es. area industriale)|Testo |O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE427|\      |Indicare la natura giuridica del bene patrimoniale tra:                                             |Testo |M      |
|                   |                                                                                                    |      |       |
|                   |* disponibile                                                                                       |      |       |
|                   |                                                                                                    |      |       |
|                   |* indisponibile                                                                                     |      |       |
|                   |                                                                                                    |      |       |
|                   |* demaniale                                                                                         |      |       |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE428|\      |es. Immobile                                                                                        |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE429|\      |Codice identificativo categoria (dato catastale).                                                   |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE430|\      |Sezione (dato catastale)                                                                            |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE431|\      |Codice identificativo foglio (dato catastale)                                                       |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE432|\      |Codice identificativo mappale (dato catastale)                                                      |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE433|\      |Codice identificativo subalterno (dato catastale)                                                   |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE434|\      |Classe_catastale                                                                                    |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE435|\      |Unità di misura della consistenza (mq, mc, vani)                                                    |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE436|\      |Grandezza del bene (solo numero riferito all’unità di misura del campo precedente)                  |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE437|\      |Rendita catastale                                                                                   |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE438|\      |Destinazione d’uso del bene                                                                         |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE439|\      |Superficie del bene (espressa in metri quadrati).                                                   |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE440|\      |Valore di mercato del bene                                                                          |Numero|O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE441|\      |Data di acquisizione del bene                                                                       |Data  |O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE442|\      |Longitudine                                                                                         |Numero|O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE443|\      |Latitudine                                                                                          |Numero|O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+

.. _h4451d524d372a6ed467c1876264f6d:

#25 Monitoraggio procedimenti (DEFINITIVO) 
-------------------------------------------

\ |STYLE444|\ : Monitoraggio dei tempi dei procedimenti

\ |STYLE445|\  Dataset tabellare

\ |STYLE446|\ : Semestrale

+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                  |Tipo  |Obbligo|
+===================+=============================================================================================+======+=======+
|Tipologia          |Tipologia del procedimento (d’ufficio o a istanza di parte)                                  |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE447|\      |Nome del procedimento                                                                        |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE448|\      |Breve descrizione del procedimento                                                           |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE449|\      |Indicare il termine massimo di conclusione del procedimento stabilito dalla legge (in giorni)|Numero|M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE450|\      |Indicare il termine effettivo di conclusione del procedimento (in giorni)                    |Numero|M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE451|\      |Ufficio responsabile del provvedimento                                                       |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE452|\      |Indicare motivi di eventuali sospensioni o ritardi                                           |Testo |O      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h132c4945185112631f3367485d57c16:

#26 Enti controllati – Società partecipate (DEFINITIVO)
-------------------------------------------------------

\ |STYLE453|\ : Elenco e informazioni sulle Società partecipate

\ |STYLE454|\  Dataset tabellare

\ |STYLE455|\ : Tempestiva

+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo            |Descrizione                                                                                       |Tipo  |Obbligo|
+===============================+==================================================================================================+======+=======+
|Ente_pubblico – Ragione_Sociale|Denominazione ente                                                                                |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE456|\                  |Funzioni affidate all’Ente                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE457|\                  |.Attività svolte dall’Ente per ottemperare alle funzioni                                          |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE458|\                  |Eventuale quota di partecipazione societaria all’ente                                             |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE459|\                  |“Indeterminato” oppure scadenza prevista                                                          |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE460|\                  |Onere complessivo a qualsiasi titolo gravante per l'anno sul bilancio dell'amministrazione        |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE461|\                  |Numero dei rappresentanti dell'amministrazione negli organi di governo                            |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE462|\                  |Trattamento economico complessivo dei rappresentanti dell'amministrazione negli organi di governo |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE463|\                  |Anno di riferimento                                                                               |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE464|\                  |Risultati di bilancio dell’anno di riferimento (ultimo anno)                                      |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE465|\                  |Risultati di bilancio del penultimo anno                                                          |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE466|\                  |Risultati di bilancio del terzultimo anno                                                         |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE467|\                  |Link al sito istituzionale                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+

.. _h7239514f337e4b15371432716b161761:

#27 Enti controllati – Enti pubblici vigilati (DEFINITIVO)
----------------------------------------------------------

\ |STYLE468|\ : Elenco e informazioni sugli Enti pubblici vigilati

\ |STYLE469|\  Dataset tabellare

\ |STYLE470|\ : Tempestiva

+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo            |Descrizione                                                                                       |Tipo  |Obbligo|
+===============================+==================================================================================================+======+=======+
|Ente_pubblico – Ragione_Sociale|Denominazione ente                                                                                |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE471|\                  |Funzioni affidate all’Ente                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE472|\                  |Attività svolte dall’Ente per ottemperare alle funzioni                                           |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE473|\                  |Eventuale quota di partecipazione societaria all’ente                                             |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE474|\                  |“Indeterminato” oppure scadenza prevista                                                          |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE475|\                  |Onere complessivo a qualsiasi titolo gravante per l'anno sul bilancio dell'amministrazione        |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE476|\                  |Numero dei rappresentanti dell'amministrazione negli organi di governo                            |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE477|\                  |Trattamento economico complessivo dei rappresentanti dell'amministrazione negli organi di governo |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE478|\                  |Anno di riferimento                                                                               |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE479|\                  |Risultati di bilancio dell’anno di riferimento (ultimo anno)                                      |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE480|\                  |Risultati di bilancio del penultimo anno                                                          |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE481|\                  |Risultati di bilancio del terzultimo anno                                                         |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE482|\                  |Link al sito istituzionale                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h6057240426a371f372442d4776d7f:

#28 Enti controllati – Enti di diritto privato controllati (DEFINITIVO)
-----------------------------------------------------------------------

\ |STYLE483|\ : Elenco e informazioni sugli Enti di diritto privato controllati

\ |STYLE484|\  Dataset tabellare

\ |STYLE485|\ : Tempestiva

+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo            |Descrizione                                                                                       |Tipo  |Obbligo|
+===============================+==================================================================================================+======+=======+
|Ente_pubblico – Ragione_Sociale|Denominazione ente                                                                                |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE486|\                  |Funzioni affidate all’Ente                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE487|\                  |.Attività svolte dall’Ente per ottemperare alle funzioni                                          |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE488|\                  |Eventuale quota di partecipazione societaria all’ente                                             |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE489|\                  |“Indeterminato” oppure scadenza prevista                                                          |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE490|\                  |Onere complessivo a qualsiasi titolo gravante per l'anno sul bilancio dell'amministrazione        |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE491|\                  |Numero dei rappresentanti dell'amministrazione negli organi di governo                            |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE492|\                  |Trattamento economico complessivo dei rappresentanti dell'amministrazione negli organi di governo |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE493|\                  |Anno di riferimento                                                                               |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE494|\                  |Risultati di bilancio dell’anno di riferimento (ultimo anno)                                      |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE495|\                  |Risultati di bilancio del penultimo anno                                                          |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE496|\                  |Risultati di bilancio del terzultimo anno                                                         |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE497|\                  |Link al sito istituzionale                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+

.. _h586361a7d1b58732243725f242:

#36 Provvedimenti dei dirigenti (DEFINITIVO)
--------------------------------------------

\ |STYLE498|\ : Elenchi dei provvedimenti adottati dai dirigenti

\ |STYLE499|\  Dataset tabellare

\ |STYLE500|\ : Mensile

Obblighi normativi: D. lgs. 33/2013, in particolare art. 23.

Vedi \ |LINK43|\  


+-------------------+----------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                 |Tipo  |Obbligo|
+===================+============================================================================+======+=======+
|Anno               |Anno di riferimento                                                         |Numero|M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE501|\      |Indicare la tipologia di provvedimento tra le seguenti:                     |Testo |O      |
|                   |                                                                            |      |       |
|                   |#. Scelta del contraente per l'affidamento di lavori, forniture e servizi   |      |       |
|                   |                                                                            |      |       |
|                   |#. Accordi stipulati dall'amministrazione                                   |      |       |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE502|\      |Numero identificativo del provvedimento                                     |Numero|M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE503|\      |Titolo del provvedimento                                                    |Testo |M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE504|\      |Dispositivo del provvedimento                                               |Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE505|\      |Data di approvazione del provvedimento.                                     |Data  |M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE506|\      |Nome dell’ufficio proponente                                                |Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE507|\      |Eventuale spesa prevista                                                    |Numero|O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE508|\      |Riferimenti ai documenti principali contenuti nel fascicolo del procedimento|Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h57b79594a60271c37774e4b797e5e68:

#37 Provvedimenti degli organi di indirizzo politico (DEFINITIVO)
-----------------------------------------------------------------

\ |STYLE509|\ : Elenchi dei Provvedimenti degli organi di indirizzo politico

\ |STYLE510|\  Dataset tabellare

\ |STYLE511|\ : Mensile

Obblighi normativi: D. lgs. 33/2013, in particolare art. 23.

Vedi \ |LINK44|\  


+-------------------+----------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                 |Tipo  |Obbligo|
+===================+============================================================================+======+=======+
|Anno               |Anno di riferimento                                                         |Numero|M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE512|\      |Scegliere tra le due opzioni:                                               |Testo |O      |
|                   |                                                                            |      |       |
|                   |* Giunta                                                                    |      |       |
|                   |                                                                            |      |       |
|                   |* Consiglio                                                                 |      |       |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE513|\      |Indicare la tipologia di provvedimento tra le seguenti:                     |Testo |O      |
|                   |                                                                            |      |       |
|                   |#. Scelta del contraente per l'affidamento di lavori, forniture e servizi   |      |       |
|                   |                                                                            |      |       |
|                   |#. Accordi stipulati dall'amministrazione                                   |      |       |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE514|\      |Numero identificativo del provvedimento                                     |Numero|M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE515|\      |Titolo del provvedimento                                                    |Testo |M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE516|\      |Dispositivo del provvedimento                                               |Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE517|\      |Data di approvazione del provvedimento                                      |Data  |M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE518|\      |Nome dell’ufficio proponente                                                |Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE519|\      |Eventuale spesa prevista                                                    |Numero|O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE520|\      |Riferimenti ai documenti principali contenuti nel fascicolo del procedimento|Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2e6413415f50581d7a6f24c6b663027:

10.  TURISMO
============

.. _h39547c1c3b3b73196a1e2b15b6df56:

#32 Accompagnatori turistici (DEFINITIVO) 
------------------------------------------

\ |STYLE521|\ : Elenco degli abilitati per l’esercizio della professione di accompagnatore turistico

\ |STYLE522|\  Dataset tabellare

\ |STYLE523|\ : Tempestiva

+-------------------+-----------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                    |Tipo  |Obbligo|
+===================+===============================================+======+=======+
|Comune             |Comune di riferimento                          |Testo |M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE524|\      |Anno di riferimento                            |Numero|M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE525|\      |Cognome dell’accompagnatore turistico abilitato|Testo |M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE526|\      |Nome dell’accompagnatore turistico abilitato   |Testo |M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE527|\      |Indicare la lingua conosciuta                  |Testo |M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE528|\      |Indicare la lingua conosciuta                  |Testo |O      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE529|\      |Indicare la lingua conosciuta                  |Testo |O      |
+-------------------+-----------------------------------------------+------+-------+

.. _h6e806e58126f423e6813804173126a5a:

#43 Flussi turistici (DEFINITIVO)
---------------------------------

\ |STYLE530|\ : Dati statistici sui flussi turistici

\ |STYLE531|\  Dataset tabellare

\ |STYLE532|\ : Trimestrale

+-------------------+-----------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                  |Tipo  |Obbligo|
+===================+=============================================================================+======+=======+
|Anno               |Anno di riferimento                                                          |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE533|\      |Mese di riferimento                                                          |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE534|\      |Comune di riferimento                                                        |Testo |M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE535|\      |Indicare se i dati si riferiscono al settore alberghiero o extra-alberghiero |Testo |M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE536|\      |N. di arrivi di turisti italiani nel mese di riferimento                     |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE537|\      |N. di presenze di turisti italiani nel mese di riferimento                   |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE538|\      |N. di arrivi di turisti stranieri nel mese di riferimento                    |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE539|\      |N. di presenze di turisti stranieri nel mese di riferimento                  |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h4d12065484b7857297a6c195c4b150:

Allegato 1
##########

Standard generali con l’indicazione dei campi relativi ad alcune informazioni.

.. _h492d313c59223e1033626dd213a121:

TABELLA 1 - UBICAZIONE
======================


+-------------------+---------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                  |Tipo |Obbligo|
+===================+=============================================+=====+=======+
|Provincia          |Provincia di riferimento (sigla)             |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE540|\      |Nome del comune dell’area                    |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE541|\      |Codice catastale del Comune                  |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE542|\      |Tipologia toponimo: Via/Piazza ecc.          |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE543|\      |Nome  Via/Piazza ecc.                        |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE544|\      |Numero civico (compresa lettera, se presente)|Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE545|\      |CAP dell’area                                |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h49516427242563e30663f4813296d:

TABELLA 2 - ORARI (senza indicazione stagionalità)
==================================================


+-------------------+-------------------+-----+-------+
|Denominazione Campo|Descrizione        |Tipo |Obbligo|
+===================+===================+=====+=======+
|Lun_Apertura       |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE546|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE547|\      |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE548|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE549|\      |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE550|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE551|\      |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE552|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE553|\      |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE554|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE555|\      |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE556|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE557|\      |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE558|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h3366642f254f454d623621727a177d61:

TABELLA 3 - ORARI CON STAGIONALITA’
===================================


+----------------------+-------------------+-----+-------+
|Denominazione Campo   |Descrizione        |Tipo |Obbligo|
+======================+===================+=====+=======+
|Invernale_Lun_Apertura|Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE559|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE560|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE561|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE562|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE563|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE564|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE565|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE566|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE567|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE568|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE569|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE570|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE571|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE572|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE573|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE574|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE575|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE576|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE577|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE578|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE579|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE580|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE581|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE582|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE583|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE584|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE585|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+

.. _h2c1d74277104e41780968148427e:




.. _h7a6e23362d711679511187c3d5b5a27:

Allegato 2
##########

.. _h266a626635674523124294953492337:

VOCABOLARIO FREQUENZE AGGIORNAMENTO
===================================

Parallelamente alla definizione degli standard relativi ai contenuti minimi dei dataset, stiamo lavorando alla definizione di un vocabolario delle frequenze di aggiornamento. 

Per quanto riguarda il paniere dei dataset qui illustrato, le frequenze di aggiornamento sono già definite nell’allegato B della DGR 7256 del 23/10/2017, ma riteniamo utile condividere anche il vocabolario da utilizzare nel caso in cui decidiate di pubblicare sul portale ulteriori dataset.

La definizione del vocabolario delle frequenze tiene conto anche di quanto previsto dallo standard DCAT-AP_IT  che fa a sua volta riferimento ad un vocabolario europeo standard:

\ |LINK45|\ 

Ecco l’elenco delle frequenze di aggiornamento individuate da specificare nei metadati del dataset:

* \ |STYLE586|\  (Dati la cui frequenza non è prevedibile, ma al verificarsi del cambiamento vengono pubblicati tempestivamente)

* \ |STYLE587|\  (Dati che vengono aggiornati in tempo reale o ogni N ore)

* \ |STYLE588|\ 

* \ |STYLE589|\  

* \ |STYLE590|\ 

* \ |STYLE591|\ 

* \ |STYLE592|\ 

* \ |STYLE593|\ 

* \ |STYLE594|\ 

* \ |STYLE595|\ 

* \ |STYLE596|\  

* \ |STYLE597|\ 

* \ |STYLE598|\ 

* \ |STYLE599|\ 

* \ |STYLE600|\ 

* \ |STYLE601|\  (Dati “storici”, che per loro natura non cambiano)

* \ |STYLE602|\  (Dati soggetti a cambiamento, ma i cui processi di aggiornamento non sono ancora definiti) 

Segue tabella di conversione con le frequenze standard per il \ |STYLE603|\ 


+---------------------------------+----------------------+
|Vocabolario www.dati.lombardia.it|Vocabolario DCAT-AP_IT|
+=================================+======================+
|Tempestiva                       |Irreg                 |
+---------------------------------+----------------------+
|Tempo reale                      |Cont                  |
+---------------------------------+----------------------+
|Giornaliera                      |Daily                 |
+---------------------------------+----------------------+
|Settimanale                      |Weekly                |
+---------------------------------+----------------------+
|Quindicinale                     |Monthly_2             |
+---------------------------------+----------------------+
|Mensile                          |Monthly               |
+---------------------------------+----------------------+
|Bimestrale                       |Bimonthly             |
+---------------------------------+----------------------+
|Trimestrale                      |Quarterly             |
+---------------------------------+----------------------+
|Quadrimestrale                   |Annual_3              |
+---------------------------------+----------------------+
|Semestrale                       |Annual_2              |
+---------------------------------+----------------------+
|Annuale                          |Annual                |
+---------------------------------+----------------------+
|Biennale                         |Biennal               |
+---------------------------------+----------------------+
|Triennale                        |Triennal              |
+---------------------------------+----------------------+
|Quinquennale                     |Other                 |
+---------------------------------+----------------------+
|Decennale                        |Other                 |
+---------------------------------+----------------------+
|Mai                              |Never                 |
+---------------------------------+----------------------+
|Non definita                     |Unknown               |
+---------------------------------+----------------------+


.. bottom of content


.. |STYLE0| replace:: **condividere e consolidare uno standard**

.. |STYLE1| replace:: **qualità**

.. |STYLE2| replace:: **completezza**

.. |STYLE3| replace:: **confronto**

.. |STYLE4| replace:: **fruibilità**

.. |STYLE5| replace:: **prima proposta di contenuti minimi da pubblicare**

.. |STYLE6| replace:: **contenuti mandatori (M)**

.. |STYLE7| replace:: **contenuti opzionali (O)**

.. |STYLE8| replace:: **Quali formati possono avere i dati?**

.. |STYLE9| replace:: **Come scegliere i formati dei dati?**

.. |STYLE10| replace:: **ordinamento crescente/ decrescente dei dati**

.. |STYLE11| replace:: **rappresentazione “percentuale”**

.. |STYLE12| replace:: **rappresentazione geografica**

.. |STYLE13| replace:: **sistema di coordinate WGS-84 EPSG 4326**

.. |STYLE14| replace:: **Specifiche per il formato “numero” e “data**

.. |STYLE15| replace:: **Specifiche per la rappresentazione geografica**

.. |STYLE16| replace:: **NB:**

.. |STYLE17| replace:: **Per i dataset con frequenza di aggiornamento "tempestiva" occorre, almeno mensilmente, aggiornare i metadati.**

.. |STYLE18| replace:: **non cambia l'ultimo aggiornamento dei dati ma l'ultimo aggiornamento dei metadati**

.. |STYLE19| replace:: **Descrizione:**

.. |STYLE20| replace:: **Tipologia:**

.. |STYLE21| replace:: **Frequenza minima:**

.. |STYLE22| replace:: **Foglio**

.. |STYLE23| replace:: **Mappale**

.. |STYLE24| replace:: **Part_cat**

.. |STYLE25| replace:: **Area_fuoco**

.. |STYLE26| replace:: **Area_tot**

.. |STYLE27| replace:: **Vincoli_15**

.. |STYLE28| replace:: **Vincoli_10**

.. |STYLE29| replace:: **Vincoli_5**

.. |STYLE30| replace:: **Descrizione:**

.. |STYLE31| replace:: **Tipologia:**

.. |STYLE32| replace:: **Frequenza minima:**

.. |STYLE33| replace:: **Toponimo**

.. |STYLE34| replace:: **Indirizzo**

.. |STYLE35| replace:: **Area_mq**

.. |STYLE36| replace:: **Descrizione:**

.. |STYLE37| replace:: **Tipologia:**

.. |STYLE38| replace:: **Frequenza minima:**

.. |STYLE39| replace:: **Denominazione**

.. |STYLE40| replace:: **Tipologia**

.. |STYLE41| replace:: **Codice_catastale**

.. |STYLE42| replace:: **Comune**

.. |STYLE43| replace:: **Superficie_mq**

.. |STYLE44| replace:: **Superficie_prato**

.. |STYLE45| replace:: **Recinzione**

.. |STYLE46| replace:: **Giochi_Bambini**

.. |STYLE47| replace:: **Animali_ammessi**

.. |STYLE48| replace:: **Fontanelle**

.. |STYLE49| replace:: **Orari**

.. |STYLE50| replace:: **Descrizione:**

.. |STYLE51| replace:: **Tipologia:**

.. |STYLE52| replace:: **Frequenza minima:**

.. |STYLE53| replace:: **Nome_Impianto**

.. |STYLE54| replace:: **Codice_catastale**

.. |STYLE55| replace:: **Comune**

.. |STYLE56| replace:: **Comuni_serviti**

.. |STYLE57| replace:: **Recettore**

.. |STYLE58| replace:: **Altezza**

.. |STYLE59| replace:: **Indirizzo**

.. |STYLE60| replace:: **Longitude**

.. |STYLE61| replace:: **Latitude**

.. |STYLE62| replace:: **Data_avvio**

.. |STYLE63| replace:: **Descrizione:**

.. |STYLE64| replace:: **Tipologia:**

.. |STYLE65| replace:: **Frequenza minima:**

.. |STYLE66| replace:: **Macro_Categoria_Rifiuti**

.. |STYLE67| replace:: **Categoria_Rifiuti**

.. |STYLE68| replace:: **ID_Categoria_Rifiuti**

.. |STYLE69| replace:: **Modalità_Raccolta**

.. |STYLE70| replace:: **Periodo**

.. |STYLE71| replace:: **Quantità**

.. |STYLE72| replace:: **Descrizione:**

.. |STYLE73| replace:: **Tipologia:**

.. |STYLE74| replace:: **Frequenza minima:**

.. |STYLE75| replace:: **Codice_Pratica**

.. |STYLE76| replace:: **Richiedente**

.. |STYLE77| replace:: **Protocollo**

.. |STYLE78| replace:: **Oggetto_Richiesta**

.. |STYLE79| replace:: **Data_Richiesta**

.. |STYLE80| replace:: **Link_pratica**

.. |STYLE81| replace:: **Descrizione:**

.. |STYLE82| replace:: **Tipologia:**

.. |STYLE83| replace:: **Frequenza minima:**

.. |STYLE84| replace:: **Ubicazione**

.. |STYLE85| replace:: **Tipologia**

.. |STYLE86| replace:: **Superficie**

.. |STYLE87| replace:: **Superficie_Altro**

.. |STYLE88| replace:: **Orari**

.. |STYLE89| replace:: **Longitude**

.. |STYLE90| replace:: **Latitude**

.. |STYLE91| replace:: **Descrizione**

.. |STYLE92| replace:: **Tipologia:**

.. |STYLE93| replace:: **Frequenza minima**

.. |STYLE94| replace:: **Ubicazione**

.. |STYLE95| replace:: **Tipo_Esercizio**

.. |STYLE96| replace:: **Tipo_Somministrazione**

.. |STYLE97| replace:: **Modalità_Somministrazione**

.. |STYLE98| replace:: **Superficie**

.. |STYLE99| replace:: **WiFi**

.. |STYLE100| replace:: **Longitude**

.. |STYLE101| replace:: **Latitude**

.. |STYLE102| replace:: **Orari**

.. |STYLE103| replace:: **Descrizione**

.. |STYLE104| replace:: **Tipologia:**

.. |STYLE105| replace:: **Frequenza minima**

.. |STYLE106| replace:: **Periodo_Rif**

.. |STYLE107| replace:: **Denominazione**

.. |STYLE108| replace:: **Tipo**

.. |STYLE109| replace:: **N_Edizione**

.. |STYLE110| replace:: **Descrizione**

.. |STYLE111| replace:: **Data_Inizio**

.. |STYLE112| replace:: **Ora_Inizio**

.. |STYLE113| replace:: **Data_Fine**

.. |STYLE114| replace:: **Ora_Fine**

.. |STYLE115| replace:: **Sito_Web**

.. |STYLE116| replace:: **Programma**

.. |STYLE117| replace:: **Nome_Organizzatore**

.. |STYLE118| replace:: **Email_Organizzatore**

.. |STYLE119| replace:: **Telefono_Organizzatore**

.. |STYLE120| replace:: **Gratuito**

.. |STYLE121| replace:: **Prezzo**

.. |STYLE122| replace:: **Longitude**

.. |STYLE123| replace:: **Latitude**

.. |STYLE124| replace:: **Descrizione**

.. |STYLE125| replace:: **Tipologia:**

.. |STYLE126| replace:: **Frequenza minima**

.. |STYLE127| replace:: **Nome**

.. |STYLE128| replace:: **Descrizione**

.. |STYLE129| replace:: **Tipologia**

.. |STYLE130| replace:: **Ubicazione**

.. |STYLE131| replace:: **Email**

.. |STYLE132| replace:: **Telefono**

.. |STYLE133| replace:: **Sito_web**

.. |STYLE134| replace:: **Note**

.. |STYLE135| replace:: **Longitude**

.. |STYLE136| replace:: **Latitude**

.. |STYLE137| replace:: **Descrizione**

.. |STYLE138| replace:: **Tipologia:**

.. |STYLE139| replace:: **Frequenza minima**

.. |STYLE140| replace:: **Ubicazione**

.. |STYLE141| replace:: **Telefono**

.. |STYLE142| replace:: **Email**

.. |STYLE143| replace:: **Descrizione**

.. |STYLE144| replace:: **Tipologia:**

.. |STYLE145| replace:: **Frequenza minima**

.. |STYLE146| replace:: **Descrizione**

.. |STYLE147| replace:: **Tipologia:**

.. |STYLE148| replace:: **Frequenza minima**

.. |STYLE149| replace:: **Periodo**

.. |STYLE150| replace:: **Dettagli**

.. |STYLE151| replace:: **Descrizione**

.. |STYLE152| replace:: **Tipologia:**

.. |STYLE153| replace:: **Frequenza minima**

.. |STYLE154| replace:: **Tipo**

.. |STYLE155| replace:: **Orari**

.. |STYLE156| replace:: **Deroghe**

.. |STYLE157| replace:: **Longitude**

.. |STYLE158| replace:: **Latitude**

.. |STYLE159| replace:: **Link**

.. |STYLE160| replace:: **Descrizione**

.. |STYLE161| replace:: **Tipologia:**

.. |STYLE162| replace:: **Frequenza minima**

.. |STYLE163| replace:: **Tipologia**

.. |STYLE164| replace:: **Ubicazione**

.. |STYLE165| replace:: **Orari**

.. |STYLE166| replace:: **Longitude**

.. |STYLE167| replace:: **Latitude**

.. |STYLE168| replace:: **Gratuito**

.. |STYLE169| replace:: **Descrizione**

.. |STYLE170| replace:: **Tipologia:**

.. |STYLE171| replace:: **Frequenza minima**

.. |STYLE172| replace:: **Descr**

.. |STYLE173| replace:: **Tipologia**

.. |STYLE174| replace:: **Sede**

.. |STYLE175| replace:: **Fondo**

.. |STYLE176| replace:: **Lung**

.. |STYLE177| replace:: **Larg**

.. |STYLE178| replace:: **Direzione**

.. |STYLE179| replace:: **Stato**

.. |STYLE180| replace:: **Ambito**

.. |STYLE181| replace:: **Descrizione**

.. |STYLE182| replace:: **Tipologia:**

.. |STYLE183| replace:: **Frequenza minima**

.. |STYLE184| replace:: **Tipo_Area**

.. |STYLE185| replace:: **Toponimo**

.. |STYLE186| replace:: **Indirizzo**

.. |STYLE187| replace:: **Descrizione**

.. |STYLE188| replace:: **Tipologia:**

.. |STYLE189| replace:: **Frequenza minima**

.. |STYLE190| replace:: **Toponimo**

.. |STYLE191| replace:: **Indirizzo**

.. |STYLE192| replace:: **Descrizione**

.. |STYLE193| replace:: **Tipologia:**

.. |STYLE194| replace:: **Frequenza minima**

.. |STYLE195| replace:: **Ubicazione**

.. |STYLE196| replace:: **Latitude**

.. |STYLE197| replace:: **Longitude**

.. |STYLE198| replace:: **N_Bici**

.. |STYLE199| replace:: **Note**

.. |STYLE200| replace:: **Descrizione**

.. |STYLE201| replace:: **Tipologia:**

.. |STYLE202| replace:: **Frequenza minima**

.. |STYLE203| replace:: **Ubicazione**

.. |STYLE204| replace:: **Telefono**

.. |STYLE205| replace:: **Email**

.. |STYLE206| replace:: **Descrizione**

.. |STYLE207| replace:: **Tipologia:**

.. |STYLE208| replace:: **Frequenza minima**

.. |STYLE209| replace:: **Ubicazione**

.. |STYLE210| replace:: **Stalli**

.. |STYLE211| replace:: **Longitude**

.. |STYLE212| replace:: **Latitude**

.. |STYLE213| replace:: **Descrizione**

.. |STYLE214| replace:: **Tipologia:**

.. |STYLE215| replace:: **Frequenza minima**

.. |STYLE216| replace:: **Ubicazione**

.. |STYLE217| replace:: **KW**

.. |STYLE218| replace:: **Modalità_Utilizzo**

.. |STYLE219| replace:: **Tipo_Presa**

.. |STYLE220| replace:: **Veicoli**

.. |STYLE221| replace:: **Data_Attivazione**

.. |STYLE222| replace:: **Longitude**

.. |STYLE223| replace:: **Latitude**

.. |STYLE224| replace:: **Descrizione**

.. |STYLE225| replace:: **Tipologia**

.. |STYLE226| replace:: **Frequenza minima**

.. |STYLE227| replace:: **Data**

.. |STYLE228| replace:: **Ora**

.. |STYLE229| replace:: **Località**

.. |STYLE230| replace:: **Natura_Incidente**

.. |STYLE231| replace:: **N_Illesi**

.. |STYLE232| replace:: **N_Feriti**

.. |STYLE233| replace:: **N_Morti**

.. |STYLE234| replace:: **Pedoni**

.. |STYLE235| replace:: **Velocipedi**

.. |STYLE236| replace:: **Ciclomotori_Motocicli**

.. |STYLE237| replace:: **Mezzi_pesanti**

.. |STYLE238| replace:: **Longitude**

.. |STYLE239| replace:: **Latitude**

.. |STYLE240| replace:: **Descrizione**

.. |STYLE241| replace:: **Tipologia:**

.. |STYLE242| replace:: **Frequenza minima**

.. |STYLE243| replace:: **Tipo_Infrazione**

.. |STYLE244| replace:: **Normativa**

.. |STYLE245| replace:: **Art.**

.. |STYLE246| replace:: **Data**

.. |STYLE247| replace:: **Tipo_Veicolo**

.. |STYLE248| replace:: **Ubicazione**

.. |STYLE249| replace:: **N_Sanzioni**

.. |STYLE250| replace:: **Longitude**

.. |STYLE251| replace:: **Latitude**

.. |STYLE252| replace:: **Descrizione**

.. |STYLE253| replace:: **Tipologia:**

.. |STYLE254| replace:: **Frequenza minima**

.. |STYLE255| replace:: **Provvedimento**

.. |STYLE256| replace:: **Controlli**

.. |STYLE257| replace:: **Verbali**

.. |STYLE258| replace:: **Descrizione**

.. |STYLE259| replace:: **Tipologia:**

.. |STYLE260| replace:: **Frequenza minima**

.. |STYLE261| replace:: **Tipo**

.. |STYLE262| replace:: **Controlli**

.. |STYLE263| replace:: **Verbali**

.. |STYLE264| replace:: **Descrizione**

.. |STYLE265| replace:: **Tipologia:**

.. |STYLE266| replace:: **Frequenza minima**

.. |STYLE267| replace:: **Tornata_elettorale**

.. |STYLE268| replace:: **Collegio_elettorale**

.. |STYLE269| replace:: **Sezione**

.. |STYLE270| replace:: **Soggetto_votato**

.. |STYLE271| replace:: **Voto**

.. |STYLE272| replace:: **N_Voti**

.. |STYLE273| replace:: **Descrizione**

.. |STYLE274| replace:: **Tipologia:**

.. |STYLE275| replace:: **Frequenza minima**

.. |STYLE276| replace:: **Tornata_elettorale**

.. |STYLE277| replace:: **Collegio_elettorale**

.. |STYLE278| replace:: **Sezione**

.. |STYLE279| replace:: **Soggetto_votato**

.. |STYLE280| replace:: **Voto**

.. |STYLE281| replace:: **N_Voti**

.. |STYLE282| replace:: **Descrizione**

.. |STYLE283| replace:: **Tipologia:**

.. |STYLE284| replace:: **Frequenza minima**

.. |STYLE285| replace:: **Tornata_elettorale**

.. |STYLE286| replace:: **Collegio_elettorale**

.. |STYLE287| replace:: **Sezione**

.. |STYLE288| replace:: **Soggetto_votato**

.. |STYLE289| replace:: **Voto**

.. |STYLE290| replace:: **N_Voti**

.. |STYLE291| replace:: **Descrizione**

.. |STYLE292| replace:: **Tipologia:**

.. |STYLE293| replace:: **Frequenza minima**

.. |STYLE294| replace:: **Tornata_Elettorale**

.. |STYLE295| replace:: **Tipo_Elezione**

.. |STYLE296| replace:: **Soggetto_votato**

.. |STYLE297| replace:: **Collegio_elettorale**

.. |STYLE298| replace:: **Sezione**

.. |STYLE299| replace:: **Voto**

.. |STYLE300| replace:: **N_Voti**

.. |STYLE301| replace:: **Descrizione**

.. |STYLE302| replace:: **Tipologia:**

.. |STYLE303| replace:: **Frequenza minima**

.. |STYLE304| replace:: **Condizione**

.. |STYLE305| replace:: **Maschi**

.. |STYLE306| replace:: **Femmine**

.. |STYLE307| replace:: **Descrizione**

.. |STYLE308| replace:: **Tipologia:**

.. |STYLE309| replace:: **Frequenza minima**

.. |STYLE310| replace:: **Indirizzo**

.. |STYLE311| replace:: **Località**

.. |STYLE312| replace:: **S_marcia**

.. |STYLE313| replace:: **Civico_inizio**

.. |STYLE314| replace:: **Civico_fine**

.. |STYLE315| replace:: **Descrizione**

.. |STYLE316| replace:: **Tipologia:**

.. |STYLE317| replace:: **Frequenza minima**

.. |STYLE318| replace:: **Nome_Toponimo**

.. |STYLE319| replace:: **Codice_Toponimo**

.. |STYLE320| replace:: **Storico**

.. |STYLE321| replace:: **Descrizione**

.. |STYLE322| replace:: **Tipologia:**

.. |STYLE323| replace:: **Frequenza minima**

.. |STYLE324| replace:: **Nome_Toponimo**

.. |STYLE325| replace:: **Numero**

.. |STYLE326| replace:: **Subalterno**

.. |STYLE327| replace:: **CAP**

.. |STYLE328| replace:: **Sezione_ISTAT**

.. |STYLE329| replace:: **Longitude**

.. |STYLE330| replace:: **Latitude**

.. |STYLE331| replace:: **Descrizione**

.. |STYLE332| replace:: **Tipologia:**

.. |STYLE333| replace:: **Frequenza minima**

.. |STYLE334| replace:: **Indirizzo**

.. |STYLE335| replace:: **Descrizione**

.. |STYLE336| replace:: **Data_Inizio**

.. |STYLE337| replace:: **Data_Fine**

.. |STYLE338| replace:: **Descrizione**

.. |STYLE339| replace:: **Tipologia:**

.. |STYLE340| replace:: **Frequenza minima**

.. |STYLE341| replace:: **ID_Accesso**

.. |STYLE342| replace:: **Tipologia_Accesso**

.. |STYLE343| replace:: **Sito**

.. |STYLE344| replace:: **Attivo**

.. |STYLE345| replace:: **Codice**

.. |STYLE346| replace:: **Longitude**

.. |STYLE347| replace:: **Latitude**

.. |STYLE348| replace:: **Raggio_Copertura_m**

.. |STYLE349| replace:: **Descrizione**

.. |STYLE350| replace:: **Tipologia:**

.. |STYLE351| replace:: **Frequenza minima**

.. |STYLE352| replace:: **Comune**

.. |STYLE353| replace:: **Toponimo**

.. |STYLE354| replace:: **Indirizzo**

.. |STYLE355| replace:: **Area_mq**

.. |STYLE356| replace:: **Fontane**

.. |STYLE357| replace:: **Attrezzi**

.. |STYLE358| replace:: **Panchine**

.. |STYLE359| replace:: **Descrizione**

.. |STYLE360| replace:: **Tipologia:**

.. |STYLE361| replace:: **Frequenza minima**

.. |STYLE362| replace:: **Tipologia**

.. |STYLE363| replace:: **ID_Istanza**

.. |STYLE364| replace:: **Data_Istanza**

.. |STYLE365| replace:: **Protocollo**

.. |STYLE366| replace:: **N_Provvedimento**

.. |STYLE367| replace:: **Data_Provvedimento**

.. |STYLE368| replace:: **Richiedente**

.. |STYLE369| replace:: **\***

.. |STYLE370| replace:: **Descrizione_ Intervento**

.. |STYLE371| replace:: **Codice_ecografico**

.. |STYLE372| replace:: **Descrizione**

.. |STYLE373| replace:: **Tipologia:**

.. |STYLE374| replace:: **Frequenza minima**

.. |STYLE375| replace:: **Tipologia**

.. |STYLE376| replace:: **Ubicazione**

.. |STYLE377| replace:: **Superficie_mq**

.. |STYLE378| replace:: **Assegnatario**

.. |STYLE379| replace:: **Progetto**

.. |STYLE380| replace:: **Destinazione_d’uso**

.. |STYLE381| replace:: **Atto_Concessione**

.. |STYLE382| replace:: **Data**

.. |STYLE383| replace:: **Durata_Anni**

.. |STYLE384| replace:: **Descrizione**

.. |STYLE385| replace:: **Tipologia:**

.. |STYLE386| replace:: **Frequenza minima**

.. |STYLE387| replace:: **Tipologia**

.. |STYLE388| replace:: **Ubicazione**

.. |STYLE389| replace:: **Telefono**

.. |STYLE390| replace:: **Descrizione**

.. |STYLE391| replace:: **Tipologia:**

.. |STYLE392| replace:: **Frequenza minima**

.. |STYLE393| replace:: **Numero_Provvedimento**

.. |STYLE394| replace:: **Data**

.. |STYLE395| replace:: **Beneficiario**

.. |STYLE396| replace:: **Tipologia_Beneficiario**

.. |STYLE397| replace:: **Codice_fiscale**

.. |STYLE398| replace:: **Partita_IVA**

.. |STYLE399| replace:: **Oggetto**

.. |STYLE400| replace:: **Norma_Titolo**

.. |STYLE401| replace:: **Link_Norma_Titolo**

.. |STYLE402| replace:: **Ufficio**

.. |STYLE403| replace:: **Cognome_Responsabile**

.. |STYLE404| replace:: **Nome_Responsabile**

.. |STYLE405| replace:: **Modalità**

.. |STYLE406| replace:: **Importo**

.. |STYLE407| replace:: **Progetto**

.. |STYLE408| replace:: **Link_Progetto**

.. |STYLE409| replace:: **Curriculum**

.. |STYLE410| replace:: **Descrizione**

.. |STYLE411| replace:: **Tipologia:**

.. |STYLE412| replace:: **Frequenza minima**

.. |STYLE413| replace:: **Tipologia_Locazione**

.. |STYLE414| replace:: **Locatario**

.. |STYLE415| replace:: **Locatore**

.. |STYLE416| replace:: **Ubicazione**

.. |STYLE417| replace:: **Destinazione**

.. |STYLE418| replace:: **Data_Inizio_Contratto**

.. |STYLE419| replace:: **Data_Fine_Contratto**

.. |STYLE420| replace:: **Canone_percepito**

.. |STYLE421| replace:: **Spese_accessorie**

.. |STYLE422| replace:: **Canone_versato**

.. |STYLE423| replace:: **Descrizione**

.. |STYLE424| replace:: **Tipologia:**

.. |STYLE425| replace:: **Frequenza minima**

.. |STYLE426| replace:: **Descrizione**

.. |STYLE427| replace:: **Natura_giuridica**

.. |STYLE428| replace:: **Tipologia_Bene**

.. |STYLE429| replace:: **Categoria_catastale**

.. |STYLE430| replace:: **Sezione**

.. |STYLE431| replace:: **Foglio**

.. |STYLE432| replace:: **Mappale**

.. |STYLE433| replace:: **Subalterno**

.. |STYLE434| replace:: **Classe**

.. |STYLE435| replace:: **Unità**

.. |STYLE436| replace:: **Consistenza**

.. |STYLE437| replace:: **Rendita**

.. |STYLE438| replace:: **Destinazione**

.. |STYLE439| replace:: **Superficie**

.. |STYLE440| replace:: **Valore**

.. |STYLE441| replace:: **Data_Acquisizione**

.. |STYLE442| replace:: **Longitude**

.. |STYLE443| replace:: **Latitude**

.. |STYLE444| replace:: **Descrizione**

.. |STYLE445| replace:: **Tipologia:**

.. |STYLE446| replace:: **Frequenza minima**

.. |STYLE447| replace:: **Titolo**

.. |STYLE448| replace:: **Descrizione**

.. |STYLE449| replace:: **Termine_massimo**

.. |STYLE450| replace:: **Tempi_effettivi**

.. |STYLE451| replace:: **Ufficio_Responsabile**

.. |STYLE452| replace:: **Note**

.. |STYLE453| replace:: **Descrizione**

.. |STYLE454| replace:: **Tipologia:**

.. |STYLE455| replace:: **Frequenza minima**

.. |STYLE456| replace:: **Funzioni_attribuite**

.. |STYLE457| replace:: **Attività_svolte**

.. |STYLE458| replace:: **Quota_Partecipazione**

.. |STYLE459| replace:: **Durata_Impegno**

.. |STYLE460| replace:: **Onere_Impegno**

.. |STYLE461| replace:: **Numero_Rappresentanti**

.. |STYLE462| replace:: **Trattamento_economico**

.. |STYLE463| replace:: **Ultimo_anno**

.. |STYLE464| replace:: **Risultati_Bilancio_Ultimo_anno**

.. |STYLE465| replace:: **Risultati_Bilancio_Penultimo_anno**

.. |STYLE466| replace:: **Risultati_Bilancio_Terzultimo_anno**

.. |STYLE467| replace:: **Sito_istituzionale**

.. |STYLE468| replace:: **Descrizione**

.. |STYLE469| replace:: **Tipologia:**

.. |STYLE470| replace:: **Frequenza minima**

.. |STYLE471| replace:: **Funzioni_attribuite**

.. |STYLE472| replace:: **Attività_svolte**

.. |STYLE473| replace:: **Quota_Partecipazione**

.. |STYLE474| replace:: **Durata_Impegno**

.. |STYLE475| replace:: **Onere_Impegno**

.. |STYLE476| replace:: **Numero_Rappresentanti**

.. |STYLE477| replace:: **Trattamento_economico**

.. |STYLE478| replace:: **Ultimo_anno**

.. |STYLE479| replace:: **Risultati_Bilancio_Ultimo_anno**

.. |STYLE480| replace:: **Risultati_Bilancio_Penultimo_anno**

.. |STYLE481| replace:: **Risultati_Bilancio_Terzultimo_anno**

.. |STYLE482| replace:: **Sito_istituzionale**

.. |STYLE483| replace:: **Descrizione**

.. |STYLE484| replace:: **Tipologia:**

.. |STYLE485| replace:: **Frequenza minima**

.. |STYLE486| replace:: **Funzioni_attribuite**

.. |STYLE487| replace:: **Attività_svolte**

.. |STYLE488| replace:: **Quota_Partecipazione**

.. |STYLE489| replace:: **Durata_Impegno**

.. |STYLE490| replace:: **Onere_Impegno**

.. |STYLE491| replace:: **Numero_Rappresentanti**

.. |STYLE492| replace:: **Trattamento_economico**

.. |STYLE493| replace:: **Ultimo_anno**

.. |STYLE494| replace:: **Risultati_Bilancio_Ultimo_anno**

.. |STYLE495| replace:: **Risultati_Bilancio_Penultimo_anno**

.. |STYLE496| replace:: **Risultati_Bilancio_Terzultimo_anno**

.. |STYLE497| replace:: **Sito_istituzionale**

.. |STYLE498| replace:: **Descrizione**

.. |STYLE499| replace:: **Tipologia:**

.. |STYLE500| replace:: **Frequenza minima**

.. |STYLE501| replace:: **Tipologia_ Provvedimento**

.. |STYLE502| replace:: **Numero_ Provvedimento**

.. |STYLE503| replace:: **Oggetto**

.. |STYLE504| replace:: **Contenuto**

.. |STYLE505| replace:: **Data_Approvazione**

.. |STYLE506| replace:: **Ufficio_proponente**

.. |STYLE507| replace:: **Spesa_prevista**

.. |STYLE508| replace:: **Estremi_Documenti_ Fascicolo**

.. |STYLE509| replace:: **Descrizione**

.. |STYLE510| replace:: **Tipologia:**

.. |STYLE511| replace:: **Frequenza minima**

.. |STYLE512| replace:: **Organo**

.. |STYLE513| replace:: **Tipologia_ Provvedimento**

.. |STYLE514| replace:: **Numero_ Provvedimento**

.. |STYLE515| replace:: **Oggetto**

.. |STYLE516| replace:: **Contenuto**

.. |STYLE517| replace:: **Data_Approvazione**

.. |STYLE518| replace:: **Ufficio proponente**

.. |STYLE519| replace:: **Spesa_prevista**

.. |STYLE520| replace:: **Estremi_Documenti_ Fascicolo**

.. |STYLE521| replace:: **Descrizione**

.. |STYLE522| replace:: **Tipologia:**

.. |STYLE523| replace:: **Frequenza minima**

.. |STYLE524| replace:: **Anno**

.. |STYLE525| replace:: **Cognome**

.. |STYLE526| replace:: **Nome**

.. |STYLE527| replace:: **Lingua 1**

.. |STYLE528| replace:: **Lingua 2**

.. |STYLE529| replace:: **Lingua n**

.. |STYLE530| replace:: **Descrizione**

.. |STYLE531| replace:: **Tipologia:**

.. |STYLE532| replace:: **Frequenza minima**

.. |STYLE533| replace:: **Mese**

.. |STYLE534| replace:: **Comune**

.. |STYLE535| replace:: **Settore**

.. |STYLE536| replace:: **Arrivi_italiani**

.. |STYLE537| replace:: **Presenze_italiani**

.. |STYLE538| replace:: **Arrivi_stranieri**

.. |STYLE539| replace:: **Presenze_stranieri**

.. |STYLE540| replace:: **Comune**

.. |STYLE541| replace:: **Codice_catastale**

.. |STYLE542| replace:: **Toponimo**

.. |STYLE543| replace:: **Indirizzo**

.. |STYLE544| replace:: **Civico**

.. |STYLE545| replace:: **CAP**

.. |STYLE546| replace:: **Lun_Chiusura**

.. |STYLE547| replace:: **Mar_Apertura**

.. |STYLE548| replace:: **Mar_Chiusura**

.. |STYLE549| replace:: **Mer_Apertura**

.. |STYLE550| replace:: **Mer_Chiusura**

.. |STYLE551| replace:: **Gio_Apertura**

.. |STYLE552| replace:: **Gio_Chiusura**

.. |STYLE553| replace:: **Ven_Apertura**

.. |STYLE554| replace:: **Ven_Chiusura**

.. |STYLE555| replace:: **Sab_Apertura**

.. |STYLE556| replace:: **Sab_Chiusura**

.. |STYLE557| replace:: **Dom_Apertura**

.. |STYLE558| replace:: **Dom_Chiusura**

.. |STYLE559| replace:: **Invernale_Lun_Chiusura**

.. |STYLE560| replace:: **Invernale_Mar_Apertura**

.. |STYLE561| replace:: **Invernale_Mar_Chiusura**

.. |STYLE562| replace:: **Invernale_Mer_Apertura**

.. |STYLE563| replace:: **Invernale_Mer_Chiusura**

.. |STYLE564| replace:: **Invernale_Gio_Apertura**

.. |STYLE565| replace:: **Invernale_Gio_Chiusura**

.. |STYLE566| replace:: **Invernale_Ven_Apertura**

.. |STYLE567| replace:: **Invernale_Ven_Chiusura**

.. |STYLE568| replace:: **Invernale_Sab_Apertura**

.. |STYLE569| replace:: **Invernale_Sab_Chiusura**

.. |STYLE570| replace:: **Invernale_Dom_Apertura**

.. |STYLE571| replace:: **Invernale_Dom_Chiusura**

.. |STYLE572| replace:: **Estivo_Lun_Apertura**

.. |STYLE573| replace:: **Estivo_Lun_Chiusura**

.. |STYLE574| replace:: **Estivo_Mar_Apertura**

.. |STYLE575| replace:: **Estivo_Mar_Chiusura**

.. |STYLE576| replace:: **Estivo_Mer_Apertura**

.. |STYLE577| replace:: **Estivo_Mer_Chiusura**

.. |STYLE578| replace:: **Estivo_Gio_Apertura**

.. |STYLE579| replace:: **Estivo_Gio_Chiusura**

.. |STYLE580| replace:: **Estivo_Ven_Apertura**

.. |STYLE581| replace:: **Estivo_Ven_Chiusura**

.. |STYLE582| replace:: **Estivo_Sab_Apertura**

.. |STYLE583| replace:: **Estivo_Sab_Chiusura**

.. |STYLE584| replace:: **Estivo_Dom_Apertura**

.. |STYLE585| replace:: **Estivo_Dom_Chiusura**

.. |STYLE586| replace:: **Tempestiva**

.. |STYLE587| replace:: **Tempo reale**

.. |STYLE588| replace:: **Giornaliera**

.. |STYLE589| replace:: **Settimanale**

.. |STYLE590| replace:: **Quindicinale**

.. |STYLE591| replace:: **Mensile**

.. |STYLE592| replace:: **Bimestrale**

.. |STYLE593| replace:: **Trimestrale**

.. |STYLE594| replace:: **Quadrimestrale**

.. |STYLE595| replace:: **Semestrale**

.. |STYLE596| replace:: **Annuale**

.. |STYLE597| replace:: **Biennale**

.. |STYLE598| replace:: **Triennale**

.. |STYLE599| replace:: **Quinquennale**

.. |STYLE600| replace:: **Decennale**

.. |STYLE601| replace:: **Mai**

.. |STYLE602| replace:: **Non definita**

.. |STYLE603| replace:: **DCAT-AP_IT**


.. |REPLACE1| raw:: html

    <img src="https://raw.githubusercontent.com/cirospat/paniere-dataset-enti-locali/master/docs/img/immagine1.JPG" />

.. |LINK1| raw:: html

    <a href="www.dati.lombardia.it">www.dati.lombardia.it</a>

.. |LINK2| raw:: html

    <a href="www.dati.lombardia.it">www.dati.lombardia.it</a>

.. |LINK3| raw:: html

    <a href="https://www.esri.com/library/whitepapers/pdfs/shapefile.pdf" target="_blank">https://www.esri.com/library/whitepapers/pdfs/shapefile.pdf</a>

.. |LINK4| raw:: html

    <a href="http://www.agendadigitale.regione.lombardia.it/wps/portal/site/agendadigitale/dettaglioavviso/patrimonio-informativo-pubblico/open-data/iniziaitiva-opendata-marzo-2018" target="_blank">Iniziativa OpenData per gli Enti Locali: quali dati e come pubblicare</a>

.. |LINK5| raw:: html

    <a href="http://www.camera.it/parlam/leggi/00353l.htm" target="_blank">legge 353 del 2000</a>

.. |LINK6| raw:: html

    <a href="https://italiaafuoco.info/" target="_blank">Italia a Fuoco</a>

.. |LINK7| raw:: html

    <a href="https://www.comune.palermo.it/opendata_dld.php?id=278" target="_blank">https://www.comune.palermo.it/opendata_dld.php?id=278</a>

.. |LINK8| raw:: html

    <a href="http://dati.comune.bologna.it/node/217" target="_blank">http://dati.comune.bologna.it/node/217</a>

.. |LINK9| raw:: html

    <a href="http://dati.trentino.it/dataset/elenco-dei-siti-di-depurazione" target="_blank">http://dati.trentino.it/dataset/elenco-dei-siti-di-depurazione</a>

.. |LINK10| raw:: html

    <a href="http://dati.toscana.it/organization/2280ad79-92a5-4ec3-970a-d4abcbc6911e?tags=Rifiuti" target="_blank">http://dati.toscana.it/organization/2280ad79-92a5-4ec3-970a-d4abcbc6911e?tags=Rifiuti</a>

.. |LINK11| raw:: html

    <a href="https://www.dati.lombardia.it/Ambiente/COMUNE-DI-ISSO-Rifiuti-quantit-prodotta-/337c-mnzh" target="_blank">https://www.dati.lombardia.it/Ambiente/COMUNE-DI-ISSO-Rifiuti-quantit-prodotta-/337c-mnzh</a>

.. |LINK12| raw:: html

    <a href="http://dati.comune.lecce.it/dataset/suap-pratiche-presentate-al-comune-di-lecce" target="_blank">http://dati.comune.lecce.it/dataset/suap-pratiche-presentate-al-comune-di-lecce</a>

.. |LINK13| raw:: html

    <a href="http://dati.comune.terlizzi.ba.it/dataset/pratiche-suap/resource/ed71e047-604c-40cb-9862-cca70fd6ff6c" target="_blank">http://dati.comune.terlizzi.ba.it/dataset/pratiche-suap/resource/ed71e047-604c-40cb-9862-cca70fd6ff6c</a>

.. |LINK14| raw:: html

    <a href="http://dati.comune.bologna.it/node/648" target="_blank">http://dati.comune.bologna.it/node/648</a>

.. |LINK15| raw:: html

    <a href="https://www.dati.lombardia.it/Cultura/PROVINCIA-MONZA-BRIANZA-Beni-culturali/hxvd-52zt" target="_blank">https://www.dati.lombardia.it/Cultura/PROVINCIA-MONZA-BRIANZA-Beni-culturali/hxvd-52zt</a>

.. |LINK16| raw:: html

    <a href="http://www.lombardiabeniculturali.it/architetture/tipologie/" target="_blank">http://www.lombardiabeniculturali.it/architetture/tipologie/</a>

.. |LINK17| raw:: html

    <a href="http://www.opendata.provincia.roma.it/?q=dataset/albo-provinciale-manutentori-impianti-termici" target="_blank">http://www.opendata.provincia.roma.it/?q=dataset/albo-provinciale-manutentori-impianti-termici</a>

.. |LINK18| raw:: html

    <a href="https://it.wikipedia.org/wiki/General_Transit_Feed_Specification" target="_blank">https://it.wikipedia.org/wiki/General_Transit_Feed_Specification</a>

.. |LINK19| raw:: html

    <a href="https://www.comune.palermo.it/opendata_dld.php?id=857" target="_blank">https://www.comune.palermo.it/opendata_dld.php?id=857</a>

.. |LINK20| raw:: html

    <a href="http://dati.comune.lecce.it/dataset/trasporto-pubblico-locale" target="_blank">http://dati.comune.lecce.it/dataset/trasporto-pubblico-locale</a>

.. |LINK21| raw:: html

    <a href="https://www.dati.lombardia.it/Mobilit-e-trasporti/Orario-Ferroviario-Regionale-Gtfs/3z4k-mxz9/data" target="_blank">https://www.dati.lombardia.it/Mobilit-e-trasporti/Orario-Ferroviario-Regionale-Gtfs/3z4k-mxz9/data</a>

.. |LINK22| raw:: html

    <a href="https://www.dati.lombardia.it/Mobilit-e-trasporti/Comune-Bergamo-Mappa-ZTL/d9mg-gia6" target="_blank">https://www.dati.lombardia.it/Mobilit-e-trasporti/Comune-Bergamo-Mappa-ZTL/d9mg-gia6</a>

.. |LINK23| raw:: html

    <a href="https://www.dati.lombardia.it/Mobilit-e-trasporti/Comune-Bergamo-Varchi-ZTL/wmcb-3jfi" target="_blank">https://www.dati.lombardia.it/Mobilit-e-trasporti/Comune-Bergamo-Varchi-ZTL/wmcb-3jfi</a>

.. |LINK24| raw:: html

    <a href="http://dati.comune.bologna.it/node/2029x" target="_blank">http://dati.comune.bologna.it/node/2029x</a>

.. |LINK25| raw:: html

    <a href="https://www.dati.lombardia.it/Territorio/PROVINCIA-MONZA-BRIANZA-Piste-ciclabili/xh9r-g2rn" target="_blank">https://www.dati.lombardia.it/Territorio/PROVINCIA-MONZA-BRIANZA-Piste-ciclabili/xh9r-g2rn</a>

.. |LINK26| raw:: html

    <a href="https://www.dati.lombardia.it/Mobilit-e-trasporti/Comune-Bergamo-Mappa-piste-ciclabili/ebbv-35wr" target="_blank">https://www.dati.lombardia.it/Mobilit-e-trasporti/Comune-Bergamo-Mappa-piste-ciclabili/ebbv-35wr</a>

.. |LINK27| raw:: html

    <a href="https://www.dati.lombardia.it/Mobilit-e-trasporti/Comune-Bergamo-Mappa-aree-di-sosta/4s28-bc25" target="_blank">https://www.dati.lombardia.it/Mobilit-e-trasporti/Comune-Bergamo-Mappa-aree-di-sosta/4s28-bc25</a>

.. |LINK28| raw:: html

    <a href="http://dati.comune.milano.it/dataset/ds51_trafficotrasporti_aree_pedonali_ztl_zone_30_" target="_blank">http://dati.comune.milano.it/dataset/ds51_trafficotrasporti_aree_pedonali_ztl_zone_30_</a>

.. |LINK29| raw:: html

    <a href="http://dati.comune.matera.it/dataset/bike-sharing" target="_blank">http://dati.comune.matera.it/dataset/bike-sharing</a>

.. |LINK30| raw:: html

    <a href="https://www.dati.lombardia.it/Mobilit-e-trasporti/PROVINCIA-MONZA-BRIANZA-Autoscuole/i8ry-ssk4" target="_blank">https://www.dati.lombardia.it/Mobilit-e-trasporti/PROVINCIA-MONZA-BRIANZA-Autoscuole/i8ry-ssk4</a>

.. |LINK31| raw:: html

    <a href="http://www.datiopen.it/it/opendata/Comune_di_Torino_Stalli_per_disabili" target="_blank">http://www.datiopen.it/it/opendata/Comune_di_Torino_Stalli_per_disabili</a>

.. |LINK32| raw:: html

    <a href="https://www.dati.lombardia.it/Mobilit-e-trasporti/PROVINCIA-MONZA-BRIANZA-Punti-di-ricarica-per-veic/ps6d-qfrf/data" target="_blank">https://www.dati.lombardia.it/Mobilit-e-trasporti/PROVINCIA-MONZA-BRIANZA-Punti-di-ricarica-per-veic/ps6d-qfrf/data</a>

.. |LINK33| raw:: html

    <a href="https://www.dati.lombardia.it/Mobilit-e-trasporti/Comune-Bergamo-Incidenti-stradali/hds3-pqjq" target="_blank">https://www.dati.lombardia.it/Mobilit-e-trasporti/Comune-Bergamo-Incidenti-stradali/hds3-pqjq</a>

.. |LINK34| raw:: html

    <a href="http://dati.comune.roma.it/cms/it/dettaglio_incidente_stradale.page?contentId=DTS7477" target="_blank">http://dati.comune.roma.it/cms/it/dettaglio_incidente_stradale.page?contentId=DTS7477</a>

.. |LINK35| raw:: html

    <a href="http://aperto.comune.torino.it/?q=content/violazioni-al-codice-della-strada" target="_blank">http://aperto.comune.torino.it/?q=content/violazioni-al-codice-della-strada</a>

.. |LINK36| raw:: html

    <a href="http://www.comune.napoli.it/flex/cm/pages/ServeBLOB.php/L/IT/IDPagina/22347" target="_blank">http://www.comune.napoli.it/flex/cm/pages/ServeBLOB.php/L/IT/IDPagina/22347</a>

.. |LINK37| raw:: html

    <a href="http://dati.toscana.it/dataset/forze-lavoro-residenti-per-sesso-per-condizione-lavorativa-unica-o-prevalente-anno-2012/resource/9525070d-68ad-4d37-8c73-c988a4a23319" target="_blank">http://dati.toscana.it/dataset/forze-lavoro-residenti-per-sesso-per-condizione-lavorativa-unica-o-prevalente-anno-2012/resource/9525070d-68ad-4d37-8c73-c988a4a23319</a>

.. |LINK38| raw:: html

    <a href="https://www.dati.lombardia.it/Territorio/Comune-Bergamo-Toponimi-stradali/9fc2-xiex" target="_blank">https://www.dati.lombardia.it/Territorio/Comune-Bergamo-Toponimi-stradali/9fc2-xiex</a>

.. |LINK39| raw:: html

    <a href="https://www.dati.lombardia.it/Territorio/Comune-Bergamo-Hotspot-WiFi/7kes-vgta/data" target="_blank">https://www.dati.lombardia.it/Territorio/Comune-Bergamo-Hotspot-WiFi/7kes-vgta/data</a>

.. |LINK40| raw:: html

    <a href="http://dati.comune.lecce.it/dataset/elenco-pratiche-sue" target="_blank">http://dati.comune.lecce.it/dataset/elenco-pratiche-sue</a>

.. |LINK41| raw:: html

    <a href="https://www.dati.lombardia.it/Territorio/PROVINCIA-MONZA-BRIANZA-Officine-di-revisione-veic/7yxi-9fvn/data" target="_blank">https://www.dati.lombardia.it/Territorio/PROVINCIA-MONZA-BRIANZA-Officine-di-revisione-veic/7yxi-9fvn/data</a>

.. |LINK42| raw:: html

    <a href="http://www.anticorruzione.it/portal/public/classic/MenuServizio/FAQ/Trasparenza#13" target="_blank">FAQ dell’ANAC relative agli artt. 26-27</a>

.. |LINK43| raw:: html

    <a href="https://www.anticorruzione.it/portal/public/classic/MenuServizio/FAQ/Trasparenza#11" target="_blank">FAQ dell’ANAC relative all’art. 23</a>

.. |LINK44| raw:: html

    <a href="https://www.anticorruzione.it/portal/public/classic/MenuServizio/FAQ/Trasparenza#11" target="_blank">FAQ dell’ANAC relative all’art. 23</a>

.. |LINK45| raw:: html

    <a href="http://linee-guida-cataloghi-dati-profilo-dcat-ap-it.readthedocs.io/it/latest/dataset_elementi_obbligatori.html#frequenza-aggiornamento-dataset-dct-accrualperiodicity" target="_blank">http://linee-guida-cataloghi-dati-profilo-dcat-ap-it.readthedocs.io/it/latest/dataset_elementi_obbligatori.html#frequenza-aggiornamento-dataset-dct-accrualperiodicity</a>

