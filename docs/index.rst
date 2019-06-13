
.. _h3b9431e3a511972f35d463f382d2:

Definizione Standard per il paniere di dataset degli Enti Locali
################################################################


.. toctree::  
    :maxdepth: 4
    :caption: INDICE 

    index.rst

.. _h978e723e45433d2f562f133364336f:

Obiettivo del documento
***********************

\ |STYLE0|\ 

Definire uno standard è un lavoro preliminare importante per:

#. Migliorare il livello di \ |STYLE1|\  dei dataset

#. Favorire la \ |STYLE2|\  delle informazioni

#. Permettere il \ |STYLE3|\  tra i dati di enti diversi

#. Facilitare la \ |STYLE4|\  dei dati

|

.. _ha5c461d7d142050542f7d6c78805d22:

Metodo di lavoro
****************

Il documento è suddiviso in paragrafi che rappresentano le 10 categorie di dataset presenti nel paniere:

#. \ |STYLE5|\ 

#. \ |STYLE6|\ 

#. \ |STYLE7|\ 

#. \ |STYLE8|\ 

#. \ |STYLE9|\ 

#. \ |STYLE10|\ 

#. \ |STYLE11|\ 

#. \ |STYLE12|\ 

#. \ |STYLE13|\ 

#. \ |STYLE14|\ 

Per ogni dataset è presente una tabella contenente una \ |STYLE15|\ , sulla base delle esperienze raccolte provenienti da diverse amministrazioni.

I contenuti minimi contengono dei \ |STYLE16|\  e dei \ |STYLE17|\  nella colonna “Obbligo” di ciascuna tabella (es. dataset #36 Provvedimenti dei dirigenti). Perchè il dataset possa essere considerato completo, è necessario inserire sia le colonne relative alle informazioni mandatorie compilate (M) sia le colonne, anche non compilate, relative alle informazioni opzionali (O). 

Gli Enti partecipanti possono utilizzare i \ |STYLE18|\  per proporre di:

* modificare i campi 

* inserire nuovi campi

* compilare i campi vuoti

* fare commenti aperti in cui inserire dubbi, suggerimenti, ecc.  

Il Team Open Data Lombardia si occuperà di raccogliere i commenti, di integrare il documento e di rispondere a eventuali dubbi espressi dagli Enti.

|

.. _hc7a4e6e33a4f2b725a72146b557b:

Formato dei dati
****************

\ |STYLE19|\ 

* Numero

* Testo

* Web URL

* Booleano (spunta)

* Data

* Valuta (sconsigliato)

* Percentuale

* Coppia di coordinate geografiche (location)

|

\ |STYLE20|\ 

La piattaforma \ |LINK1|\  ingloba una serie di funzionalità avanzate sui dataset di tipo tabellare (Datasets), che permette di aggiungere funzionalità fruibili direttamente on-line, quali ad esempio l’ordinamento crescente/decrescente, link ad un elemento esterno e altro.

Per permettere l’\ |STYLE21|\ , è necessario scegliere un formato «ordinabile» (numero,data).

Per una \ |STYLE22|\ , occorre scegliere un numero con il punto come separatore dei decimali

Per una \ |STYLE23|\ , occorre inserire una coppia di dati, in formato numerico e con \ |STYLE24|\  (ad es. 46.4039704°, 9.3668236°), dove i numeri dovranno avere un punto come separatore. Un campo conterrà la latitudine e l’altro la longitudine: questi due campi popoleranno una colonna di tipo “location” che verrà usata per creare una vista derivata di tipo «mappa».

|

\ |STYLE25|\ ”

La piattaforma \ |LINK2|\  è costruita con tutti i tipi di formattazione di date e numeri in uso negli USA secondo le specifiche ISO 8601.

Per ovviare ad inconvenienti di rappresentazione, è importante che i numeri contenuti nel dataset non presentino separatori delle migliaia e che i decimali vengano inseriti con il punto come segno separatore.

La visualizzazione finale potrà comunque essere modificata dall’interfaccia utente.

|

\ |STYLE26|\ 

Per la rappresentazione geografica, è possibile:

#. caricare uno shapefile come allegato

#. importare uno shapefile. Questa opzione consente di:

* visualizzare i dati su mappa

* scaricare i dati in diversi formati

* utilizzare le API

Per la specifica degli shapefile fare riferimento a \ |LINK3|\ 

\ |STYLE27|\  Se si utilizza un sistema di coordinate diverso dal WGS-84, occorre specificare questa informazione e includere il sistema utilizzato nello shapefile.

|

.. _h4b6e4114411a7b4b386e221d24477e3:

Frequenza di aggiornamento tempestiva
*************************************

\ |STYLE28|\ 

Anche se i dati non cambiano, occorre quindi specificare nei metadati che i dati pubblicati sono ancora validi: in questo caso, \ |STYLE29|\ . 

Per modificare la data di ultimo aggiornamento dei metadati occorre cliccare su "Modifica Metadata" e modificare la "Data di aggiornamento" presente nella sezione "Frequenza di aggiornamento".


|REPLACE1|


+------------------------------------------------------------------------------------------------------------------+
|Per ulteriori informazioni consultare la pagina dedicata all’evento formativo del 22 marzo scorso: “\ |LINK4|\ ”. |
+------------------------------------------------------------------------------------------------------------------+

 

|


.. _hb2252384d6f2d652c47455b4f755c4:

1.     AMBIENTE
***************

.. _h613337737e83b26d2f785122671612:

#1     Carta degli incendi (DEFINITIVO)
=======================================

\ |STYLE30|\  Mappa e scheda delle aree percorse da incendi 

\ |STYLE31|\  Dataset geografico (Shapefile)

\ |STYLE32|\  Mensile

Obblighi normativi: \ |LINK5|\ , in particolare art. 10 c. 1 e 2.

Interessante il progetto civico: \ |LINK6|\ 

Sono possibili 2 opzioni di pubblicazione:

#. Tabella con informazioni catastali dell’area percorsa dal fuoco (obbligatoria) + shapefile dell’area (opzionale)

#. Inserire nello zip dello shapefile 2 layer: uno con le particelle catastali dell’area percorsa dal fuoco e uno con l’area completa (soluzione con GIS)

+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                                                                                                                                                                                   |Tipo  |Obbligo|
+===================+==============================================================================================================================================================================================================================================================================================+======+=======+
|Data_Inc           |Data dell’incendio                                                                                                                                                                                                                                                                            |Data  |M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE33|\       |Foglio in cui è presente la particella percorsa dal fuoco nella sua totalità o solo parzialmente                                                                                                                                                                                              |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE34|\       |Mappale in cui è presente la particella percorsa dal fuoco nella sua totalità o solo parzialmente                                                                                                                                                                                             |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE35|\       |Particella catastale della zona interessata                                                                                                                                                                                                                                                   |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE36|\       |Area della particella percorsa dal fuoco (mq)                                                                                                                                                                                                                                                 |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE37|\       |Area totale della particella (mq)                                                                                                                                                                                                                                                             |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE38|\       |Indicare se esiste il vincolo (15 anni) che impone il mantenimento della destinazione d’uso preesistente all’incendio impedendone la modifica (SI/NO)                                                                                                                                         |Testo |O      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE39|\       |Indicare se è vietata (vincolo 10 anni) la realizzazione di edifici nonché di strutture e infrastrutture finalizzate ad insediamenti civili ed attività produttive e il divieto di pascolo e di caccia per 10 anni, limitatamente ai soprassuoli delle zone boscate percorsi dal fuoco (SI/NO)|Testo |O      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE40|\       |Indicare se esiste il divieto (vincolo 5 anni) di attività di rimboschimento e di ingegneria ambientale sostenute con risorse finanziarie pubbliche (SI/NO)                                                                                                                                   |Testo |O      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+

|

.. _h2c1d74277104e41780968148427e:




.. _h73633d4a4c4c22737a3215b39c2b3b:

#17     Aree Verdi (DEFINITIVO)
===============================

\ |STYLE41|\  Elenco delle aree verdi del territorio 

\ |STYLE42|\  Dataset geografico (Shapefile)

\ |STYLE43|\  Tempestiva

Esempio 1: \ |LINK7|\ 

Esempio 2: \ |LINK8|\  


+-------------------+-------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                      |Tipo  |Obbligo|
+===================+=================================================+======+=======+
|Denom              |Nome dell’area o descrizione                     |Testo |M      |
+-------------------+-------------------------------------------------+------+-------+
|\ |STYLE44|\       |Via/piazza, ecc.                                 |Testo |M      |
+-------------------+-------------------------------------------------+------+-------+
|\ |STYLE45|\       |Nome della via/piazza                            |Testo |M      |
+-------------------+-------------------------------------------------+------+-------+
|\ |STYLE46|\       |Superficie dell’area (espressa in metri quadrati)|Numero|M      |
+-------------------+-------------------------------------------------+------+-------+

|

.. _h2c1d74277104e41780968148427e:




.. _h534b1577195b553752123805a281950:

#18     Aree Verdi Informazioni (DEFINITIVO)
============================================

\ |STYLE47|\  Informazioni sulle aree verdi

\ |STYLE48|\  Dataset tabellare

\ |STYLE49|\  Tempestiva

NOTA: In seguito alle segnalazioni degli Enti è stato creato un tracciato che contiene informazioni relative alle aree verdi comunali e sovracomunali.


+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo  |Obbligo                      |
+===================+==========================================================================================================================================+======+=============================+
|Anno               |Anno di riferimento                                                                                                                       |Numero|M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE50|\       |Nome dell’area o descrizione                                                                                                              |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE51|\       |Tipologia di area (Comunale/Sovracomunale)                                                                                                |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE52|\       |Codice catastale del comune o dei comuni in cui è ubicata l’area, inserendo tra l’uno e l’altro il separatore pipe                        |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE53|\       |Nome del comune o dei comuni in cui è ubicata l’area, inserendo tra l’uno e l’altro il separatore pipe                                    |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE54|\       |Superficie dell’area (espressa in metri quadrati)                                                                                         |Numero|M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE55|\       |Superficie a prato (espressa in metri quadrati)                                                                                           |Numero|O                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE56|\       |Presenza di recinzione (SI/NO/Non applicabile)                                                                                            |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE57|\       |Presenza di aree giochi per bambini (SI/NO/Non applicabile)                                                                               |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE58|\       |Permesso di introdurre animali (SI/NO/Non applicabile)                                                                                    |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE59|\       |Numero di fontanelle presenti                                                                                                             |Numero|O                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE60|\       |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo |M (se presente la recinzione)|
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+

.. _h2c1d74277104e41780968148427e:




|

.. _h6c466e2d2d97084e145847153214d:

#34 Elenco degli impianti di depurazione (DEFINITIVO)
=====================================================

\ |STYLE61|\  Elenco degli impianti di depurazione pubblici di competenza, georeferenziati 

\ |STYLE62|\  Dataset tabellare

\ |STYLE63|\  Mensile

Esempio: \ |LINK9|\  


+-------------------+--------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                             |Tipo  |Obbligo|
+===================+========================================================+======+=======+
|ID_Impianto        |Codice identificativo dell’impianto                     |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE64|\       |Nome dell’impianto                                      |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE65|\       |Codice identificativo del comune                        |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE66|\       |Comune di riferimento                                   |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE67|\       |Comuni serviti dall’impianto                            |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE68|\       |Indicare il corpo idrico recettore (es. nome “fiume x”) |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE69|\       |Altezza espressa in mslm                                |Numero|M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE70|\       |Via in cui si trova l’impianto                          |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE71|\       |Longitudine                                             |Numero|M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE72|\       |Latitudine                                              |Numero|M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE73|\       |Data di avvio                                           |Data  |O      |
+-------------------+--------------------------------------------------------+------+-------+

|

.. _h43321d10544d6f71592d465d7a1f3b4d:

#35 Quantità rifiuti prodotta (DEFINITIVO)
==========================================

\ |STYLE74|\  Quantità di rifiuti prodotti dalla raccolta differenziata e non differenziata, specificandone categoria e modalità di raccolta. 

\ |STYLE75|\  Dataset tabellare

\ |STYLE76|\  Mensile

Esempio 1: \ |LINK10|\ 

Esempio 2: Comune di Isso -  \ |LINK11|\ 


+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                               |Tipo  |Obbligo|
+===================+==========================================================================================================================+======+=======+
|Anno               |Anno di riferimento                                                                                                       |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE77|\       |Indicare se si tratta di rifiuti non differenziati, raccolta differenziata o Inerti e rifiuti da costruzione e demolizione|Testo |M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE78|\       |Indicare la categoria di rifiuti (es. carta e cartone, vetro, ecc.)                                                       |Testo |M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE79|\       |Codice della Categoria rifiuti                                                                                            |Testo |O      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE80|\       |Indicare la modalità di raccolta (es. meccanizzata, porta a porta, area attrezzata)                                       |Testo |M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE81|\       |Indicare il mese di riferimento in numero                                                                                 |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE82|\       |Indicare la quantità in kg                                                                                                |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+

|

.. _h5a82773c2c5d1dc685335262c4f51:

2.     COMMERCIO
****************

.. _h4a55719171347357e636635565315a:

#20        Pratiche SUAP (DEFINITIVO)
=====================================

\ |STYLE83|\  Elenco pratiche gestite dallo Sportello Unico Attività Produttive

\ |STYLE84|\  Dataset tabellare

\ |STYLE85|\  Mensile

Esempio 1: \ |LINK12|\  

Esempio 2: \ |LINK13|\  


+-------------------+-----------------------------------+-------+-------+
|Denominazione Campo|Descrizione                        |Tipo   |Obbligo|
+===================+===================================+=======+=======+
|Anno               |Anno di riferimento                |Numero |M      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE86|\       |Codice identificativo della pratica|Testo  |O      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE87|\       |Ragione sociale del richiedente    |Testo  |M      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE88|\       |Numero di protocollo               |Testo  |M      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE89|\       |Indicare l’oggetto della richiesta |Testo  |O      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE90|\       |Data della richiesta               |Data   |M      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE91|\       |Link alla pratica                  |Web URL|O      |
+-------------------+-----------------------------------+-------+-------+

|

.. _h2c1d74277104e41780968148427e:




.. _h65512721d471161b6456c5353295:

#45        Servizi alla persona (DEFINITIVO)
============================================

\ |STYLE92|\  Elenco e informazioni relative ai servizi alla persona

\ |STYLE93|\  Dataset tabellare

\ |STYLE94|\  Tempestiva

Esempio: \ |LINK14|\  

+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo  |Obbligo|
+===================+==========================================================================================================================================+======+=======+
|Denominazione      |Denominazione attività                                                                                                                    |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE95|\       |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                                                                           |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE96|\       |Breve descrizione del tipo di servizio offerto (ad esempio parrucchiere, estetista, ecc.)                                                 |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE97|\       |Superficie destinata all’esercizio dell’attività (espressa in metri quadrati)                                                             |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE98|\       |Superficie destinata ad altri usi (espressa in metri quadrati)                                                                            |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE99|\       |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE100|\      |Longitudine                                                                                                                               |Numero|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE101|\      |Latitudine                                                                                                                                |Numero|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+

|

.. _h2c1d74277104e41780968148427e:




.. _h192d703349757a442f2040344a7476f:

#47    Pubblici esercizi (DEFINITIVO)
=====================================

\ |STYLE102|\ : Informazioni sugli esercizi pubblici con dati georeferenziati

\ |STYLE103|\  Dataset tabellare

\ |STYLE104|\ : Tempestiva

+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo  |Obbligo|
+===================+==========================================================================================================================================+======+=======+
|Denominazione      |Denominazione esercizio                                                                                                                   |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE105|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                                                                           |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE106|\      |Tipologia di esercizio (ad esempio bar, ristorante ecc.)                                                                                  |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE107|\      |Tipologia di somministrazione (ad esempio bevande, pasti ecc.)                                                                            |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE108|\      |Modalità di somministrazione (ad esempio al banco, al tavolo ecc.)                                                                        |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE109|\      |Superficie destinata alla somministrazione (espressa in metri quadrati)                                                                   |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE110|\      |Presenza di WiFi pubblico (Si/No)                                                                                                         |Testo |O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE111|\      |Longitudine                                                                                                                               |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE112|\      |Latitudine                                                                                                                                |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE113|\      |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo |O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+

|

.. _h1216263d3b30172471575b782e2e3b7a:

3.       CULTURA
****************

.. _h1e1aa304264214b219785d425e70:

#48   Eventi (DEFINITIVO)
=========================

\ |STYLE114|\ : Informazioni su eventi e manifestazioni 

\ |STYLE115|\  Dataset tabellare

\ |STYLE116|\ : Tempestiva

+-------------------+---------------------------------------------------------------+--------+---------------------------+
|Denominazione Campo|Descrizione                                                    |Tipo    |Obbligo                    |
+===================+===============================================================+========+===========================+
|Ubicazione         |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE117|\      |Anno di riferimento                                            |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE118|\      |Denominazione evento                                           |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE119|\      |Tipologia evento                                               |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE120|\      |Numero edizione dell’evento                                    |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE121|\      |Descrizione dell’evento                                        |Testo   |O                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE122|\      |Data di inizio dell’evento                                     |Data    |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE123|\      |Ora di inizio dell’evento                                      |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE124|\      |Data di conclusione dell’evento                                |Data    |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE125|\      |Ora di conclusione dell’evento                                 |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE126|\      |Link al sito web dell’evento                                   |Link Web|M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE127|\      |Link al programma dell’evento                                  |Link Web|M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE128|\      |Nome dell’ente che organizza l’evento                          |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE129|\      |Indirizzo email dell’ente organizzatore                        |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE130|\      |Telefono dell’ente organizzatore                               |Testo   |O                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE131|\      |Evento gratuito (SI/NO)                                        |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE132|\      |Prezzo biglietto                                               |Testo   | M (se evento non gratuito)|
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE133|\      |Longitudine                                                    |Numero  |O                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE134|\      |Latitudine                                                     |Numero  |O                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+

|

.. _h161c2f3833454e4976932653c2b775:

#50 Beni artistici e architettonici (DEFINITIVO)
================================================

\ |STYLE135|\ : Beni artistici e architettonici del territorio

\ |STYLE136|\  Dataset tabellare

\ |STYLE137|\ : Tempestiva

Esempio: \ |LINK15|\  

+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|Denominazione Campo|Descrizione                                                                               |Tipo   |Obbligo|
+===================+==========================================================================================+=======+=======+
|ID_Bene            |Codice identificativo del bene artistico o architettonico                                 |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE138|\      |Denominazione del bene artistico o architettonico                                         |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE139|\      |Descrizione del bene                                                                      |Testo  |O      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE140|\      |Inserire la tipologia di bene (es. Museo, villa, parco…come classificato qui \ |LINK16|\ )|Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE141|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                           |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE142|\      |Indirizzo email per richiedere informazioni                                               |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE143|\      |Recapito telefonico a cui richiedere informazioni                                         |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE144|\      |Link al sito web                                                                          |Web URL|M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE145|\      |Eventuali ulteriori informazioni                                                          |Testo  |O      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE146|\      |Longitudine                                                                               |Numero |O      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE147|\      |Latitudine                                                                                |Numero |O      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+

|

.. _h405b7c14e20627c163b5a181f5126:

4.       ENERGIA
****************

.. _h31437f1420597a45737174704a683466:

#30 Albo provinciale manutentori impianti termici (DEFINITIVO)
==============================================================

\ |STYLE148|\ : Elenco manutentori impianti termici abilitati

\ |STYLE149|\  Dataset tabellare

\ |STYLE150|\ : Tempestiva

Esempio: \ |LINK17|\  

+-------------------+---------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                    |Tipo  |Obbligo|
+===================+===============================================================+======+=======+
|Nome               |Nome o ragione sociale del manutentore                         |Testo |M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE151|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo |M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE152|\      |Numero telefonico del manutentore                              |Numero|O      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE153|\      |Indirizzo email del manutentore                                |Testo |O      |
+-------------------+---------------------------------------------------------------+------+-------+

|


.. _h496c7f2d61647381a4a4c53306f344a:

5.       MOBILITÀ E TRASPORTI
*****************************

.. _h71376c30591b534c645e1d4c7b187:

#3 Orario Trasporto Pubblico (DEFINITIVO)
=========================================

\ |STYLE154|\ : Il dataset contiene i dati relativi alle corse, agli orari e alle fermate del trasporto pubblico urbano ed extra-urbano (pianificato). 

\ |STYLE155|\  Dataset tabellare

\ |STYLE156|\ : Tempestiva

Si tratta di uno Zip file. Lo standard di riferimento è il GTFS. \ |LINK18|\ 

Esempio 1: \ |LINK19|\   

Esempio 2: \ |LINK20|\  

Esempio 3: \ |LINK21|\  

|

.. _h3761631274d34195427717075576131:

#8 Mappa ZTL (DEFINITIVO)
=========================

\ |STYLE157|\ : Mappa Zona a Traffico Limitato 

\ |STYLE158|\  Dataset geografico (Shapefile)

\ |STYLE159|\ : Tempestiva

Esempio: \ |LINK22|\  


+-------------------+--------------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                                   |Tipo |Obbligo|
+===================+==============================================================+=====+=======+
|Nome_ZTL           |Denominazione della ZTL                                       |Testo|M      |
+-------------------+--------------------------------------------------------------+-----+-------+
|\ |STYLE160|\      |Indicare il periodo di riferimento (es. annuale, estivo, ecc.)|Testo|M      |
+-------------------+--------------------------------------------------------------+-----+-------+
|\ |STYLE161|\      |Informazioni aggiuntive (es. orari)                           |Testo|M      |
+-------------------+--------------------------------------------------------------+-----+-------+

|

.. _h794ab20525873f625363207210359:

#9 Varchi ZTL (DEFINITIVO)
==========================

\ |STYLE162|\ : Informazioni sui  varchi della ZTL, georeferenziati

\ |STYLE163|\  Dataset tabellare

\ |STYLE164|\ : Tempestiva

Esempio: \ |LINK23|\  

+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo   |Obbligo|
+===================+==========================================================================================================================================+=======+=======+
|Via                |Nome della via in cui è posizionato il varco                                                                                              |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE165|\      |Tipologia del varco (es. videosorvegliato)                                                                                                |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE166|\      |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo  |O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE167|\      |Eventuali deroghe all’accesso (ad esempio velocipedi)                                                                                     |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE168|\      |Longitudine                                                                                                                               |Numero |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE169|\      |Latitudine                                                                                                                                |Numero |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE170|\      |Link alla pagina informativa, se presente sul sito web dell’ente                                                                          |Web URL|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+

|

.. _h477818b50292f6c2d1821685f246:

#10 Parcheggi (DEFINITIVO)
==========================

\ |STYLE171|\ : Posizione e informazioni sui Parcheggi

\ |STYLE172|\  Dataset tabellare

\ |STYLE173|\ : Tempestiva

Esempio: \ |LINK24|\  

+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo  |Obbligo|
+===================+==========================================================================================================================================+======+=======+
|ID_Parcheggio      |Codice identificativo del parcheggio                                                                                                      |Testo |O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE174|\      |Tipologia del parcheggio (es. aperto, coperto)                                                                                            |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE175|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                                                                           |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE176|\      |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE177|\      |Longitudine                                                                                                                               |Numero|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE178|\      |Latitudine                                                                                                                                |Numero|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE179|\      |Indicare se il parcheggio è gratuito (SI/NO)                                                                                              |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+

|

.. _h7a387f69313ca44387272731b5f2b50:

#11   Piste ciclabili (DEFINITIVO)
==================================

\ |STYLE180|\ : Tracciato delle piste ciclabili  piste ciclabili

\ |STYLE181|\  Dataset geografico (Shapefile)

\ |STYLE182|\ : Tempestiva

Esempio 1: \ |LINK25|\ 

Esempio 2: \ |LINK26|\ 

+-------------------+-------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                            |Tipo  |Obbligo|
+===================+=======================================================+======+=======+
|ID                 |Identificativo pista ciclabile                         |Testo |M      |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE183|\      |Breve descrizione                                      |Testo |M      |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE184|\      |Tipologia percorso, scegliendo tra le seguenti opzioni:|Testo |M      |
|                   |                                                       |      |       |
|                   |* ciclabile                                            |      |       |
|                   |                                                       |      |       |
|                   |* ciclopedonale                                        |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE185|\      |Indicare una delle seguenti opzioni:                   |Testo |M      |
|                   |                                                       |      |       |
|                   |* sede propria                                         |      |       |
|                   |                                                       |      |       |
|                   |* sede promiscua veicolare                             |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE186|\      |Tipo di fondo, scegliendo tra:                         |Testo |M      |
|                   |                                                       |      |       |
|                   |* asfaltato                                            |      |       |
|                   |                                                       |      |       |
|                   |* sterrato                                             |      |       |
|                   |                                                       |      |       |
|                   |* ciottolato                                           |      |       |
|                   |                                                       |      |       |
|                   |* pavimentato (es. resina)                             |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE187|\      |Lunghezza del percorso (espressa in metri)             |Numero|M      |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE188|\      |Larghezza del percorso (espressa in metri)             |Numero|O      |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE189|\      |Specificare una delle seguenti opzioni:                |Testo |M      |
|                   |                                                       |      |       |
|                   |* monodirezionale                                      |      |       |
|                   |                                                       |      |       |
|                   |* bidirezionale                                        |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE190|\      |Indicare una delle seguenti opzioni:                   |Testo |O      |
|                   |                                                       |      |       |
|                   |* aperta                                               |      |       |
|                   |                                                       |      |       |
|                   |* chiusa                                               |      |       |
|                   |                                                       |      |       |
|                   |* in costruzione                                       |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE191|\      |Ambito del percorso (es. stradale, fluviale, parco)    |Testo |O      |
+-------------------+-------------------------------------------------------+------+-------+

|

.. _h4673596e42433c23372f496042157a48:

#12 Aree di sosta (DEFINITIVO)
==============================

\ |STYLE192|\ : Aree di sosta 

\ |STYLE193|\  Dataset geografico (Shapefile)

\ |STYLE194|\ : Tempestiva

Esempio: \ |LINK27|\  

+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                                                                                                                |Tipo |Obbligo|
+===================+===========================================================================================================================================+=====+=======+
|ID_Area            |Codice identificativo dell’area                                                                                                            |Testo|M      |
+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+
|\ |STYLE195|\      |Indicare la tipologia di area per soggetto interessato (es. disabili, sosta libera, bici, autobus, autocarri,ecc.) come da tabella seguente|Testo|M      |
+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+
|\ |STYLE196|\      |Via, Piazza, ecc                                                                                                                           |Testo|M      |
+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+
|\ |STYLE197|\      |Nome Via, Piazza, ecc.                                                                                                                     |Testo|M      |
+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+

|


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

|

.. _h74377a1f30156255c70574b4a62b69:

#13 Aree pedonali (DEFINITIVO)
==============================

\ |STYLE198|\ : Aree pedonali

\ |STYLE199|\  Dataset geografico (Shapefile)

\ |STYLE200|\ : Tempestiva

Esempio: \ |LINK28|\  

+-------------------+-------------------------------+-----+-------+
|Denominazione Campo|Descrizione                    |Tipo |Obbligo|
+===================+===============================+=====+=======+
|ID_Area            |Codice identificativo dell’area|Testo|M      |
+-------------------+-------------------------------+-----+-------+
|\ |STYLE201|\      |Via, Piazza, ecc               |Testo|M      |
+-------------------+-------------------------------+-----+-------+
|\ |STYLE202|\      |Nome Via, Piazza, ecc.         |Testo|M      |
+-------------------+-------------------------------+-----+-------+

|

.. _h413751694948146ea793c3974582760:

#15 Bike sharing (DEFINITIVO)
=============================

\ |STYLE203|\ : Postazioni di Bike sharing

\ |STYLE204|\  Dataset geografico (Shapefile)

\ |STYLE205|\ : Tempestiva

Esempio: \ |LINK29|\  

+-------------------+-------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                  |Tipo  |Obbligo|
+===================+=============================================================+======+=======+
|ID_Staz            |Codice identificativo della stazione di bike sharing         |Numero|M      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE206|\      |Per le informazioni di ubicazione vedere Allegato 1 Tabella 1|Testo |M      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE207|\      |Latitudine                                                   |Numero|M      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE208|\      |Longitudine                                                  |Numero|M      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE209|\      |Numero di biciclette disponibile per stazione                |Numero|O      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE210|\      |Ulteriore descrizione dell’area                              |Testo |O      |
+-------------------+-------------------------------------------------------------+------+-------+

|

.. _h2c1d74277104e41780968148427e:




.. _h781030632f513187a587241745959:

#31 Autoscuole (DEFINITIVO)
===========================

\ |STYLE211|\ : Elenco delle Autoscuole autorizzate nel territorio

\ |STYLE212|\  Dataset tabellare

\ |STYLE213|\ : Tempestiva

Esempio: \ |LINK30|\  

L’esempio si riferisce alla tipologia di informazioni da inserire nel dataset. Per quanto riguarda la suddivisione delle informazioni in campi, occorre fare riferimento alla tabella seguente. In particolare, per l’indirizzo occorre inserire tutti i campi previsti per l’ubicazione come indicati nell’Allegato 1 Tabella 1. 

+-------------------+---------------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                                    |Tipo |Obbligo|
+===================+===============================================================+=====+=======+
|Nome               |Nome dell’autoscuola                                           |Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE214|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE215|\      |Numero di telefono dell’autoscuola                             |Testo|O      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE216|\      |Indirizzo email dell’autoscuola                                |Testo|O      |
+-------------------+---------------------------------------------------------------+-----+-------+

|

.. _h29173c11c44516963343b7a352726b:

#33 Aree di sosta per disabili (DEFINITIVO)
===========================================

\ |STYLE217|\ : Elenco delle Aree di sosta per disabili presenti nel territorio

\ |STYLE218|\  Dataset tabellare

\ |STYLE219|\ : Tempestiva

Esempio: \ |LINK31|\  

+-------------------+---------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                    |Tipo  |Obbligo|
+===================+===============================================================+======+=======+
|ID_Area            |Codice identificativo dell’area                                |Testo |M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE220|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo |M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE221|\      |Numero stalli dell’area di sosta                               |Numero|M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE222|\      |Longitudine                                                    |Numero|O      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE223|\      |Latitudine                                                     |Numero|O      |
+-------------------+---------------------------------------------------------------+------+-------+

|

.. _h7f1d5c471796a7032617255597b173a:

#44 Punti di ricarica veicoli (DEFINITIVO)
==========================================

\ |STYLE224|\ : Dataset con coordinate geografiche dei punti di ricarica dei veicoli elettrici, con indicazione del tipo di presa e KW

\ |STYLE225|\  Dataset tabellare

\ |STYLE226|\ : Tempestiva

Esempio: \ |LINK32|\  

+-------------------+--------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                     |Tipo  |Obbligo|
+===================+================================================================================+======+=======+
|ID_Sito            |Codice identificativo del sito in cui è possibile ricaricare i veicoli elettrici|Numero|O      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE227|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                 |Testo |M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE228|\      |Potenza della ricarica                                                          |Numero|M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE229|\      |Indicare la modalità di utilizzo del servizio (es. tramite CRS)                 |Testo |M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE230|\      |Indicare la tipologia di presa (es. universale)                                 |Testo |M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE231|\      |Indicare le tipologie di veicoli per le quali è disponibile la ricarica         |Testo |M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE232|\      |Data di attivazione del sito                                                    |Data  |O      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE233|\      |Longitudine                                                                     |Numero|M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE234|\      |Latitudine                                                                      |Numero|M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+

|

.. _h127c74681e53786e536b765a2f6647e:

6.       SICUREZZA
******************

.. _h824122d55a315e452768e7f292a6e:

#7 Incidenti stradali (DEFINITIVO)
==================================

\ |STYLE235|\ : Dataset contenente gli incidenti stradali con data, ora, coordinate geografiche, mezzi coinvolti, eventuali morti e feriti

\ |STYLE236|\ : Dataset tabellare

\ |STYLE237|\ : Mensile

Esempio 1: \ |LINK33|\ 

Esempio 2: \ |LINK34|\  

+-------------------+----------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                       |Tipo  |Obbligo|
+===================+==================================================================================+======+=======+
|Anno               |Anno di riferimento                                                               |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE238|\      |Data dell’incidente                                                               |Data  |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE239|\      |Ora dell’incidente                                                                |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE240|\      |Descrizione del punto preciso dell’incidente (es. via...all’intersezione con via…)|Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE241|\      |Tipologia di incidente (es. scontro frontale)                                     |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE242|\      |Numero delle persone illese                                                       |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE243|\      |Numero delle persone ferite                                                       |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE244|\      |Numero dei morti                                                                  |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE245|\      |Indicare se sono stati coinvolti pedoni (SI/NO)                                   |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE246|\      |Indicare se sono stati coinvolti velocipedi (SI/NO)                               |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE247|\      |Indicare se sono stati coinvolti ciclomotori o motocicli (SI/NO)                  |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE248|\      |Indicare se sono stati coinvolti mezzi pesanti (SI/NO)                            |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE249|\      |Longitudine                                                                       |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE250|\      |Latitudine                                                                        |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+

|

.. _h2c1d74277104e41780968148427e:




.. _h4760d266a547666543d45223781653:

#41  Principali infrazioni al Codice della Strada (DEFINITIVO)
==============================================================

\ |STYLE251|\ : Elenco, tipologia e anno di riferimento delle principali infrazioni al Codice della Strada.

\ |STYLE252|\  Dataset tabellare

\ |STYLE253|\ : Mensile

Esempio: \ |LINK35|\ 

+-------------------+--------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                         |Tipo  |Obbligo|
+===================+====================================================================+======+=======+
|Anno               |Anno di riferimento                                                 |Numero|M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE254|\      |Tipo di infrazione (es. limite velocità, sensi unici, sosta, ecc.)  |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE255|\      |Normativa di riferimento dell’infrazione (es. Legge)                |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE256|\      |Art. di legge o altra norma che regola il tipo di infrazione        |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE257|\      |Data infrazione                                                     |Data  |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE258|\      |Tipologia di veicolo: autovettura, motoveicolo, ciclomotore         |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE259|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1     |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE260|\      |Inserire il numero delle sanzioni erogate per l’infrazione specifica|Numero|M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE261|\      |Longitudine                                                         |Numero|O      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE262|\      |Latitudine                                                          |Numero|O      |
+-------------------+--------------------------------------------------------------------+------+-------+

|

.. _h6f396320344978474c3f7b4d6b7e531c:

#42 Provvedimenti adottati dalla Polizia Locale in materia di commercio (DEFINITIVO)
====================================================================================

\ |STYLE263|\ : Elenco e tipologia dei provvedimenti adottati in materia di commercio dalla Polizia Municipale

\ |STYLE264|\  Dataset tabellare

\ |STYLE265|\ : Mensile

Esempio: \ |LINK36|\  

+-------------------+---------------------+------+-------+
|Denominazione Campo|Descrizione          |Tipo  |Obbligo|
+===================+=====================+======+=======+
|Anno               |Anno di riferimento  |Numero|M      |
+-------------------+---------------------+------+-------+
|\ |STYLE266|\      |Tipo di provvedimento|Testo |M      |
+-------------------+---------------------+------+-------+
|\ |STYLE267|\      |Numero di controlli  |Numero|M      |
+-------------------+---------------------+------+-------+
|\ |STYLE268|\      |Numero di verbali    |Numero|M      |
+-------------------+---------------------+------+-------+

|

.. _h2c1d74277104e41780968148427e:




.. _h04573713141737316103050642c523f:

#49 Controlli in cantiere effettuati dalla Polizia Locale (DEFINITIVO)
======================================================================

\ |STYLE269|\ : Elenco, tipologia e anno di riferimento dei controlli effettuati nei cantieri dalla Polizia locale

\ |STYLE270|\  Dataset tabellare

\ |STYLE271|\ : Mensile

+-------------------+----------------------+------+-------+
|Denominazione Campo|Descrizione           |Tipo  |Obbligo|
+===================+======================+======+=======+
|Anno               |Anno di riferimento   |Numero|M      |
+-------------------+----------------------+------+-------+
|\ |STYLE272|\      |Tipologia di controllo|Testo |M      |
+-------------------+----------------------+------+-------+
|\ |STYLE273|\      |Numero di controlli   |Numero|M      |
+-------------------+----------------------+------+-------+
|\ |STYLE274|\      |Numero di verbali     |Numero|M      |
+-------------------+----------------------+------+-------+

|

.. _h6a50711f57485b63626e405f165261:

7.      STATISTICA
******************

Per quanto riguarda i risultati delle elezioni, in seguito ad un’analisi ulteriore è stata individuata una soluzione alternativa alla pubblicazione dei 3 dataset distinti (#38, #39 e #40): pubblicare un unico dataset che comprenda sia i risultati delle elezioni sia i dati statistici sull’affluenza (vedere tabella #38#39#40BIS Risultati elezioni). Questo consentirebbe di mantenere sempre uguale la struttura del dataset (campi) rendendo più facilmente confrontabili i dati. 

Ai fini del co-finanziamento, la pubblicazione del dataset #38#39#40BIS viene equiparata alla pubblicazione dei 3 dataset relativi alle elezioni (#38 + #39 + #40). 

|

.. _h47274b145479547445336f771b35280:

#38 Risultati elezioni comunali (DEFINITIVO)
============================================

\ |STYLE275|\ : Risultati elettorali delle elezioni amministrative del proprio comune o provincia

\ |STYLE276|\  Dataset tabellare

\ |STYLE277|\ : Tempestiva

+-------------------+-----------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                        |Tipo  |Obbligo|
+===================+===================================================================================+======+=======+
|Data               |Data elezione (giorno, mese, anno)                                                 |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE278|\      |Indicare se si tratta di:                                                          |Testo |M      |
|                   |                                                                                   |      |       |
|                   |* 1° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* 2° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* turno unico                                                                      |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE279|\      |Collegio elettorale o circoscrizione                                               |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE280|\      |Numero della sezione                                                               |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE281|\      |Consiglio comunale o Sindaco                                                       |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE282|\      |Inserire in questa colonna una riga per ciascuna delle seguenti informazioni:      |Testo |M      |
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
|\ |STYLE283|\      |Inserire una riga per ciascuna delle seguenti informazioni:                        |Numero|M      |
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

|

.. _h2c1d74277104e41780968148427e:




.. _h6e64461642c1b5e501d5d104b713c1d:

#39 Risultati elezioni regionali (DEFINITIVO)
=============================================

\ |STYLE284|\ : Risultati elettorali delle elezioni regionali nel proprio comune o provincia

\ |STYLE285|\  Dataset tabellare

\ |STYLE286|\ : Tempestiva

+-------------------+-----------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                        |Tipo  |Obbligo|
+===================+===================================================================================+======+=======+
|Data               |Data elezione (giorno, mese, anno)                                                 |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE287|\      |Indicare se si tratta di:                                                          |Testo |M      |
|                   |                                                                                   |      |       |
|                   |* 1° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* 2° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* turno unico                                                                      |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE288|\      |Collegio elettorale o circoscrizione                                               |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE289|\      |Numero della sezione                                                               |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE290|\      |Consiglio regionale o Presidente della Regione                                     |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE291|\      |Inserire in questa colonna una riga per ciascuna delle seguenti informazioni:      |Testo |M      |
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
|\ |STYLE292|\      |Inserire una riga per ciascuna delle seguenti informazioni:                        |Numero|M      |
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

|

.. _h61f79121f287221467271742a444f:

#40 Risultati elezioni nazionali (DEFINITIVO)
=============================================

\ |STYLE293|\ : Risultati elettorali delle elezioni nazionali nel proprio comune o provincia

\ |STYLE294|\  Dataset tabellare

\ |STYLE295|\ : Tempestiva

+-------------------+-----------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                        |Tipo  |Obbligo|
+===================+===================================================================================+======+=======+
|Data               |Data elezione (giorno, mese, anno)                                                 |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE296|\      |Indicare se si tratta di:                                                          |Testo |M      |
|                   |                                                                                   |      |       |
|                   |* 1° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* 2° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* turno unico                                                                      |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE297|\      |Collegio elettorale o circoscrizione                                               |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE298|\      |Numero della sezione                                                               |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE299|\      |Camera dei deputati o Senato della Repubblica                                      |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE300|\      |Inserire in questa colonna una riga per ciascuna delle seguenti informazioni:      |Testo |M      |
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
|\ |STYLE301|\      |Inserire una riga per ciascuna delle seguenti informazioni:                        |Numero|M      |
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

|

.. _h3c4d632b744227d45777a02552663:

#38 #39 #40BIS Risultati elezioni (DEFINITIVO)
==============================================

\ |STYLE302|\ : Risultati elettorali e dati sull’affluenza 

\ |STYLE303|\  Dataset tabellare

\ |STYLE304|\ : Tempestiva

+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                                                                                                                                                |Tipo  |Obbligo|
+===================+===========================================================================================================================================================================================================================================================+======+=======+
|Data               |Data elezione (giorno, mese, anno)                                                                                                                                                                                                                         |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE305|\      |In caso di più tornate elettorali, specificare il turno o indicare se turno unico (1° turno, 2° turno, turno unico)                                                                                                                                        |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE306|\      |Tipologia di elezione (es. Camera, Senato, Comunali, Circoscrizionali, Provinciali, Regionali, Europee, Referendum 1, Referendum 2, ecc.)                                                                                                                  |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE307|\      |Es. Camera dei Deputati, Senato della Repubblica, Consiglio comunale, Sindaco, Consiglio provinciale, Presidente della Provincia, Consiglio regionale, Presidente della Regione, Parlamento europeo, oppure l’oggetto del referendum (es. energia nucleare)|Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE308|\      |Collegio elettorale o Circoscrizione                                                                                                                                                                                                                       |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE309|\      |Numero della sezione                                                                                                                                                                                                                                       |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE310|\      |Inserire in questa colonna una riga per ciascuna delle seguenti informazioni:                                                                                                                                                                              |Testo |M      |
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
|\ |STYLE311|\      |Inserire una riga per ciascuna delle seguenti informazioni:                                                                                                                                                                                                |Numero|M      |
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

|

.. _h492e3345c6f1555f5b19363179137c:

#46 Condizione lavorativa (DEFINITIVO)
======================================

\ |STYLE312|\ : Informazioni sulla condizione lavorativa dei residenti (ad esempio occupato, in cerca di occupazione ecc.)

\ |STYLE313|\  Dataset tabellare

\ |STYLE314|\ : Trimestrale

Esempio: \ |LINK37|\  

+-------------------+-------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                              |Tipo  |Obbligo|
+===================+=========================================================================+======+=======+
|Anno               |Anno di riferimento                                                      |Numero|M      |
+-------------------+-------------------------------------------------------------------------+------+-------+
|\ |STYLE315|\      |Condizione lavorativa (ad esempio occupato, in cerca di occupazione ecc.)|Testo |M      |
+-------------------+-------------------------------------------------------------------------+------+-------+
|\ |STYLE316|\      |Numero di maschi                                                         |Numero|M      |
+-------------------+-------------------------------------------------------------------------+------+-------+
|\ |STYLE317|\      |Numero di femmine                                                        |Numero|M      |
+-------------------+-------------------------------------------------------------------------+------+-------+

|

.. _h47325942212741500d25226c3727f:

8.      TERRITORIO
******************

.. _h784465346686a592127d1e14157730:

#4 Rete viaria - Dataset geografico (DEFINITIVO)
================================================

\ |STYLE318|\ : Rete viaria 

\ |STYLE319|\  Dataset geografico (Shapefile)

\ |STYLE320|\ : Tempestiva

+-------------------+------------------------+-----+-------+
|Denominazione Campo|Descrizione             |Tipo |Obbligo|
+===================+========================+=====+=======+
|Toponimo           |Toponimo della strada   |Testo|M      |
+-------------------+------------------------+-----+-------+
|\ |STYLE321|\      |Nome del toponimo       |Testo|M      |
+-------------------+------------------------+-----+-------+
|\ |STYLE322|\      |Località                |Testo|M      |
+-------------------+------------------------+-----+-------+
|\ |STYLE323|\      |Senso di marcia (U/D/A):|Testo|M      |
|                   |                        |     |       |
|                   |* U - Unico             |     |       |
|                   |                        |     |       |
|                   |* D - Doppio            |     |       |
|                   |                        |     |       |
|                   |* A - Alternato         |     |       |
+-------------------+------------------------+-----+-------+
|\ |STYLE324|\      |Primo numero civico     |Testo|M      |
+-------------------+------------------------+-----+-------+
|\ |STYLE325|\      |Ultimo numero civico    |Testo|M      |
+-------------------+------------------------+-----+-------+

|

.. _h5457273b5f6970146f702b17c7f3550:

#5 Rete viaria - Toponimi stradali (DEFINITIVO)
===============================================

\ |STYLE326|\ : Elenco Toponimi stradali

\ |STYLE327|\  Dataset tabellare

\ |STYLE328|\ : Tempestiva

Esempio: \ |LINK38|\  

+-------------------+----------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                               |Tipo |Obbligo|
+===================+==========================================================+=====+=======+
|Classe_Toponimo    |Indicare la classe toponimo (es. Via, Piazza, Largo, ecc.)|Testo|M      |
+-------------------+----------------------------------------------------------+-----+-------+
|\ |STYLE329|\      |Nome di Via, Piazza, Largo, ecc.                          |Testo|M      |
+-------------------+----------------------------------------------------------+-----+-------+
|\ |STYLE330|\      |Codice del toponimo                                       |Testo|M      |
+-------------------+----------------------------------------------------------+-----+-------+
|\ |STYLE331|\      |Inserire se si tratta di un dato storico (SI/NO)          |Testo|M      |
+-------------------+----------------------------------------------------------+-----+-------+

|

.. _h2c1d74277104e41780968148427e:




.. _h563b1f5f11515e35374069365613121:

#6 Rete viaria - Numeri civici (DEFINITIVO)
===========================================

\ |STYLE332|\ : Numeri civici georeferenziati

\ |STYLE333|\  Dataset tabellare

\ |STYLE334|\ : Tempestiva

Esempio: https://www.dati.lombardia.it/Territorio/Comune-Bergamo-Numerazione-civica/pcif-9jj7

+-------------------+------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                           |Tipo  |Obbligo|
+===================+======================================================+======+=======+
|Classe_Toponimo    |Indicare la classe toponimo (Via, Piazza, Largo, ecc.)|Testo |M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE335|\      |Nome di Via, Piazza, Largo, ecc.                      |Testo |M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE336|\      |Numero del civico                                     |Numero|M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE337|\      |Componente alfabetica del civico (es. A, Bis, ecc.)   |Testo |M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE338|\      |CAP                                                   |Numero|M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE339|\      |Sezione di censimento ISTAT                           |Numero|O      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE340|\      |Longitudine                                           |Numero|M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE341|\      |Latitudine                                            |Numero|M      |
+-------------------+------------------------------------------------------+------+-------+

|

.. _h32623c3510287d7f3af50466d4e60:

#14      Cantieri stradali (DEFINITIVO)
=======================================

\ |STYLE342|\ : Cantieri stradali attivi 

\ |STYLE343|\  Dataset geografico (Shapefile)

\ |STYLE344|\ : Tempestiva


+-------------------+--------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                 |Tipo |Obbligo|
+===================+============================================+=====+=======+
|Toponimo           |Via, Piazza, ecc.                           |Testo|M      |
+-------------------+--------------------------------------------+-----+-------+
|\ |STYLE345|\      |Nome della via, piazza, ecc.                |Testo|M      |
+-------------------+--------------------------------------------+-----+-------+
|\ |STYLE346|\      |Breve descrizione dei lavori in svolgimento |Testo|M      |
+-------------------+--------------------------------------------+-----+-------+
|\ |STYLE347|\      |Data di inizio lavoro                       |Data |M      |
+-------------------+--------------------------------------------+-----+-------+
|\ |STYLE348|\      |Data prevista di fine lavoro                |Data |M      |
+-------------------+--------------------------------------------+-----+-------+

|

.. _h1a736c403f6676679673a673f60363a:

#16 HotSpot Wifi (DEFINITIVO)
=============================

\ |STYLE349|\ : Elenco hotspot wifi pubblici, georeferenziati o dataset geografico

\ |STYLE350|\  Dataset tabellare

\ |STYLE351|\ : Tempestiva

Esempio: \ |LINK39|\  

+-------------------+--------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                           |Tipo  |Obbligo|
+===================+======================================================================================+======+=======+
|Rete               |Nome della rete (SSID)                                                                |Testo |O      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE352|\      |Codice identificativo del punto di accesso (singolo HotSpot Wifi) attribuito dall’ente|Testo |M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE353|\      |Indicare la tipologia del punto di accesso (HotSpot/Dispositivo estensione)           |Testo |O      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE354|\      |Nome del sito dove si trova il punto di accesso (es. denominazione Biblioteca…)       |Testo |M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE355|\      |Punto di accesso attivo (si, no)                                                      |Testo |M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE356|\      |Codice accesso                                                                        |Testo |O      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE357|\      |Longitudine                                                                           |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE358|\      |Latitudine                                                                            |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE359|\      |Indicare il raggio di copertura in metri                                              |Numero|O      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+

 

|

.. _h5a2161623f35403f62b4f305243726a:

#19 Area per sgambatura cani (DEFINITIVO)
=========================================

\ |STYLE360|\ : Mappa aree per sgambatura cani

\ |STYLE361|\  Dataset geografico (Shapefile)

\ |STYLE362|\ : Tempestiva

+-------------------+----------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                     |Tipo  |Obbligo|
+===================+================================================================+======+=======+
|ID_Area            |Codice identificativo dell’area                                 |Numero|M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE363|\      |Comune in cui è ubicata l’area                                  |Testo |M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE364|\      |Via, Piazza, ecc.                                               |Testo |M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE365|\      |Nome della via, piazza, ecc.                                    |Testo |M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE366|\      |Indicare la superficie dell’area (mq)                           |Numero|M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE367|\      |Indicare se sono presenti fontanelle (SI/NO)                    |Testo |O      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE368|\      |Indicare se sono presenti attrezzature per addestramento (SI/NO)|Testo |O      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE369|\      |Indicare se sono presenti panchine(SI/NO)                       |Testo |O      |
+-------------------+----------------------------------------------------------------+------+-------+

|

.. _h2ca5320503f5437a26b171269386a:

#21 Pratiche edilizie (DEFINITIVO) 
===================================

\ |STYLE370|\ : Elenco Pratiche edilizie gestite dallo Sportello Unico per l’Edilizia

\ |STYLE371|\  Dataset tabellare

\ |STYLE372|\ : Mensile

Esempio: \ |LINK40|\  

+-------------------+--------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                             |Tipo  |Obbligo|
+===================+========================================================+======+=======+
|Anno               |Anno di riferimento                                     |Numero|M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE373|\      |Tipologia istanza (es. SCIA, PDC, ecc.)                 |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE374|\      |Codice identificativo dell’istanza                      |Testo |O      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE375|\      |Data di presentazione dell’istanza                      |Data  |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE376|\      |Numero di protocollo dell’istanza                       |Numero|O      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE377|\      |Numero del provvedimento (nel caso di PDC)              |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE378|\      |Data del provvedimento (nel caso di PDC)                |Data  |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE379|\      |Nominativo o Ragione sociale dell’istante \ |STYLE380|\ |Testo |O      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE381|\      |Descrizione dell’intervento oggetto dell’istanza        |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE382|\      |Codice ecografico del fabbricato                        |Testo |O      |
+-------------------+--------------------------------------------------------+------+-------+

\* Ciascun ente valuta la pubblicazione del dato in base al principio del bilanciamento tra l’interesse pubblico a conoscere dati, informazioni e documenti per tutelare i diritti dei cittadini e l’interesse pubblico alla tutela dei diritti delle persone e delle organizzazioni private che potrebbero essere lesi dalla disponibilità di dati, informazioni e documenti.

|

.. _h2c1d74277104e41780968148427e:




.. _h752c462f6e4e4179353571873311521:

#22 Elenco beni confiscati (DEFINITIVO) 
========================================

\ |STYLE383|\ : Elenco beni confiscati alla mafia e assegnati al comune

\ |STYLE384|\  Dataset tabellare

\ |STYLE385|\ : Mensile

+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                              |Tipo  |Obbligo|
+===================+=========================================================================================+======+=======+
|ID_Bene            |Codice identificativo del bene confiscato                                                |Testo |O      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE386|\      |Tipologia del bene confiscato (es. appartamento, villa, ecc.)                            |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE387|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                          |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE388|\      |Superficie del bene confiscato (mq)                                                      |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE389|\      |Nominativo o ragione sociale dell’assegnatario del bene                                  |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE390|\      |Breve descrizione del progetto in funzione del quale il bene confiscato è stato assegnato|Testo |O      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE391|\      |Destinazione d’uso del bene confiscato                                                   |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE392|\      |Riferimenti all’atto di concessione                                                      |Testo |O      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE393|\      |Data dell’atto di concessione                                                            |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE394|\      |Numero di anni della concessione                                                         |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+

|

.. _h1534f311220496307c39787c131e20:

#29 Centri revisione auto (DEFINITIVO)
======================================

\ |STYLE395|\ : Centri revisione auto autorizzati dalla Provincia

\ |STYLE396|\  Dataset tabellare

\ |STYLE397|\ : Tempestiva

Esempio: \ |LINK41|\ 


+-------------------+---------------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                                    |Tipo |Obbligo|
+===================+===============================================================+=====+=======+
|Nome               |Nome del centro di revisione                                   |Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE398|\      |Tipologia di revisione (es. auto, moto, ecc.)                  |Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE399|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE400|\      |Numero di telefono del centro di revisione                     |Testo|O      |
+-------------------+---------------------------------------------------------------+-----+-------+

|

.. _h5e126927772356f4b3651622c12502f:

9.  TRASPARENZA 
****************

.. _h6a113f1a7b5a1f2e7d29274624462967:

#2 Contributi e sussidi (DEFINITIVO)
====================================

\ |STYLE401|\ : Dati relativi agli atti di concessione di sovvenzioni, contributi, sussidi ed ausili finanziari alle imprese e comunque di vantaggi economici di qualunque genere a persone ed enti pubblici e privati

\ |STYLE402|\  Dataset tabellare

\ |STYLE403|\ : Tempestiva

Obblighi normativi: D. lgs. 33/2013, in particolare artt. 26-27.

Vedi \ |LINK42|\  (FAQ N. 13) 


+-------------------+-------------------------------------------------------------------------------+-------+-------+
|Denominazione Campo|Descrizione                                                                    |Tipo   |Obbligo|
+===================+===============================================================================+=======+=======+
|Anno               |Anno di riferimento                                                            |Numero |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE404|\      |Codice identificativo del provvedimento                                        |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE405|\      |Data del provvedimento                                                         |Data   |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE406|\      |Nominativo o Ragione sociale del soggetto beneficiario del provvedimento       |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE407|\      |Indicare se si tratta di amministrazione pubblica, privato, Onlus o altro ente |Testo  |O      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE408|\      |Codice fiscale del soggetto beneficiario del provvedimento                     |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE409|\      |Partita IVA del soggetto beneficiario del provvedimento                        |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE410|\      |Oggetto del provvedimento                                                      |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE411|\      |Riferimenti della norma o titolo a base dell’attribuzione                      |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE412|\      |URL norma o titolo                                                             |Web URL|O      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE413|\      |Ufficio responsabile del provvedimento.                                        |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE414|\      |Cognome del responsabile del procedimento                                      |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE415|\      |Nome del responsabile del procedimento                                         |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE416|\      |Modalità di individuazione del soggetto beneficiario (es. aggiudicazione bando)|Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE417|\      |Importo del vantaggio economico corrisposto                                    |Numero |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE418|\      |Breve descrizione progetto allegato al provvedimento                           |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE419|\      |URL progetto                                                                   |Web URL|O      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE420|\      |Link al curriculum del soggetto beneficiario                                   |Web URL|O      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+

|

.. _h7782e36e316052235761422844d44:

#23 Elenco canoni di locazione (DEFINITIVO)
===========================================

\ |STYLE421|\ : Elenco canoni di locazione o di affitto percepiti

\ |STYLE422|\  Dataset tabellare

\ |STYLE423|\ : Mensile

Obblighi normativi: D. lgs. 33/2013, in particolare art. 30.

+-------------------+---------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                            |Tipo  |Obbligo|
+===================+=======================================================================================+======+=======+
|Anno               |Anno di riferimento                                                                    |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE424|\      |Indicare la tipologia di locazione (Attiva/Passiva)                                    |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE425|\      |Nominativo o Ragione sociale del locatario                                             |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE426|\      |Nominativo o Ragione sociale del locatore                                              |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE427|\      |Per le informazioni relative all’ubicazione dell’immobile vedere Allegato 1 - Tabella 1|Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE428|\      |Destinazione dell’immobile (es. uffici)                                                |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE429|\      |Data di decorrenza del contratto                                                       |Data  |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE430|\      |Data di scadenza del contratto                                                         |Data  |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE431|\      |Canone annuale di affitto percepito al netto delle spese                               |Numero|M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE432|\      |Altre spese non inserite nel canone annuale                                            |Numero|M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE433|\      |Canone annuale di affitto versato                                                      |Numero|M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+

|

.. _h6326371021e1b65335f1b3a15d202c:

#24 Elenco immobili di proprietà (DEFINITIVO)
=============================================

\ |STYLE434|\ : Elenco informazioni identificative degli immobili posseduti

\ |STYLE435|\  Dataset tabellare

\ |STYLE436|\ : Mensile

Obblighi normativi: D. lgs. 33/2013, in particolare art. 30.

+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                         |Tipo  |Obbligo|
+===================+====================================================================================================+======+=======+
|Ubicazione         |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                                     |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE437|\      |Denominazione dell’unità immobiliare (es. Palazzo Pirelli) o descrizione area (es. area industriale)|Testo |O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE438|\      |Indicare la natura giuridica del bene patrimoniale tra:                                             |Testo |M      |
|                   |                                                                                                    |      |       |
|                   |* disponibile                                                                                       |      |       |
|                   |                                                                                                    |      |       |
|                   |* indisponibile                                                                                     |      |       |
|                   |                                                                                                    |      |       |
|                   |* demaniale                                                                                         |      |       |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE439|\      |es. Immobile                                                                                        |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE440|\      |Codice identificativo categoria (dato catastale).                                                   |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE441|\      |Sezione (dato catastale)                                                                            |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE442|\      |Codice identificativo foglio (dato catastale)                                                       |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE443|\      |Codice identificativo mappale (dato catastale)                                                      |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE444|\      |Codice identificativo subalterno (dato catastale)                                                   |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE445|\      |Classe_catastale                                                                                    |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE446|\      |Unità di misura della consistenza (mq, mc, vani)                                                    |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE447|\      |Grandezza del bene (solo numero riferito all’unità di misura del campo precedente)                  |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE448|\      |Rendita catastale                                                                                   |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE449|\      |Destinazione d’uso del bene                                                                         |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE450|\      |Superficie del bene (espressa in metri quadrati).                                                   |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE451|\      |Valore di mercato del bene                                                                          |Numero|O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE452|\      |Data di acquisizione del bene                                                                       |Data  |O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE453|\      |Longitudine                                                                                         |Numero|O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE454|\      |Latitudine                                                                                          |Numero|O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+

|

.. _h4451d524d372a6ed467c1876264f6d:

#25 Monitoraggio procedimenti (DEFINITIVO) 
===========================================

\ |STYLE455|\ : Monitoraggio dei tempi dei procedimenti

\ |STYLE456|\  Dataset tabellare

\ |STYLE457|\ : Semestrale

+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                  |Tipo  |Obbligo|
+===================+=============================================================================================+======+=======+
|Tipologia          |Tipologia del procedimento (d’ufficio o a istanza di parte)                                  |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE458|\      |Nome del procedimento                                                                        |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE459|\      |Breve descrizione del procedimento                                                           |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE460|\      |Indicare il termine massimo di conclusione del procedimento stabilito dalla legge (in giorni)|Numero|M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE461|\      |Indicare il termine effettivo di conclusione del procedimento (in giorni)                    |Numero|M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE462|\      |Ufficio responsabile del provvedimento                                                       |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE463|\      |Indicare motivi di eventuali sospensioni o ritardi                                           |Testo |O      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+

|

.. _h132c4945185112631f3367485d57c16:

#26 Enti controllati – Società partecipate (DEFINITIVO)
=======================================================

\ |STYLE464|\ : Elenco e informazioni sulle Società partecipate

\ |STYLE465|\  Dataset tabellare

\ |STYLE466|\ : Tempestiva

+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo            |Descrizione                                                                                       |Tipo  |Obbligo|
+===============================+==================================================================================================+======+=======+
|Ente_pubblico – Ragione_Sociale|Denominazione ente                                                                                |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE467|\                  |Funzioni affidate all’Ente                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE468|\                  |.Attività svolte dall’Ente per ottemperare alle funzioni                                          |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE469|\                  |Eventuale quota di partecipazione societaria all’ente                                             |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE470|\                  |“Indeterminato” oppure scadenza prevista                                                          |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE471|\                  |Onere complessivo a qualsiasi titolo gravante per l'anno sul bilancio dell'amministrazione        |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE472|\                  |Numero dei rappresentanti dell'amministrazione negli organi di governo                            |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE473|\                  |Trattamento economico complessivo dei rappresentanti dell'amministrazione negli organi di governo |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE474|\                  |Anno di riferimento                                                                               |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE475|\                  |Risultati di bilancio dell’anno di riferimento (ultimo anno)                                      |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE476|\                  |Risultati di bilancio del penultimo anno                                                          |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE477|\                  |Risultati di bilancio del terzultimo anno                                                         |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE478|\                  |Link al sito istituzionale                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+

|

.. _h7239514f337e4b15371432716b161761:

#27 Enti controllati – Enti pubblici vigilati (DEFINITIVO)
==========================================================

\ |STYLE479|\ : Elenco e informazioni sugli Enti pubblici vigilati

\ |STYLE480|\  Dataset tabellare

\ |STYLE481|\ : Tempestiva

+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo            |Descrizione                                                                                       |Tipo  |Obbligo|
+===============================+==================================================================================================+======+=======+
|Ente_pubblico – Ragione_Sociale|Denominazione ente                                                                                |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE482|\                  |Funzioni affidate all’Ente                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE483|\                  |Attività svolte dall’Ente per ottemperare alle funzioni                                           |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE484|\                  |Eventuale quota di partecipazione societaria all’ente                                             |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE485|\                  |“Indeterminato” oppure scadenza prevista                                                          |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE486|\                  |Onere complessivo a qualsiasi titolo gravante per l'anno sul bilancio dell'amministrazione        |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE487|\                  |Numero dei rappresentanti dell'amministrazione negli organi di governo                            |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE488|\                  |Trattamento economico complessivo dei rappresentanti dell'amministrazione negli organi di governo |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE489|\                  |Anno di riferimento                                                                               |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE490|\                  |Risultati di bilancio dell’anno di riferimento (ultimo anno)                                      |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE491|\                  |Risultati di bilancio del penultimo anno                                                          |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE492|\                  |Risultati di bilancio del terzultimo anno                                                         |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE493|\                  |Link al sito istituzionale                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+

|

.. _h6057240426a371f372442d4776d7f:

#28 Enti controllati – Enti di diritto privato controllati (DEFINITIVO)
=======================================================================

\ |STYLE494|\ : Elenco e informazioni sugli Enti di diritto privato controllati

\ |STYLE495|\  Dataset tabellare

\ |STYLE496|\ : Tempestiva

+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo            |Descrizione                                                                                       |Tipo  |Obbligo|
+===============================+==================================================================================================+======+=======+
|Ente_pubblico – Ragione_Sociale|Denominazione ente                                                                                |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE497|\                  |Funzioni affidate all’Ente                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE498|\                  |.Attività svolte dall’Ente per ottemperare alle funzioni                                          |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE499|\                  |Eventuale quota di partecipazione societaria all’ente                                             |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE500|\                  |“Indeterminato” oppure scadenza prevista                                                          |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE501|\                  |Onere complessivo a qualsiasi titolo gravante per l'anno sul bilancio dell'amministrazione        |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE502|\                  |Numero dei rappresentanti dell'amministrazione negli organi di governo                            |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE503|\                  |Trattamento economico complessivo dei rappresentanti dell'amministrazione negli organi di governo |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE504|\                  |Anno di riferimento                                                                               |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE505|\                  |Risultati di bilancio dell’anno di riferimento (ultimo anno)                                      |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE506|\                  |Risultati di bilancio del penultimo anno                                                          |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE507|\                  |Risultati di bilancio del terzultimo anno                                                         |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE508|\                  |Link al sito istituzionale                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+

|

.. _h586361a7d1b58732243725f242:

#36 Provvedimenti dei dirigenti (DEFINITIVO)
============================================

\ |STYLE509|\ : Elenchi dei provvedimenti adottati dai dirigenti

\ |STYLE510|\  Dataset tabellare

\ |STYLE511|\ : Mensile

Obblighi normativi: D. lgs. 33/2013, in particolare art. 23.

Vedi \ |LINK43|\  


+-------------------+----------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                 |Tipo  |Obbligo|
+===================+============================================================================+======+=======+
|Anno               |Anno di riferimento                                                         |Numero|M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE512|\      |Indicare la tipologia di provvedimento tra le seguenti:                     |Testo |O      |
|                   |                                                                            |      |       |
|                   |#. Scelta del contraente per l'affidamento di lavori, forniture e servizi   |      |       |
|                   |                                                                            |      |       |
|                   |#. Accordi stipulati dall'amministrazione                                   |      |       |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE513|\      |Numero identificativo del provvedimento                                     |Numero|M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE514|\      |Titolo del provvedimento                                                    |Testo |M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE515|\      |Dispositivo del provvedimento                                               |Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE516|\      |Data di approvazione del provvedimento.                                     |Data  |M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE517|\      |Nome dell’ufficio proponente                                                |Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE518|\      |Eventuale spesa prevista                                                    |Numero|O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE519|\      |Riferimenti ai documenti principali contenuti nel fascicolo del procedimento|Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+

|

.. _h2c1d74277104e41780968148427e:




.. _h57b79594a60271c37774e4b797e5e68:

#37 Provvedimenti degli organi di indirizzo politico (DEFINITIVO)
=================================================================

\ |STYLE520|\ : Elenchi dei Provvedimenti degli organi di indirizzo politico

\ |STYLE521|\  Dataset tabellare

\ |STYLE522|\ : Mensile

Obblighi normativi: D. lgs. 33/2013, in particolare art. 23.

Vedi \ |LINK44|\  


+-------------------+----------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                 |Tipo  |Obbligo|
+===================+============================================================================+======+=======+
|Anno               |Anno di riferimento                                                         |Numero|M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE523|\      |Scegliere tra le due opzioni:                                               |Testo |O      |
|                   |                                                                            |      |       |
|                   |* Giunta                                                                    |      |       |
|                   |                                                                            |      |       |
|                   |* Consiglio                                                                 |      |       |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE524|\      |Indicare la tipologia di provvedimento tra le seguenti:                     |Testo |O      |
|                   |                                                                            |      |       |
|                   |#. Scelta del contraente per l'affidamento di lavori, forniture e servizi   |      |       |
|                   |                                                                            |      |       |
|                   |#. Accordi stipulati dall'amministrazione                                   |      |       |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE525|\      |Numero identificativo del provvedimento                                     |Numero|M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE526|\      |Titolo del provvedimento                                                    |Testo |M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE527|\      |Dispositivo del provvedimento                                               |Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE528|\      |Data di approvazione del provvedimento                                      |Data  |M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE529|\      |Nome dell’ufficio proponente                                                |Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE530|\      |Eventuale spesa prevista                                                    |Numero|O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE531|\      |Riferimenti ai documenti principali contenuti nel fascicolo del procedimento|Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+

|

.. _h2e6413415f50581d7a6f24c6b663027:

10.  TURISMO
************

.. _h39547c1c3b3b73196a1e2b15b6df56:

#32 Accompagnatori turistici (DEFINITIVO) 
==========================================

\ |STYLE532|\ : Elenco degli abilitati per l’esercizio della professione di accompagnatore turistico

\ |STYLE533|\  Dataset tabellare

\ |STYLE534|\ : Tempestiva

+-------------------+-----------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                    |Tipo  |Obbligo|
+===================+===============================================+======+=======+
|Comune             |Comune di riferimento                          |Testo |M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE535|\      |Anno di riferimento                            |Numero|M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE536|\      |Cognome dell’accompagnatore turistico abilitato|Testo |M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE537|\      |Nome dell’accompagnatore turistico abilitato   |Testo |M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE538|\      |Indicare la lingua conosciuta                  |Testo |M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE539|\      |Indicare la lingua conosciuta                  |Testo |O      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE540|\      |Indicare la lingua conosciuta                  |Testo |O      |
+-------------------+-----------------------------------------------+------+-------+

|

.. _h6e806e58126f423e6813804173126a5a:

#43 Flussi turistici (DEFINITIVO)
=================================

\ |STYLE541|\ : Dati statistici sui flussi turistici

\ |STYLE542|\  Dataset tabellare

\ |STYLE543|\ : Trimestrale

+-------------------+-----------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                  |Tipo  |Obbligo|
+===================+=============================================================================+======+=======+
|Anno               |Anno di riferimento                                                          |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE544|\      |Mese di riferimento                                                          |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE545|\      |Comune di riferimento                                                        |Testo |M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE546|\      |Indicare se i dati si riferiscono al settore alberghiero o extra-alberghiero |Testo |M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE547|\      |N. di arrivi di turisti italiani nel mese di riferimento                     |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE548|\      |N. di presenze di turisti italiani nel mese di riferimento                   |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE549|\      |N. di arrivi di turisti stranieri nel mese di riferimento                    |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE550|\      |N. di presenze di turisti stranieri nel mese di riferimento                  |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+

|


.. _h4d12065484b7857297a6c195c4b150:

Allegato 1
**********

Standard generali con l’indicazione dei campi relativi ad alcune informazioni.

.. _h492d313c59223e1033626dd213a121:

TABELLA 1 - UBICAZIONE
======================


+-------------------+---------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                  |Tipo |Obbligo|
+===================+=============================================+=====+=======+
|Provincia          |Provincia di riferimento (sigla)             |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE551|\      |Nome del comune dell’area                    |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE552|\      |Codice catastale del Comune                  |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE553|\      |Tipologia toponimo: Via/Piazza ecc.          |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE554|\      |Nome  Via/Piazza ecc.                        |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE555|\      |Numero civico (compresa lettera, se presente)|Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE556|\      |CAP dell’area                                |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+

|


.. _h49516427242563e30663f4813296d:

TABELLA 2 - ORARI (senza indicazione stagionalità)
==================================================


+-------------------+-------------------+-----+-------+
|Denominazione Campo|Descrizione        |Tipo |Obbligo|
+===================+===================+=====+=======+
|Lun_Apertura       |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE557|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE558|\      |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE559|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE560|\      |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE561|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE562|\      |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE563|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE564|\      |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE565|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE566|\      |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE567|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE568|\      |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE569|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+

|

.. _h3366642f254f454d623621727a177d61:

TABELLA 3 - ORARI CON STAGIONALITA’
===================================


+----------------------+-------------------+-----+-------+
|Denominazione Campo   |Descrizione        |Tipo |Obbligo|
+======================+===================+=====+=======+
|Invernale_Lun_Apertura|Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE570|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE571|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE572|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE573|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE574|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE575|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE576|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE577|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE578|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE579|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE580|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE581|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE582|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE583|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE584|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE585|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE586|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE587|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE588|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE589|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE590|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE591|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE592|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE593|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE594|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE595|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE596|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+

|


.. _h7a6e23362d711679511187c3d5b5a27:

Allegato 2
**********

.. _h266a626635674523124294953492337:

VOCABOLARIO FREQUENZE AGGIORNAMENTO
===================================

Parallelamente alla definizione degli standard relativi ai contenuti minimi dei dataset, stiamo lavorando alla definizione di un vocabolario delle frequenze di aggiornamento. 

Per quanto riguarda il paniere dei dataset qui illustrato, le frequenze di aggiornamento sono già definite nell’allegato B della DGR 7256 del 23/10/2017, ma riteniamo utile condividere anche il vocabolario da utilizzare nel caso in cui decidiate di pubblicare sul portale ulteriori dataset.

La definizione del vocabolario delle frequenze tiene conto anche di quanto previsto dallo standard DCAT-AP_IT  che fa a sua volta riferimento ad un vocabolario europeo standard:

\ |LINK45|\ 

Ecco l’elenco delle frequenze di aggiornamento individuate da specificare nei metadati del dataset:

* \ |STYLE597|\  (Dati la cui frequenza non è prevedibile, ma al verificarsi del cambiamento vengono pubblicati tempestivamente)

* \ |STYLE598|\  (Dati che vengono aggiornati in tempo reale o ogni N ore)

* \ |STYLE599|\ 

* \ |STYLE600|\  

* \ |STYLE601|\ 

* \ |STYLE602|\ 

* \ |STYLE603|\ 

* \ |STYLE604|\ 

* \ |STYLE605|\ 

* \ |STYLE606|\ 

* \ |STYLE607|\  

* \ |STYLE608|\ 

* \ |STYLE609|\ 

* \ |STYLE610|\ 

* \ |STYLE611|\ 

* \ |STYLE612|\  (Dati “storici”, che per loro natura non cambiano)

* \ |STYLE613|\  (Dati soggetti a cambiamento, ma i cui processi di aggiornamento non sono ancora definiti) 

Segue tabella di conversione con le frequenze standard per il \ |STYLE614|\ 

+----------------------------------+----------------------+
|Vocabolario www.dati.lombardia.it |Vocabolario DCAT-AP_IT|
+==================================+======================+
|Tempestiva                        |Irreg                 |
+----------------------------------+----------------------+
|Tempo reale                       |Cont                  |
+----------------------------------+----------------------+
|Giornaliera                       |Daily                 |
+----------------------------------+----------------------+
|Settimanale                       |Weekly                |
+----------------------------------+----------------------+
|Quindicinale                      |Monthly_2             |
+----------------------------------+----------------------+
|Mensile                           |Monthly               |
+----------------------------------+----------------------+
|Bimestrale                        |Bimonthly             |
+----------------------------------+----------------------+
|Trimestrale                       |Quarterly             |
+----------------------------------+----------------------+
|Quadrimestrale                    |Annual_3              |
+----------------------------------+----------------------+
|Semestrale                        |Annual_2              |
+----------------------------------+----------------------+
|Annuale                           |Annual                |
+----------------------------------+----------------------+
|Biennale                          |Biennal               |
+----------------------------------+----------------------+
|Triennale                         |Triennal              |
+----------------------------------+----------------------+
|Quinquennale                      |Other                 |
+----------------------------------+----------------------+
|Decennale                         |Other                 |
+----------------------------------+----------------------+
|Mai                               |Never                 |
+----------------------------------+----------------------+
|Non definita                      |Unknown               |
+----------------------------------+----------------------+


.. bottom of content


.. |STYLE0| replace:: **L’obiettivo del documento è quello di condividere e consolidare uno standard relativo ai contenuti minimi che ciascun dataset deve contenere.**

.. |STYLE1| replace:: **qualità**

.. |STYLE2| replace:: **completezza**

.. |STYLE3| replace:: **confronto**

.. |STYLE4| replace:: **fruibilità**

.. |STYLE5| replace:: **Ambiente**

.. |STYLE6| replace:: **Commercio**

.. |STYLE7| replace:: **Cultura**

.. |STYLE8| replace:: **Energia**

.. |STYLE9| replace:: **Mobilità e trasporti**

.. |STYLE10| replace:: **Sicurezza**

.. |STYLE11| replace:: **Statistica**

.. |STYLE12| replace:: **Territorio**

.. |STYLE13| replace:: **Trasparenza**

.. |STYLE14| replace:: **Turismo**

.. |STYLE15| replace:: **prima proposta di contenuti minimi da pubblicare**

.. |STYLE16| replace:: **contenuti mandatori (M)**

.. |STYLE17| replace:: **contenuti opzionali (O)**

.. |STYLE18| replace:: **commenti**

.. |STYLE19| replace:: **Quali formati possono avere i dati?**

.. |STYLE20| replace:: **Come scegliere i formati dei dati?**

.. |STYLE21| replace:: **ordinamento crescente/ decrescente dei dati**

.. |STYLE22| replace:: **rappresentazione “percentuale”**

.. |STYLE23| replace:: **rappresentazione geografica**

.. |STYLE24| replace:: **sistema di coordinate WGS-84 EPSG 4326**

.. |STYLE25| replace:: **Specifiche per il formato “numero” e “data**

.. |STYLE26| replace:: **Specifiche per la rappresentazione geografica**

.. |STYLE27| replace:: **NB:**

.. |STYLE28| replace:: **Per i dataset con frequenza di aggiornamento "tempestiva" occorre, almeno mensilmente, aggiornare i metadati.**

.. |STYLE29| replace:: **non cambia l'ultimo aggiornamento dei dati ma l'ultimo aggiornamento dei metadati**

.. |STYLE30| replace:: **Descrizione:**

.. |STYLE31| replace:: **Tipologia:**

.. |STYLE32| replace:: **Frequenza minima:**

.. |STYLE33| replace:: **Foglio**

.. |STYLE34| replace:: **Mappale**

.. |STYLE35| replace:: **Part_cat**

.. |STYLE36| replace:: **Area_fuoco**

.. |STYLE37| replace:: **Area_tot**

.. |STYLE38| replace:: **Vincoli_15**

.. |STYLE39| replace:: **Vincoli_10**

.. |STYLE40| replace:: **Vincoli_5**

.. |STYLE41| replace:: **Descrizione:**

.. |STYLE42| replace:: **Tipologia:**

.. |STYLE43| replace:: **Frequenza minima:**

.. |STYLE44| replace:: **Toponimo**

.. |STYLE45| replace:: **Indirizzo**

.. |STYLE46| replace:: **Area_mq**

.. |STYLE47| replace:: **Descrizione:**

.. |STYLE48| replace:: **Tipologia:**

.. |STYLE49| replace:: **Frequenza minima:**

.. |STYLE50| replace:: **Denominazione**

.. |STYLE51| replace:: **Tipologia**

.. |STYLE52| replace:: **Codice_catastale**

.. |STYLE53| replace:: **Comune**

.. |STYLE54| replace:: **Superficie_mq**

.. |STYLE55| replace:: **Superficie_prato**

.. |STYLE56| replace:: **Recinzione**

.. |STYLE57| replace:: **Giochi_Bambini**

.. |STYLE58| replace:: **Animali_ammessi**

.. |STYLE59| replace:: **Fontanelle**

.. |STYLE60| replace:: **Orari**

.. |STYLE61| replace:: **Descrizione:**

.. |STYLE62| replace:: **Tipologia:**

.. |STYLE63| replace:: **Frequenza minima:**

.. |STYLE64| replace:: **Nome_Impianto**

.. |STYLE65| replace:: **Codice_catastale**

.. |STYLE66| replace:: **Comune**

.. |STYLE67| replace:: **Comuni_serviti**

.. |STYLE68| replace:: **Recettore**

.. |STYLE69| replace:: **Altezza**

.. |STYLE70| replace:: **Indirizzo**

.. |STYLE71| replace:: **Longitude**

.. |STYLE72| replace:: **Latitude**

.. |STYLE73| replace:: **Data_avvio**

.. |STYLE74| replace:: **Descrizione:**

.. |STYLE75| replace:: **Tipologia:**

.. |STYLE76| replace:: **Frequenza minima:**

.. |STYLE77| replace:: **Macro_Categoria_Rifiuti**

.. |STYLE78| replace:: **Categoria_Rifiuti**

.. |STYLE79| replace:: **ID_Categoria_Rifiuti**

.. |STYLE80| replace:: **Modalità_Raccolta**

.. |STYLE81| replace:: **Periodo**

.. |STYLE82| replace:: **Quantità**

.. |STYLE83| replace:: **Descrizione:**

.. |STYLE84| replace:: **Tipologia:**

.. |STYLE85| replace:: **Frequenza minima:**

.. |STYLE86| replace:: **Codice_Pratica**

.. |STYLE87| replace:: **Richiedente**

.. |STYLE88| replace:: **Protocollo**

.. |STYLE89| replace:: **Oggetto_Richiesta**

.. |STYLE90| replace:: **Data_Richiesta**

.. |STYLE91| replace:: **Link_pratica**

.. |STYLE92| replace:: **Descrizione:**

.. |STYLE93| replace:: **Tipologia:**

.. |STYLE94| replace:: **Frequenza minima:**

.. |STYLE95| replace:: **Ubicazione**

.. |STYLE96| replace:: **Tipologia**

.. |STYLE97| replace:: **Superficie**

.. |STYLE98| replace:: **Superficie_Altro**

.. |STYLE99| replace:: **Orari**

.. |STYLE100| replace:: **Longitude**

.. |STYLE101| replace:: **Latitude**

.. |STYLE102| replace:: **Descrizione**

.. |STYLE103| replace:: **Tipologia:**

.. |STYLE104| replace:: **Frequenza minima**

.. |STYLE105| replace:: **Ubicazione**

.. |STYLE106| replace:: **Tipo_Esercizio**

.. |STYLE107| replace:: **Tipo_Somministrazione**

.. |STYLE108| replace:: **Modalità_Somministrazione**

.. |STYLE109| replace:: **Superficie**

.. |STYLE110| replace:: **WiFi**

.. |STYLE111| replace:: **Longitude**

.. |STYLE112| replace:: **Latitude**

.. |STYLE113| replace:: **Orari**

.. |STYLE114| replace:: **Descrizione**

.. |STYLE115| replace:: **Tipologia:**

.. |STYLE116| replace:: **Frequenza minima**

.. |STYLE117| replace:: **Periodo_Rif**

.. |STYLE118| replace:: **Denominazione**

.. |STYLE119| replace:: **Tipo**

.. |STYLE120| replace:: **N_Edizione**

.. |STYLE121| replace:: **Descrizione**

.. |STYLE122| replace:: **Data_Inizio**

.. |STYLE123| replace:: **Ora_Inizio**

.. |STYLE124| replace:: **Data_Fine**

.. |STYLE125| replace:: **Ora_Fine**

.. |STYLE126| replace:: **Sito_Web**

.. |STYLE127| replace:: **Programma**

.. |STYLE128| replace:: **Nome_Organizzatore**

.. |STYLE129| replace:: **Email_Organizzatore**

.. |STYLE130| replace:: **Telefono_Organizzatore**

.. |STYLE131| replace:: **Gratuito**

.. |STYLE132| replace:: **Prezzo**

.. |STYLE133| replace:: **Longitude**

.. |STYLE134| replace:: **Latitude**

.. |STYLE135| replace:: **Descrizione**

.. |STYLE136| replace:: **Tipologia:**

.. |STYLE137| replace:: **Frequenza minima**

.. |STYLE138| replace:: **Nome**

.. |STYLE139| replace:: **Descrizione**

.. |STYLE140| replace:: **Tipologia**

.. |STYLE141| replace:: **Ubicazione**

.. |STYLE142| replace:: **Email**

.. |STYLE143| replace:: **Telefono**

.. |STYLE144| replace:: **Sito_web**

.. |STYLE145| replace:: **Note**

.. |STYLE146| replace:: **Longitude**

.. |STYLE147| replace:: **Latitude**

.. |STYLE148| replace:: **Descrizione**

.. |STYLE149| replace:: **Tipologia:**

.. |STYLE150| replace:: **Frequenza minima**

.. |STYLE151| replace:: **Ubicazione**

.. |STYLE152| replace:: **Telefono**

.. |STYLE153| replace:: **Email**

.. |STYLE154| replace:: **Descrizione**

.. |STYLE155| replace:: **Tipologia:**

.. |STYLE156| replace:: **Frequenza minima**

.. |STYLE157| replace:: **Descrizione**

.. |STYLE158| replace:: **Tipologia:**

.. |STYLE159| replace:: **Frequenza minima**

.. |STYLE160| replace:: **Periodo**

.. |STYLE161| replace:: **Dettagli**

.. |STYLE162| replace:: **Descrizione**

.. |STYLE163| replace:: **Tipologia:**

.. |STYLE164| replace:: **Frequenza minima**

.. |STYLE165| replace:: **Tipo**

.. |STYLE166| replace:: **Orari**

.. |STYLE167| replace:: **Deroghe**

.. |STYLE168| replace:: **Longitude**

.. |STYLE169| replace:: **Latitude**

.. |STYLE170| replace:: **Link**

.. |STYLE171| replace:: **Descrizione**

.. |STYLE172| replace:: **Tipologia:**

.. |STYLE173| replace:: **Frequenza minima**

.. |STYLE174| replace:: **Tipologia**

.. |STYLE175| replace:: **Ubicazione**

.. |STYLE176| replace:: **Orari**

.. |STYLE177| replace:: **Longitude**

.. |STYLE178| replace:: **Latitude**

.. |STYLE179| replace:: **Gratuito**

.. |STYLE180| replace:: **Descrizione**

.. |STYLE181| replace:: **Tipologia:**

.. |STYLE182| replace:: **Frequenza minima**

.. |STYLE183| replace:: **Descr**

.. |STYLE184| replace:: **Tipologia**

.. |STYLE185| replace:: **Sede**

.. |STYLE186| replace:: **Fondo**

.. |STYLE187| replace:: **Lung**

.. |STYLE188| replace:: **Larg**

.. |STYLE189| replace:: **Direzione**

.. |STYLE190| replace:: **Stato**

.. |STYLE191| replace:: **Ambito**

.. |STYLE192| replace:: **Descrizione**

.. |STYLE193| replace:: **Tipologia:**

.. |STYLE194| replace:: **Frequenza minima**

.. |STYLE195| replace:: **Tipo_Area**

.. |STYLE196| replace:: **Toponimo**

.. |STYLE197| replace:: **Indirizzo**

.. |STYLE198| replace:: **Descrizione**

.. |STYLE199| replace:: **Tipologia:**

.. |STYLE200| replace:: **Frequenza minima**

.. |STYLE201| replace:: **Toponimo**

.. |STYLE202| replace:: **Indirizzo**

.. |STYLE203| replace:: **Descrizione**

.. |STYLE204| replace:: **Tipologia:**

.. |STYLE205| replace:: **Frequenza minima**

.. |STYLE206| replace:: **Ubicazione**

.. |STYLE207| replace:: **Latitude**

.. |STYLE208| replace:: **Longitude**

.. |STYLE209| replace:: **N_Bici**

.. |STYLE210| replace:: **Note**

.. |STYLE211| replace:: **Descrizione**

.. |STYLE212| replace:: **Tipologia:**

.. |STYLE213| replace:: **Frequenza minima**

.. |STYLE214| replace:: **Ubicazione**

.. |STYLE215| replace:: **Telefono**

.. |STYLE216| replace:: **Email**

.. |STYLE217| replace:: **Descrizione**

.. |STYLE218| replace:: **Tipologia:**

.. |STYLE219| replace:: **Frequenza minima**

.. |STYLE220| replace:: **Ubicazione**

.. |STYLE221| replace:: **Stalli**

.. |STYLE222| replace:: **Longitude**

.. |STYLE223| replace:: **Latitude**

.. |STYLE224| replace:: **Descrizione**

.. |STYLE225| replace:: **Tipologia:**

.. |STYLE226| replace:: **Frequenza minima**

.. |STYLE227| replace:: **Ubicazione**

.. |STYLE228| replace:: **KW**

.. |STYLE229| replace:: **Modalità_Utilizzo**

.. |STYLE230| replace:: **Tipo_Presa**

.. |STYLE231| replace:: **Veicoli**

.. |STYLE232| replace:: **Data_Attivazione**

.. |STYLE233| replace:: **Longitude**

.. |STYLE234| replace:: **Latitude**

.. |STYLE235| replace:: **Descrizione**

.. |STYLE236| replace:: **Tipologia**

.. |STYLE237| replace:: **Frequenza minima**

.. |STYLE238| replace:: **Data**

.. |STYLE239| replace:: **Ora**

.. |STYLE240| replace:: **Località**

.. |STYLE241| replace:: **Natura_Incidente**

.. |STYLE242| replace:: **N_Illesi**

.. |STYLE243| replace:: **N_Feriti**

.. |STYLE244| replace:: **N_Morti**

.. |STYLE245| replace:: **Pedoni**

.. |STYLE246| replace:: **Velocipedi**

.. |STYLE247| replace:: **Ciclomotori_Motocicli**

.. |STYLE248| replace:: **Mezzi_pesanti**

.. |STYLE249| replace:: **Longitude**

.. |STYLE250| replace:: **Latitude**

.. |STYLE251| replace:: **Descrizione**

.. |STYLE252| replace:: **Tipologia:**

.. |STYLE253| replace:: **Frequenza minima**

.. |STYLE254| replace:: **Tipo_Infrazione**

.. |STYLE255| replace:: **Normativa**

.. |STYLE256| replace:: **Art.**

.. |STYLE257| replace:: **Data**

.. |STYLE258| replace:: **Tipo_Veicolo**

.. |STYLE259| replace:: **Ubicazione**

.. |STYLE260| replace:: **N_Sanzioni**

.. |STYLE261| replace:: **Longitude**

.. |STYLE262| replace:: **Latitude**

.. |STYLE263| replace:: **Descrizione**

.. |STYLE264| replace:: **Tipologia:**

.. |STYLE265| replace:: **Frequenza minima**

.. |STYLE266| replace:: **Provvedimento**

.. |STYLE267| replace:: **Controlli**

.. |STYLE268| replace:: **Verbali**

.. |STYLE269| replace:: **Descrizione**

.. |STYLE270| replace:: **Tipologia:**

.. |STYLE271| replace:: **Frequenza minima**

.. |STYLE272| replace:: **Tipo**

.. |STYLE273| replace:: **Controlli**

.. |STYLE274| replace:: **Verbali**

.. |STYLE275| replace:: **Descrizione**

.. |STYLE276| replace:: **Tipologia:**

.. |STYLE277| replace:: **Frequenza minima**

.. |STYLE278| replace:: **Tornata_elettorale**

.. |STYLE279| replace:: **Collegio_elettorale**

.. |STYLE280| replace:: **Sezione**

.. |STYLE281| replace:: **Soggetto_votato**

.. |STYLE282| replace:: **Voto**

.. |STYLE283| replace:: **N_Voti**

.. |STYLE284| replace:: **Descrizione**

.. |STYLE285| replace:: **Tipologia:**

.. |STYLE286| replace:: **Frequenza minima**

.. |STYLE287| replace:: **Tornata_elettorale**

.. |STYLE288| replace:: **Collegio_elettorale**

.. |STYLE289| replace:: **Sezione**

.. |STYLE290| replace:: **Soggetto_votato**

.. |STYLE291| replace:: **Voto**

.. |STYLE292| replace:: **N_Voti**

.. |STYLE293| replace:: **Descrizione**

.. |STYLE294| replace:: **Tipologia:**

.. |STYLE295| replace:: **Frequenza minima**

.. |STYLE296| replace:: **Tornata_elettorale**

.. |STYLE297| replace:: **Collegio_elettorale**

.. |STYLE298| replace:: **Sezione**

.. |STYLE299| replace:: **Soggetto_votato**

.. |STYLE300| replace:: **Voto**

.. |STYLE301| replace:: **N_Voti**

.. |STYLE302| replace:: **Descrizione**

.. |STYLE303| replace:: **Tipologia:**

.. |STYLE304| replace:: **Frequenza minima**

.. |STYLE305| replace:: **Tornata_Elettorale**

.. |STYLE306| replace:: **Tipo_Elezione**

.. |STYLE307| replace:: **Soggetto_votato**

.. |STYLE308| replace:: **Collegio_elettorale**

.. |STYLE309| replace:: **Sezione**

.. |STYLE310| replace:: **Voto**

.. |STYLE311| replace:: **N_Voti**

.. |STYLE312| replace:: **Descrizione**

.. |STYLE313| replace:: **Tipologia:**

.. |STYLE314| replace:: **Frequenza minima**

.. |STYLE315| replace:: **Condizione**

.. |STYLE316| replace:: **Maschi**

.. |STYLE317| replace:: **Femmine**

.. |STYLE318| replace:: **Descrizione**

.. |STYLE319| replace:: **Tipologia:**

.. |STYLE320| replace:: **Frequenza minima**

.. |STYLE321| replace:: **Indirizzo**

.. |STYLE322| replace:: **Località**

.. |STYLE323| replace:: **S_marcia**

.. |STYLE324| replace:: **Civico_inizio**

.. |STYLE325| replace:: **Civico_fine**

.. |STYLE326| replace:: **Descrizione**

.. |STYLE327| replace:: **Tipologia:**

.. |STYLE328| replace:: **Frequenza minima**

.. |STYLE329| replace:: **Nome_Toponimo**

.. |STYLE330| replace:: **Codice_Toponimo**

.. |STYLE331| replace:: **Storico**

.. |STYLE332| replace:: **Descrizione**

.. |STYLE333| replace:: **Tipologia:**

.. |STYLE334| replace:: **Frequenza minima**

.. |STYLE335| replace:: **Nome_Toponimo**

.. |STYLE336| replace:: **Numero**

.. |STYLE337| replace:: **Subalterno**

.. |STYLE338| replace:: **CAP**

.. |STYLE339| replace:: **Sezione_ISTAT**

.. |STYLE340| replace:: **Longitude**

.. |STYLE341| replace:: **Latitude**

.. |STYLE342| replace:: **Descrizione**

.. |STYLE343| replace:: **Tipologia:**

.. |STYLE344| replace:: **Frequenza minima**

.. |STYLE345| replace:: **Indirizzo**

.. |STYLE346| replace:: **Descrizione**

.. |STYLE347| replace:: **Data_Inizio**

.. |STYLE348| replace:: **Data_Fine**

.. |STYLE349| replace:: **Descrizione**

.. |STYLE350| replace:: **Tipologia:**

.. |STYLE351| replace:: **Frequenza minima**

.. |STYLE352| replace:: **ID_Accesso**

.. |STYLE353| replace:: **Tipologia_Accesso**

.. |STYLE354| replace:: **Sito**

.. |STYLE355| replace:: **Attivo**

.. |STYLE356| replace:: **Codice**

.. |STYLE357| replace:: **Longitude**

.. |STYLE358| replace:: **Latitude**

.. |STYLE359| replace:: **Raggio_Copertura_m**

.. |STYLE360| replace:: **Descrizione**

.. |STYLE361| replace:: **Tipologia:**

.. |STYLE362| replace:: **Frequenza minima**

.. |STYLE363| replace:: **Comune**

.. |STYLE364| replace:: **Toponimo**

.. |STYLE365| replace:: **Indirizzo**

.. |STYLE366| replace:: **Area_mq**

.. |STYLE367| replace:: **Fontane**

.. |STYLE368| replace:: **Attrezzi**

.. |STYLE369| replace:: **Panchine**

.. |STYLE370| replace:: **Descrizione**

.. |STYLE371| replace:: **Tipologia:**

.. |STYLE372| replace:: **Frequenza minima**

.. |STYLE373| replace:: **Tipologia**

.. |STYLE374| replace:: **ID_Istanza**

.. |STYLE375| replace:: **Data_Istanza**

.. |STYLE376| replace:: **Protocollo**

.. |STYLE377| replace:: **N_Provvedimento**

.. |STYLE378| replace:: **Data_Provvedimento**

.. |STYLE379| replace:: **Richiedente**

.. |STYLE380| replace:: **\***

.. |STYLE381| replace:: **Descrizione_ Intervento**

.. |STYLE382| replace:: **Codice_ecografico**

.. |STYLE383| replace:: **Descrizione**

.. |STYLE384| replace:: **Tipologia:**

.. |STYLE385| replace:: **Frequenza minima**

.. |STYLE386| replace:: **Tipologia**

.. |STYLE387| replace:: **Ubicazione**

.. |STYLE388| replace:: **Superficie_mq**

.. |STYLE389| replace:: **Assegnatario**

.. |STYLE390| replace:: **Progetto**

.. |STYLE391| replace:: **Destinazione_d’uso**

.. |STYLE392| replace:: **Atto_Concessione**

.. |STYLE393| replace:: **Data**

.. |STYLE394| replace:: **Durata_Anni**

.. |STYLE395| replace:: **Descrizione**

.. |STYLE396| replace:: **Tipologia:**

.. |STYLE397| replace:: **Frequenza minima**

.. |STYLE398| replace:: **Tipologia**

.. |STYLE399| replace:: **Ubicazione**

.. |STYLE400| replace:: **Telefono**

.. |STYLE401| replace:: **Descrizione**

.. |STYLE402| replace:: **Tipologia:**

.. |STYLE403| replace:: **Frequenza minima**

.. |STYLE404| replace:: **Numero_Provvedimento**

.. |STYLE405| replace:: **Data**

.. |STYLE406| replace:: **Beneficiario**

.. |STYLE407| replace:: **Tipologia_Beneficiario**

.. |STYLE408| replace:: **Codice_fiscale**

.. |STYLE409| replace:: **Partita_IVA**

.. |STYLE410| replace:: **Oggetto**

.. |STYLE411| replace:: **Norma_Titolo**

.. |STYLE412| replace:: **Link_Norma_Titolo**

.. |STYLE413| replace:: **Ufficio**

.. |STYLE414| replace:: **Cognome_Responsabile**

.. |STYLE415| replace:: **Nome_Responsabile**

.. |STYLE416| replace:: **Modalità**

.. |STYLE417| replace:: **Importo**

.. |STYLE418| replace:: **Progetto**

.. |STYLE419| replace:: **Link_Progetto**

.. |STYLE420| replace:: **Curriculum**

.. |STYLE421| replace:: **Descrizione**

.. |STYLE422| replace:: **Tipologia:**

.. |STYLE423| replace:: **Frequenza minima**

.. |STYLE424| replace:: **Tipologia_Locazione**

.. |STYLE425| replace:: **Locatario**

.. |STYLE426| replace:: **Locatore**

.. |STYLE427| replace:: **Ubicazione**

.. |STYLE428| replace:: **Destinazione**

.. |STYLE429| replace:: **Data_Inizio_Contratto**

.. |STYLE430| replace:: **Data_Fine_Contratto**

.. |STYLE431| replace:: **Canone_percepito**

.. |STYLE432| replace:: **Spese_accessorie**

.. |STYLE433| replace:: **Canone_versato**

.. |STYLE434| replace:: **Descrizione**

.. |STYLE435| replace:: **Tipologia:**

.. |STYLE436| replace:: **Frequenza minima**

.. |STYLE437| replace:: **Descrizione**

.. |STYLE438| replace:: **Natura_giuridica**

.. |STYLE439| replace:: **Tipologia_Bene**

.. |STYLE440| replace:: **Categoria_catastale**

.. |STYLE441| replace:: **Sezione**

.. |STYLE442| replace:: **Foglio**

.. |STYLE443| replace:: **Mappale**

.. |STYLE444| replace:: **Subalterno**

.. |STYLE445| replace:: **Classe**

.. |STYLE446| replace:: **Unità**

.. |STYLE447| replace:: **Consistenza**

.. |STYLE448| replace:: **Rendita**

.. |STYLE449| replace:: **Destinazione**

.. |STYLE450| replace:: **Superficie**

.. |STYLE451| replace:: **Valore**

.. |STYLE452| replace:: **Data_Acquisizione**

.. |STYLE453| replace:: **Longitude**

.. |STYLE454| replace:: **Latitude**

.. |STYLE455| replace:: **Descrizione**

.. |STYLE456| replace:: **Tipologia:**

.. |STYLE457| replace:: **Frequenza minima**

.. |STYLE458| replace:: **Titolo**

.. |STYLE459| replace:: **Descrizione**

.. |STYLE460| replace:: **Termine_massimo**

.. |STYLE461| replace:: **Tempi_effettivi**

.. |STYLE462| replace:: **Ufficio_Responsabile**

.. |STYLE463| replace:: **Note**

.. |STYLE464| replace:: **Descrizione**

.. |STYLE465| replace:: **Tipologia:**

.. |STYLE466| replace:: **Frequenza minima**

.. |STYLE467| replace:: **Funzioni_attribuite**

.. |STYLE468| replace:: **Attività_svolte**

.. |STYLE469| replace:: **Quota_Partecipazione**

.. |STYLE470| replace:: **Durata_Impegno**

.. |STYLE471| replace:: **Onere_Impegno**

.. |STYLE472| replace:: **Numero_Rappresentanti**

.. |STYLE473| replace:: **Trattamento_economico**

.. |STYLE474| replace:: **Ultimo_anno**

.. |STYLE475| replace:: **Risultati_Bilancio_Ultimo_anno**

.. |STYLE476| replace:: **Risultati_Bilancio_Penultimo_anno**

.. |STYLE477| replace:: **Risultati_Bilancio_Terzultimo_anno**

.. |STYLE478| replace:: **Sito_istituzionale**

.. |STYLE479| replace:: **Descrizione**

.. |STYLE480| replace:: **Tipologia:**

.. |STYLE481| replace:: **Frequenza minima**

.. |STYLE482| replace:: **Funzioni_attribuite**

.. |STYLE483| replace:: **Attività_svolte**

.. |STYLE484| replace:: **Quota_Partecipazione**

.. |STYLE485| replace:: **Durata_Impegno**

.. |STYLE486| replace:: **Onere_Impegno**

.. |STYLE487| replace:: **Numero_Rappresentanti**

.. |STYLE488| replace:: **Trattamento_economico**

.. |STYLE489| replace:: **Ultimo_anno**

.. |STYLE490| replace:: **Risultati_Bilancio_Ultimo_anno**

.. |STYLE491| replace:: **Risultati_Bilancio_Penultimo_anno**

.. |STYLE492| replace:: **Risultati_Bilancio_Terzultimo_anno**

.. |STYLE493| replace:: **Sito_istituzionale**

.. |STYLE494| replace:: **Descrizione**

.. |STYLE495| replace:: **Tipologia:**

.. |STYLE496| replace:: **Frequenza minima**

.. |STYLE497| replace:: **Funzioni_attribuite**

.. |STYLE498| replace:: **Attività_svolte**

.. |STYLE499| replace:: **Quota_Partecipazione**

.. |STYLE500| replace:: **Durata_Impegno**

.. |STYLE501| replace:: **Onere_Impegno**

.. |STYLE502| replace:: **Numero_Rappresentanti**

.. |STYLE503| replace:: **Trattamento_economico**

.. |STYLE504| replace:: **Ultimo_anno**

.. |STYLE505| replace:: **Risultati_Bilancio_Ultimo_anno**

.. |STYLE506| replace:: **Risultati_Bilancio_Penultimo_anno**

.. |STYLE507| replace:: **Risultati_Bilancio_Terzultimo_anno**

.. |STYLE508| replace:: **Sito_istituzionale**

.. |STYLE509| replace:: **Descrizione**

.. |STYLE510| replace:: **Tipologia:**

.. |STYLE511| replace:: **Frequenza minima**

.. |STYLE512| replace:: **Tipologia_ Provvedimento**

.. |STYLE513| replace:: **Numero_ Provvedimento**

.. |STYLE514| replace:: **Oggetto**

.. |STYLE515| replace:: **Contenuto**

.. |STYLE516| replace:: **Data_Approvazione**

.. |STYLE517| replace:: **Ufficio_proponente**

.. |STYLE518| replace:: **Spesa_prevista**

.. |STYLE519| replace:: **Estremi_Documenti_ Fascicolo**

.. |STYLE520| replace:: **Descrizione**

.. |STYLE521| replace:: **Tipologia:**

.. |STYLE522| replace:: **Frequenza minima**

.. |STYLE523| replace:: **Organo**

.. |STYLE524| replace:: **Tipologia_ Provvedimento**

.. |STYLE525| replace:: **Numero_ Provvedimento**

.. |STYLE526| replace:: **Oggetto**

.. |STYLE527| replace:: **Contenuto**

.. |STYLE528| replace:: **Data_Approvazione**

.. |STYLE529| replace:: **Ufficio proponente**

.. |STYLE530| replace:: **Spesa_prevista**

.. |STYLE531| replace:: **Estremi_Documenti_ Fascicolo**

.. |STYLE532| replace:: **Descrizione**

.. |STYLE533| replace:: **Tipologia:**

.. |STYLE534| replace:: **Frequenza minima**

.. |STYLE535| replace:: **Anno**

.. |STYLE536| replace:: **Cognome**

.. |STYLE537| replace:: **Nome**

.. |STYLE538| replace:: **Lingua 1**

.. |STYLE539| replace:: **Lingua 2**

.. |STYLE540| replace:: **Lingua n**

.. |STYLE541| replace:: **Descrizione**

.. |STYLE542| replace:: **Tipologia:**

.. |STYLE543| replace:: **Frequenza minima**

.. |STYLE544| replace:: **Mese**

.. |STYLE545| replace:: **Comune**

.. |STYLE546| replace:: **Settore**

.. |STYLE547| replace:: **Arrivi_italiani**

.. |STYLE548| replace:: **Presenze_italiani**

.. |STYLE549| replace:: **Arrivi_stranieri**

.. |STYLE550| replace:: **Presenze_stranieri**

.. |STYLE551| replace:: **Comune**

.. |STYLE552| replace:: **Codice_catastale**

.. |STYLE553| replace:: **Toponimo**

.. |STYLE554| replace:: **Indirizzo**

.. |STYLE555| replace:: **Civico**

.. |STYLE556| replace:: **CAP**

.. |STYLE557| replace:: **Lun_Chiusura**

.. |STYLE558| replace:: **Mar_Apertura**

.. |STYLE559| replace:: **Mar_Chiusura**

.. |STYLE560| replace:: **Mer_Apertura**

.. |STYLE561| replace:: **Mer_Chiusura**

.. |STYLE562| replace:: **Gio_Apertura**

.. |STYLE563| replace:: **Gio_Chiusura**

.. |STYLE564| replace:: **Ven_Apertura**

.. |STYLE565| replace:: **Ven_Chiusura**

.. |STYLE566| replace:: **Sab_Apertura**

.. |STYLE567| replace:: **Sab_Chiusura**

.. |STYLE568| replace:: **Dom_Apertura**

.. |STYLE569| replace:: **Dom_Chiusura**

.. |STYLE570| replace:: **Invernale_Lun_Chiusura**

.. |STYLE571| replace:: **Invernale_Mar_Apertura**

.. |STYLE572| replace:: **Invernale_Mar_Chiusura**

.. |STYLE573| replace:: **Invernale_Mer_Apertura**

.. |STYLE574| replace:: **Invernale_Mer_Chiusura**

.. |STYLE575| replace:: **Invernale_Gio_Apertura**

.. |STYLE576| replace:: **Invernale_Gio_Chiusura**

.. |STYLE577| replace:: **Invernale_Ven_Apertura**

.. |STYLE578| replace:: **Invernale_Ven_Chiusura**

.. |STYLE579| replace:: **Invernale_Sab_Apertura**

.. |STYLE580| replace:: **Invernale_Sab_Chiusura**

.. |STYLE581| replace:: **Invernale_Dom_Apertura**

.. |STYLE582| replace:: **Invernale_Dom_Chiusura**

.. |STYLE583| replace:: **Estivo_Lun_Apertura**

.. |STYLE584| replace:: **Estivo_Lun_Chiusura**

.. |STYLE585| replace:: **Estivo_Mar_Apertura**

.. |STYLE586| replace:: **Estivo_Mar_Chiusura**

.. |STYLE587| replace:: **Estivo_Mer_Apertura**

.. |STYLE588| replace:: **Estivo_Mer_Chiusura**

.. |STYLE589| replace:: **Estivo_Gio_Apertura**

.. |STYLE590| replace:: **Estivo_Gio_Chiusura**

.. |STYLE591| replace:: **Estivo_Ven_Apertura**

.. |STYLE592| replace:: **Estivo_Ven_Chiusura**

.. |STYLE593| replace:: **Estivo_Sab_Apertura**

.. |STYLE594| replace:: **Estivo_Sab_Chiusura**

.. |STYLE595| replace:: **Estivo_Dom_Apertura**

.. |STYLE596| replace:: **Estivo_Dom_Chiusura**

.. |STYLE597| replace:: **Tempestiva**

.. |STYLE598| replace:: **Tempo reale**

.. |STYLE599| replace:: **Giornaliera**

.. |STYLE600| replace:: **Settimanale**

.. |STYLE601| replace:: **Quindicinale**

.. |STYLE602| replace:: **Mensile**

.. |STYLE603| replace:: **Bimestrale**

.. |STYLE604| replace:: **Trimestrale**

.. |STYLE605| replace:: **Quadrimestrale**

.. |STYLE606| replace:: **Semestrale**

.. |STYLE607| replace:: **Annuale**

.. |STYLE608| replace:: **Biennale**

.. |STYLE609| replace:: **Triennale**

.. |STYLE610| replace:: **Quinquennale**

.. |STYLE611| replace:: **Decennale**

.. |STYLE612| replace:: **Mai**

.. |STYLE613| replace:: **Non definita**

.. |STYLE614| replace:: **DCAT-AP_IT**


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

