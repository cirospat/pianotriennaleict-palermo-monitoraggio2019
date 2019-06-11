
.. _h3b9431e3a511972f35d463f382d2:

Definizione Standard per il paniere di dataset degli Enti Locali
################################################################


.. toctree::  
    :maxdepth: 4
    :caption: Definizione standard paniere

    paniere_dataset_degli_enti_locali

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

.. _h1c3547b27524222165e713f566d6446:

Quali formati possono avere i dati?
===================================

* Numero

* Testo

* Web URL

* Booleano (spunta)

* Data

* Valuta (sconsigliato)

* Percentuale

* Coppia di coordinate geografiche (location)

.. _h684876693261113965665f736c5c7979:

Come scegliere i formati dei dati?
==================================

La piattaforma \ |LINK1|\  ingloba una serie di funzionalità avanzate sui dataset di tipo tabellare (Datasets), che permette di aggiungere funzionalità fruibili direttamente on-line, quali ad esempio l’ordinamento crescente/decrescente, link ad un elemento esterno e altro.

Per permettere l’\ |STYLE8|\ , è necessario scegliere un formato «ordinabile» (numero,data).

Per una \ |STYLE9|\ , occorre scegliere un numero con il punto come separatore dei decimali

Per una \ |STYLE10|\ , occorre inserire una coppia di dati, in formato numerico e con \ |STYLE11|\  (ad es. 46.4039704°, 9.3668236°), dove i numeri dovranno avere un punto come separatore. Un campo conterrà la latitudine e l’altro la longitudine: questi due campi popoleranno una colonna di tipo “location” che verrà usata per creare una vista derivata di tipo «mappa».

.. _h7b393b78722a50605c7c69481ba4631:

Specifiche per il formato “numero” e “data”
===========================================

La piattaforma \ |LINK2|\  è costruita con tutti i tipi di formattazione di date e numeri in uso negli USA secondo le specifiche ISO 8601.

Per ovviare ad inconvenienti di rappresentazione, è importante che i numeri contenuti nel dataset non presentino separatori delle migliaia e che i decimali vengano inseriti con il punto come segno separatore.

La visualizzazione finale potrà comunque essere modificata dall’interfaccia utente.

.. _h7f654f4a5e732221d7282b7a6f2e:

Specifiche per la rappresentazione geografica
=============================================

Per la rappresentazione geografica, è possibile:

#. caricare uno shapefile come allegato

#. importare uno shapefile. Questa opzione consente di:

* visualizzare i dati su mappa

* scaricare i dati in diversi formati

* utilizzare le API

Per la specifica degli shapefile fare riferimento a \ |LINK3|\ 

\ |STYLE12|\  Se si utilizza un sistema di coordinate diverso dal WGS-84, occorre specificare questa informazione e includere il sistema utilizzato nello shapefile.

.. _h2591956d562d53487858431c49e1f:

FREQUENZA DI AGGIORNAMENTO TEMPESTIVA
*************************************

\ |STYLE13|\ 

Anche se i dati non cambiano, occorre quindi specificare nei metadati che i dati pubblicati sono ancora validi: in questo caso, \ |STYLE14|\ . 

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

\ |STYLE15|\  Mappa e scheda delle aree percorse da incendi 

\ |STYLE16|\  Dataset geografico (Shapefile)

\ |STYLE17|\  Mensile

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
|\ |STYLE18|\       |Foglio in cui è presente la particella percorsa dal fuoco nella sua totalità o solo parzialmente                                                                                                                                                                                              |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE19|\       |Mappale in cui è presente la particella percorsa dal fuoco nella sua totalità o solo parzialmente                                                                                                                                                                                             |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE20|\       |Particella catastale della zona interessata                                                                                                                                                                                                                                                   |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE21|\       |Area della particella percorsa dal fuoco (mq)                                                                                                                                                                                                                                                 |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE22|\       |Area totale della particella (mq)                                                                                                                                                                                                                                                             |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE23|\       |Indicare se esiste il vincolo (15 anni) che impone il mantenimento della destinazione d’uso preesistente all’incendio impedendone la modifica (SI/NO)                                                                                                                                         |Testo |O      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE24|\       |Indicare se è vietata (vincolo 10 anni) la realizzazione di edifici nonché di strutture e infrastrutture finalizzate ad insediamenti civili ed attività produttive e il divieto di pascolo e di caccia per 10 anni, limitatamente ai soprassuoli delle zone boscate percorsi dal fuoco (SI/NO)|Testo |O      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE25|\       |Indicare se esiste il divieto (vincolo 5 anni) di attività di rimboschimento e di ingegneria ambientale sostenute con risorse finanziarie pubbliche (SI/NO)                                                                                                                                   |Testo |O      |
+-------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+

.. _h73633d4a4c4c22737a3215b39c2b3b:

#17     Aree Verdi (DEFINITIVO)
-------------------------------

\ |STYLE26|\  Elenco delle aree verdi del territorio 

\ |STYLE27|\  Dataset geografico (Shapefile)

\ |STYLE28|\  Tempestiva

Esempio 1: \ |LINK7|\ 

Esempio 2: \ |LINK8|\  


+-------------------+-------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                      |Tipo  |Obbligo|
+===================+=================================================+======+=======+
|Denom              |Nome dell’area o descrizione                     |Testo |M      |
+-------------------+-------------------------------------------------+------+-------+
|\ |STYLE29|\       |Via/piazza, ecc.                                 |Testo |M      |
+-------------------+-------------------------------------------------+------+-------+
|\ |STYLE30|\       |Nome della via/piazza                            |Testo |M      |
+-------------------+-------------------------------------------------+------+-------+
|\ |STYLE31|\       |Superficie dell’area (espressa in metri quadrati)|Numero|M      |
+-------------------+-------------------------------------------------+------+-------+

.. _h534b1577195b553752123805a281950:

#18     Aree Verdi Informazioni (DEFINITIVO)
--------------------------------------------

\ |STYLE32|\  Informazioni sulle aree verdi

\ |STYLE33|\  Dataset tabellare

\ |STYLE34|\  Tempestiva

NOTA: In seguito alle segnalazioni degli Enti è stato creato un tracciato che contiene informazioni relative alle aree verdi comunali e sovracomunali.


+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo  |Obbligo                      |
+===================+==========================================================================================================================================+======+=============================+
|Anno               |Anno di riferimento                                                                                                                       |Numero|M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE35|\       |Nome dell’area o descrizione                                                                                                              |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE36|\       |Tipologia di area (Comunale/Sovracomunale)                                                                                                |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE37|\       |Codice catastale del comune o dei comuni in cui è ubicata l’area, inserendo tra l’uno e l’altro il separatore pipe                        |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE38|\       |Nome del comune o dei comuni in cui è ubicata l’area, inserendo tra l’uno e l’altro il separatore pipe                                    |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE39|\       |Superficie dell’area (espressa in metri quadrati)                                                                                         |Numero|M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE40|\       |Superficie a prato (espressa in metri quadrati)                                                                                           |Numero|O                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE41|\       |Presenza di recinzione (SI/NO/Non applicabile)                                                                                            |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE42|\       |Presenza di aree giochi per bambini (SI/NO/Non applicabile)                                                                               |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE43|\       |Permesso di introdurre animali (SI/NO/Non applicabile)                                                                                    |Testo |M                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE44|\       |Numero di fontanelle presenti                                                                                                             |Numero|O                            |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+
|\ |STYLE45|\       |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo |M (se presente la recinzione)|
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-----------------------------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h6c466e2d2d97084e145847153214d:

#34 Elenco degli impianti di depurazione (DEFINITIVO)
-----------------------------------------------------

\ |STYLE46|\  Elenco degli impianti di depurazione pubblici di competenza, georeferenziati 

\ |STYLE47|\  Dataset tabellare

\ |STYLE48|\  Mensile

Esempio: \ |LINK9|\  


+-------------------+--------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                             |Tipo  |Obbligo|
+===================+========================================================+======+=======+
|ID_Impianto        |Codice identificativo dell’impianto                     |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE49|\       |Nome dell’impianto                                      |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE50|\       |Codice identificativo del comune                        |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE51|\       |Comune di riferimento                                   |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE52|\       |Comuni serviti dall’impianto                            |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE53|\       |Indicare il corpo idrico recettore (es. nome “fiume x”) |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE54|\       |Altezza espressa in mslm                                |Numero|M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE55|\       |Via in cui si trova l’impianto                          |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE56|\       |Longitudine                                             |Numero|M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE57|\       |Latitudine                                              |Numero|M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE58|\       |Data di avvio                                           |Data  |O      |
+-------------------+--------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h43321d10544d6f71592d465d7a1f3b4d:

#35 Quantità rifiuti prodotta (DEFINITIVO)
------------------------------------------

\ |STYLE59|\  Quantità di rifiuti prodotti dalla raccolta differenziata e non differenziata, specificandone categoria e modalità di raccolta. 

\ |STYLE60|\  Dataset tabellare

\ |STYLE61|\  Mensile

Esempio 1: \ |LINK10|\ 

Esempio 2: Comune di Isso -  \ |LINK11|\ 


+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                               |Tipo  |Obbligo|
+===================+==========================================================================================================================+======+=======+
|Anno               |Anno di riferimento                                                                                                       |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE62|\       |Indicare se si tratta di rifiuti non differenziati, raccolta differenziata o Inerti e rifiuti da costruzione e demolizione|Testo |M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE63|\       |Indicare la categoria di rifiuti (es. carta e cartone, vetro, ecc.)                                                       |Testo |M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE64|\       |Codice della Categoria rifiuti                                                                                            |Testo |O      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE65|\       |Indicare la modalità di raccolta (es. meccanizzata, porta a porta, area attrezzata)                                       |Testo |M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE66|\       |Indicare il mese di riferimento in numero                                                                                 |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE67|\       |Indicare la quantità in kg                                                                                                |Numero|M      |
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

\ |STYLE68|\  Elenco pratiche gestite dallo Sportello Unico Attività Produttive

\ |STYLE69|\  Dataset tabellare

\ |STYLE70|\  Mensile

Esempio 1: \ |LINK12|\  

Esempio 2: \ |LINK13|\  


+-------------------+-----------------------------------+-------+-------+
|Denominazione Campo|Descrizione                        |Tipo   |Obbligo|
+===================+===================================+=======+=======+
|Anno               |Anno di riferimento                |Numero |M      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE71|\       |Codice identificativo della pratica|Testo  |O      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE72|\       |Ragione sociale del richiedente    |Testo  |M      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE73|\       |Numero di protocollo               |Testo  |M      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE74|\       |Indicare l’oggetto della richiesta |Testo  |O      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE75|\       |Data della richiesta               |Data   |M      |
+-------------------+-----------------------------------+-------+-------+
|\ |STYLE76|\       |Link alla pratica                  |Web URL|O      |
+-------------------+-----------------------------------+-------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h65512721d471161b6456c5353295:

#45        Servizi alla persona (DEFINITIVO)
--------------------------------------------

\ |STYLE77|\  Elenco e informazioni relative ai servizi alla persona

\ |STYLE78|\  Dataset tabellare

\ |STYLE79|\  Tempestiva

Esempio: \ |LINK14|\  

+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo  |Obbligo|
+===================+==========================================================================================================================================+======+=======+
|Denominazione      |Denominazione attività                                                                                                                    |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE80|\       |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                                                                           |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE81|\       |Breve descrizione del tipo di servizio offerto (ad esempio parrucchiere, estetista, ecc.)                                                 |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE82|\       |Superficie destinata all’esercizio dell’attività (espressa in metri quadrati)                                                             |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE83|\       |Superficie destinata ad altri usi (espressa in metri quadrati)                                                                            |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE84|\       |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE85|\       |Longitudine                                                                                                                               |Numero|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE86|\       |Latitudine                                                                                                                                |Numero|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h192d703349757a442f2040344a7476f:

#47    Pubblici esercizi (DEFINITIVO)
-------------------------------------

\ |STYLE87|\ : Informazioni sugli esercizi pubblici con dati georeferenziati

\ |STYLE88|\  Dataset tabellare

\ |STYLE89|\ : Tempestiva

+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo  |Obbligo|
+===================+==========================================================================================================================================+======+=======+
|Denominazione      |Denominazione esercizio                                                                                                                   |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE90|\       |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                                                                           |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE91|\       |Tipologia di esercizio (ad esempio bar, ristorante ecc.)                                                                                  |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE92|\       |Tipologia di somministrazione (ad esempio bevande, pasti ecc.)                                                                            |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE93|\       |Modalità di somministrazione (ad esempio al banco, al tavolo ecc.)                                                                        |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE94|\       |Superficie destinata alla somministrazione (espressa in metri quadrati)                                                                   |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE95|\       |Presenza di WiFi pubblico (Si/No)                                                                                                         |Testo |O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE96|\       |Longitudine                                                                                                                               |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE97|\       |Latitudine                                                                                                                                |Numero|M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE98|\       |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo |O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+

.. _h1216263d3b30172471575b782e2e3b7a:

3.       CULTURA
================

.. _h1e1aa304264214b219785d425e70:

#48   Eventi (DEFINITIVO)
-------------------------

\ |STYLE99|\ : Informazioni su eventi e manifestazioni 

\ |STYLE100|\  Dataset tabellare

\ |STYLE101|\ : Tempestiva

+-------------------+---------------------------------------------------------------+--------+---------------------------+
|Denominazione Campo|Descrizione                                                    |Tipo    |Obbligo                    |
+===================+===============================================================+========+===========================+
|Ubicazione         |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE102|\      |Anno di riferimento                                            |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE103|\      |Denominazione evento                                           |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE104|\      |Tipologia evento                                               |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE105|\      |Numero edizione dell’evento                                    |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE106|\      |Descrizione dell’evento                                        |Testo   |O                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE107|\      |Data di inizio dell’evento                                     |Data    |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE108|\      |Ora di inizio dell’evento                                      |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE109|\      |Data di conclusione dell’evento                                |Data    |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE110|\      |Ora di conclusione dell’evento                                 |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE111|\      |Link al sito web dell’evento                                   |Link Web|M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE112|\      |Link al programma dell’evento                                  |Link Web|M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE113|\      |Nome dell’ente che organizza l’evento                          |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE114|\      |Indirizzo email dell’ente organizzatore                        |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE115|\      |Telefono dell’ente organizzatore                               |Testo   |O                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE116|\      |Evento gratuito (SI/NO)                                        |Testo   |M                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE117|\      |Prezzo biglietto                                               |Testo   | M (se evento non gratuito)|
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE118|\      |Longitudine                                                    |Numero  |O                          |
+-------------------+---------------------------------------------------------------+--------+---------------------------+
|\ |STYLE119|\      |Latitudine                                                     |Numero  |O                          |
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

\ |STYLE120|\ : Beni artistici e architettonici del territorio

\ |STYLE121|\  Dataset tabellare

\ |STYLE122|\ : Tempestiva

Esempio: \ |LINK15|\  

+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|Denominazione Campo|Descrizione                                                                               |Tipo   |Obbligo|
+===================+==========================================================================================+=======+=======+
|ID_Bene            |Codice identificativo del bene artistico o architettonico                                 |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE123|\      |Denominazione del bene artistico o architettonico                                         |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE124|\      |Descrizione del bene                                                                      |Testo  |O      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE125|\      |Inserire la tipologia di bene (es. Museo, villa, parco…come classificato qui \ |LINK16|\ )|Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE126|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                           |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE127|\      |Indirizzo email per richiedere informazioni                                               |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE128|\      |Recapito telefonico a cui richiedere informazioni                                         |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE129|\      |Link al sito web                                                                          |Web URL|M      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE130|\      |Eventuali ulteriori informazioni                                                          |Testo  |O      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE131|\      |Longitudine                                                                               |Numero |O      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE132|\      |Latitudine                                                                                |Numero |O      |
+-------------------+------------------------------------------------------------------------------------------+-------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h405b7c14e20627c163b5a181f5126:

4.       ENERGIA
================

.. _h31437f1420597a45737174704a683466:

#30 Albo provinciale manutentori impianti termici (DEFINITIVO)
--------------------------------------------------------------

\ |STYLE133|\ : Elenco manutentori impianti termici abilitati

\ |STYLE134|\  Dataset tabellare

\ |STYLE135|\ : Tempestiva

Esempio: \ |LINK17|\  

+-------------------+---------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                    |Tipo  |Obbligo|
+===================+===============================================================+======+=======+
|Nome               |Nome o ragione sociale del manutentore                         |Testo |M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE136|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo |M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE137|\      |Numero telefonico del manutentore                              |Numero|O      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE138|\      |Indirizzo email del manutentore                                |Testo |O      |
+-------------------+---------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h496c7f2d61647381a4a4c53306f344a:

5.       MOBILITÀ E TRASPORTI
=============================

.. _h71376c30591b534c645e1d4c7b187:

#3 Orario Trasporto Pubblico (DEFINITIVO)
-----------------------------------------

\ |STYLE139|\ : Il dataset contiene i dati relativi alle corse, agli orari e alle fermate del trasporto pubblico urbano ed extra-urbano (pianificato). 

\ |STYLE140|\  Dataset tabellare

\ |STYLE141|\ : Tempestiva

Si tratta di uno Zip file. Lo standard di riferimento è il GTFS. \ |LINK18|\ 

Esempio 1: \ |LINK19|\   

Esempio 2: \ |LINK20|\  

Esempio 3: \ |LINK21|\  

.. _h3761631274d34195427717075576131:

#8 Mappa ZTL (DEFINITIVO)
-------------------------

\ |STYLE142|\ : Mappa Zona a Traffico Limitato 

\ |STYLE143|\  Dataset geografico (Shapefile)

\ |STYLE144|\ : Tempestiva

Esempio: \ |LINK22|\  


+-------------------+--------------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                                   |Tipo |Obbligo|
+===================+==============================================================+=====+=======+
|Nome_ZTL           |Denominazione della ZTL                                       |Testo|M      |
+-------------------+--------------------------------------------------------------+-----+-------+
|\ |STYLE145|\      |Indicare il periodo di riferimento (es. annuale, estivo, ecc.)|Testo|M      |
+-------------------+--------------------------------------------------------------+-----+-------+
|\ |STYLE146|\      |Informazioni aggiuntive (es. orari)                           |Testo|M      |
+-------------------+--------------------------------------------------------------+-----+-------+

.. _h2c1d74277104e41780968148427e:




.. _h794ab20525873f625363207210359:

#9 Varchi ZTL (DEFINITIVO)
--------------------------

\ |STYLE147|\ : Informazioni sui  varchi della ZTL, georeferenziati

\ |STYLE148|\  Dataset tabellare

\ |STYLE149|\ : Tempestiva

Esempio: \ |LINK23|\  

+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo   |Obbligo|
+===================+==========================================================================================================================================+=======+=======+
|Via                |Nome della via in cui è posizionato il varco                                                                                              |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE150|\      |Tipologia del varco (es. videosorvegliato)                                                                                                |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE151|\      |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo  |O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE152|\      |Eventuali deroghe all’accesso (ad esempio velocipedi)                                                                                     |Testo  |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE153|\      |Longitudine                                                                                                                               |Numero |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE154|\      |Latitudine                                                                                                                                |Numero |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+-------+-------+
|\ |STYLE155|\      |Link alla pagina informativa, se presente sul sito web dell’ente                                                                          |Web URL|O      |
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

\ |STYLE156|\ : Posizione e informazioni sui Parcheggi

\ |STYLE157|\  Dataset tabellare

\ |STYLE158|\ : Tempestiva

Esempio: \ |LINK24|\  

+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                               |Tipo  |Obbligo|
+===================+==========================================================================================================================================+======+=======+
|ID_Parcheggio      |Codice identificativo del parcheggio                                                                                                      |Testo |O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE159|\      |Tipologia del parcheggio (es. aperto, coperto)                                                                                            |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE160|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                                                                           |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE161|\      |Per gli orari di apertura e chiusura vedere l’Allegato 1 - Tabella 2 (oppure Tabella 3 se gli orari sono diversi a seconda della stagione)|Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE162|\      |Longitudine                                                                                                                               |Numero|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE163|\      |Latitudine                                                                                                                                |Numero|O      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE164|\      |Indicare se il parcheggio è gratuito (SI/NO)                                                                                              |Testo |M      |
+-------------------+------------------------------------------------------------------------------------------------------------------------------------------+------+-------+

.. _h7a387f69313ca44387272731b5f2b50:

#11   Piste ciclabili (DEFINITIVO)
----------------------------------

\ |STYLE165|\ : Tracciato delle piste ciclabili  piste ciclabili

\ |STYLE166|\  Dataset geografico (Shapefile)

\ |STYLE167|\ : Tempestiva

Esempio 1: \ |LINK25|\ 

Esempio 2: \ |LINK26|\ 

+-------------------+-------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                            |Tipo  |Obbligo|
+===================+=======================================================+======+=======+
|ID                 |Identificativo pista ciclabile                         |Testo |M      |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE168|\      |Breve descrizione                                      |Testo |M      |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE169|\      |Tipologia percorso, scegliendo tra le seguenti opzioni:|Testo |M      |
|                   |                                                       |      |       |
|                   |* ciclabile                                            |      |       |
|                   |                                                       |      |       |
|                   |* ciclopedonale                                        |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE170|\      |Indicare una delle seguenti opzioni:                   |Testo |M      |
|                   |                                                       |      |       |
|                   |* sede propria                                         |      |       |
|                   |                                                       |      |       |
|                   |* sede promiscua veicolare                             |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE171|\      |Tipo di fondo, scegliendo tra:                         |Testo |M      |
|                   |                                                       |      |       |
|                   |* asfaltato                                            |      |       |
|                   |                                                       |      |       |
|                   |* sterrato                                             |      |       |
|                   |                                                       |      |       |
|                   |* ciottolato                                           |      |       |
|                   |                                                       |      |       |
|                   |* pavimentato (es. resina)                             |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE172|\      |Lunghezza del percorso (espressa in metri)             |Numero|M      |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE173|\      |Larghezza del percorso (espressa in metri)             |Numero|O      |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE174|\      |Specificare una delle seguenti opzioni:                |Testo |M      |
|                   |                                                       |      |       |
|                   |* monodirezionale                                      |      |       |
|                   |                                                       |      |       |
|                   |* bidirezionale                                        |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE175|\      |Indicare una delle seguenti opzioni:                   |Testo |O      |
|                   |                                                       |      |       |
|                   |* aperta                                               |      |       |
|                   |                                                       |      |       |
|                   |* chiusa                                               |      |       |
|                   |                                                       |      |       |
|                   |* in costruzione                                       |      |       |
+-------------------+-------------------------------------------------------+------+-------+
|\ |STYLE176|\      |Ambito del percorso (es. stradale, fluviale, parco)    |Testo |O      |
+-------------------+-------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h4673596e42433c23372f496042157a48:

#12 Aree di sosta (DEFINITIVO)
------------------------------

\ |STYLE177|\ : Aree di sosta 

\ |STYLE178|\  Dataset geografico (Shapefile)

\ |STYLE179|\ : Tempestiva

Esempio: \ |LINK27|\  

+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                                                                                                                |Tipo |Obbligo|
+===================+===========================================================================================================================================+=====+=======+
|ID_Area            |Codice identificativo dell’area                                                                                                            |Testo|M      |
+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+
|\ |STYLE180|\      |Indicare la tipologia di area per soggetto interessato (es. disabili, sosta libera, bici, autobus, autocarri,ecc.) come da tabella seguente|Testo|M      |
+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+
|\ |STYLE181|\      |Via, Piazza, ecc                                                                                                                           |Testo|M      |
+-------------------+-------------------------------------------------------------------------------------------------------------------------------------------+-----+-------+
|\ |STYLE182|\      |Nome Via, Piazza, ecc.                                                                                                                     |Testo|M      |
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

\ |STYLE183|\ : Aree pedonali

\ |STYLE184|\  Dataset geografico (Shapefile)

\ |STYLE185|\ : Tempestiva

Esempio: \ |LINK28|\  

+-------------------+-------------------------------+-----+-------+
|Denominazione Campo|Descrizione                    |Tipo |Obbligo|
+===================+===============================+=====+=======+
|ID_Area            |Codice identificativo dell’area|Testo|M      |
+-------------------+-------------------------------+-----+-------+
|\ |STYLE186|\      |Via, Piazza, ecc               |Testo|M      |
+-------------------+-------------------------------+-----+-------+
|\ |STYLE187|\      |Nome Via, Piazza, ecc.         |Testo|M      |
+-------------------+-------------------------------+-----+-------+

.. _h413751694948146ea793c3974582760:

#15 Bike sharing (DEFINITIVO)
-----------------------------

\ |STYLE188|\ : Postazioni di Bike sharing

\ |STYLE189|\  Dataset geografico (Shapefile)

\ |STYLE190|\ : Tempestiva

Esempio: \ |LINK29|\  

+-------------------+-------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                  |Tipo  |Obbligo|
+===================+=============================================================+======+=======+
|ID_Staz            |Codice identificativo della stazione di bike sharing         |Numero|M      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE191|\      |Per le informazioni di ubicazione vedere Allegato 1 Tabella 1|Testo |M      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE192|\      |Latitudine                                                   |Numero|M      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE193|\      |Longitudine                                                  |Numero|M      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE194|\      |Numero di biciclette disponibile per stazione                |Numero|O      |
+-------------------+-------------------------------------------------------------+------+-------+
|\ |STYLE195|\      |Ulteriore descrizione dell’area                              |Testo |O      |
+-------------------+-------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h781030632f513187a587241745959:

#31 Autoscuole (DEFINITIVO)
---------------------------

\ |STYLE196|\ : Elenco delle Autoscuole autorizzate nel territorio

\ |STYLE197|\  Dataset tabellare

\ |STYLE198|\ : Tempestiva

Esempio: \ |LINK30|\  

L’esempio si riferisce alla tipologia di informazioni da inserire nel dataset. Per quanto riguarda la suddivisione delle informazioni in campi, occorre fare riferimento alla tabella seguente. In particolare, per l’indirizzo occorre inserire tutti i campi previsti per l’ubicazione come indicati nell’Allegato 1 Tabella 1. 

+-------------------+---------------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                                    |Tipo |Obbligo|
+===================+===============================================================+=====+=======+
|Nome               |Nome dell’autoscuola                                           |Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE199|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE200|\      |Numero di telefono dell’autoscuola                             |Testo|O      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE201|\      |Indirizzo email dell’autoscuola                                |Testo|O      |
+-------------------+---------------------------------------------------------------+-----+-------+

.. _h2c1d74277104e41780968148427e:




.. _h29173c11c44516963343b7a352726b:

#33 Aree di sosta per disabili (DEFINITIVO)
-------------------------------------------

\ |STYLE202|\ : Elenco delle Aree di sosta per disabili presenti nel territorio

\ |STYLE203|\  Dataset tabellare

\ |STYLE204|\ : Tempestiva

Esempio: \ |LINK31|\  

+-------------------+---------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                    |Tipo  |Obbligo|
+===================+===============================================================+======+=======+
|ID_Area            |Codice identificativo dell’area                                |Testo |M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE205|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo |M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE206|\      |Numero stalli dell’area di sosta                               |Numero|M      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE207|\      |Longitudine                                                    |Numero|O      |
+-------------------+---------------------------------------------------------------+------+-------+
|\ |STYLE208|\      |Latitudine                                                     |Numero|O      |
+-------------------+---------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h7f1d5c471796a7032617255597b173a:

#44 Punti di ricarica veicoli (DEFINITIVO)
------------------------------------------

\ |STYLE209|\ : Dataset con coordinate geografiche dei punti di ricarica dei veicoli elettrici, con indicazione del tipo di presa e KW

\ |STYLE210|\  Dataset tabellare

\ |STYLE211|\ : Tempestiva

Esempio: \ |LINK32|\  

+-------------------+--------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                     |Tipo  |Obbligo|
+===================+================================================================================+======+=======+
|ID_Sito            |Codice identificativo del sito in cui è possibile ricaricare i veicoli elettrici|Numero|O      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE212|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                 |Testo |M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE213|\      |Potenza della ricarica                                                          |Numero|M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE214|\      |Indicare la modalità di utilizzo del servizio (es. tramite CRS)                 |Testo |M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE215|\      |Indicare la tipologia di presa (es. universale)                                 |Testo |M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE216|\      |Indicare le tipologie di veicoli per le quali è disponibile la ricarica         |Testo |M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE217|\      |Data di attivazione del sito                                                    |Data  |O      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE218|\      |Longitudine                                                                     |Numero|M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+
|\ |STYLE219|\      |Latitudine                                                                      |Numero|M      |
+-------------------+--------------------------------------------------------------------------------+------+-------+

.. _h127c74681e53786e536b765a2f6647e:

6.       SICUREZZA
==================

.. _h824122d55a315e452768e7f292a6e:

#7 Incidenti stradali (DEFINITIVO)
----------------------------------

\ |STYLE220|\ : Dataset contenente gli incidenti stradali con data, ora, coordinate geografiche, mezzi coinvolti, eventuali morti e feriti

\ |STYLE221|\ : Dataset tabellare

\ |STYLE222|\ : Mensile

Esempio 1: \ |LINK33|\ 

Esempio 2: \ |LINK34|\  

+-------------------+----------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                       |Tipo  |Obbligo|
+===================+==================================================================================+======+=======+
|Anno               |Anno di riferimento                                                               |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE223|\      |Data dell’incidente                                                               |Data  |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE224|\      |Ora dell’incidente                                                                |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE225|\      |Descrizione del punto preciso dell’incidente (es. via...all’intersezione con via…)|Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE226|\      |Tipologia di incidente (es. scontro frontale)                                     |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE227|\      |Numero delle persone illese                                                       |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE228|\      |Numero delle persone ferite                                                       |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE229|\      |Numero dei morti                                                                  |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE230|\      |Indicare se sono stati coinvolti pedoni (SI/NO)                                   |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE231|\      |Indicare se sono stati coinvolti velocipedi (SI/NO)                               |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE232|\      |Indicare se sono stati coinvolti ciclomotori o motocicli (SI/NO)                  |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE233|\      |Indicare se sono stati coinvolti mezzi pesanti (SI/NO)                            |Testo |M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE234|\      |Longitudine                                                                       |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+
|\ |STYLE235|\      |Latitudine                                                                        |Numero|M      |
+-------------------+----------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h4760d266a547666543d45223781653:

#41  Principali infrazioni al Codice della Strada (DEFINITIVO)
--------------------------------------------------------------

\ |STYLE236|\ : Elenco, tipologia e anno di riferimento delle principali infrazioni al Codice della Strada.

\ |STYLE237|\  Dataset tabellare

\ |STYLE238|\ : Mensile

Esempio: \ |LINK35|\ 

+-------------------+--------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                         |Tipo  |Obbligo|
+===================+====================================================================+======+=======+
|Anno               |Anno di riferimento                                                 |Numero|M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE239|\      |Tipo di infrazione (es. limite velocità, sensi unici, sosta, ecc.)  |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE240|\      |Normativa di riferimento dell’infrazione (es. Legge)                |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE241|\      |Art. di legge o altra norma che regola il tipo di infrazione        |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE242|\      |Data infrazione                                                     |Data  |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE243|\      |Tipologia di veicolo: autovettura, motoveicolo, ciclomotore         |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE244|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1     |Testo |M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE245|\      |Inserire il numero delle sanzioni erogate per l’infrazione specifica|Numero|M      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE246|\      |Longitudine                                                         |Numero|O      |
+-------------------+--------------------------------------------------------------------+------+-------+
|\ |STYLE247|\      |Latitudine                                                          |Numero|O      |
+-------------------+--------------------------------------------------------------------+------+-------+

.. _h6f396320344978474c3f7b4d6b7e531c:

#42 Provvedimenti adottati dalla Polizia Locale in materia di commercio (DEFINITIVO)
------------------------------------------------------------------------------------

\ |STYLE248|\ : Elenco e tipologia dei provvedimenti adottati in materia di commercio dalla Polizia Municipale

\ |STYLE249|\  Dataset tabellare

\ |STYLE250|\ : Mensile

Esempio: \ |LINK36|\  

+-------------------+---------------------+------+-------+
|Denominazione Campo|Descrizione          |Tipo  |Obbligo|
+===================+=====================+======+=======+
|Anno               |Anno di riferimento  |Numero|M      |
+-------------------+---------------------+------+-------+
|\ |STYLE251|\      |Tipo di provvedimento|Testo |M      |
+-------------------+---------------------+------+-------+
|\ |STYLE252|\      |Numero di controlli  |Numero|M      |
+-------------------+---------------------+------+-------+
|\ |STYLE253|\      |Numero di verbali    |Numero|M      |
+-------------------+---------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h04573713141737316103050642c523f:

#49 Controlli in cantiere effettuati dalla Polizia Locale (DEFINITIVO)
----------------------------------------------------------------------

\ |STYLE254|\ : Elenco, tipologia e anno di riferimento dei controlli effettuati nei cantieri dalla Polizia locale

\ |STYLE255|\  Dataset tabellare

\ |STYLE256|\ : Mensile

+-------------------+----------------------+------+-------+
|Denominazione Campo|Descrizione           |Tipo  |Obbligo|
+===================+======================+======+=======+
|Anno               |Anno di riferimento   |Numero|M      |
+-------------------+----------------------+------+-------+
|\ |STYLE257|\      |Tipologia di controllo|Testo |M      |
+-------------------+----------------------+------+-------+
|\ |STYLE258|\      |Numero di controlli   |Numero|M      |
+-------------------+----------------------+------+-------+
|\ |STYLE259|\      |Numero di verbali     |Numero|M      |
+-------------------+----------------------+------+-------+

.. _h6a50711f57485b63626e405f165261:

7.      STATISTICA
==================

.. _h5613e1e752356544a7e5e63615a2a59:

Per quanto riguarda i risultati delle elezioni, in seguito ad un’analisi ulteriore è stata individuata una soluzione alternativa alla pubblicazione dei 3 dataset distinti (#38, #39 e #40): pubblicare un unico dataset che comprenda sia i risultati delle elezioni sia i dati statistici sull’affluenza (vedere tabella #38#39#40BIS Risultati elezioni). Questo consentirebbe di mantenere sempre uguale la struttura del dataset (campi) rendendo più facilmente confrontabili i dati. 
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

.. _h622e23792f56633f6528392962727827:

Ai fini del co-finanziamento, la pubblicazione del dataset #38#39#40BIS viene equiparata alla pubblicazione dei 3 dataset relativi alle elezioni (#38 + #39 + #40). 
--------------------------------------------------------------------------------------------------------------------------------------------------------------------

.. _h47274b145479547445336f771b35280:

#38 Risultati elezioni comunali (DEFINITIVO)
--------------------------------------------

\ |STYLE260|\ : Risultati elettorali delle elezioni amministrative del proprio comune o provincia

\ |STYLE261|\  Dataset tabellare

\ |STYLE262|\ : Tempestiva

+-------------------+-----------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                        |Tipo  |Obbligo|
+===================+===================================================================================+======+=======+
|Data               |Data elezione (giorno, mese, anno)                                                 |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE263|\      |Indicare se si tratta di:                                                          |Testo |M      |
|                   |                                                                                   |      |       |
|                   |* 1° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* 2° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* turno unico                                                                      |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE264|\      |Collegio elettorale o circoscrizione                                               |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE265|\      |Numero della sezione                                                               |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE266|\      |Consiglio comunale o Sindaco                                                       |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE267|\      |Inserire in questa colonna una riga per ciascuna delle seguenti informazioni:      |Testo |M      |
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
|\ |STYLE268|\      |Inserire una riga per ciascuna delle seguenti informazioni:                        |Numero|M      |
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

\ |STYLE269|\ : Risultati elettorali delle elezioni regionali nel proprio comune o provincia

\ |STYLE270|\  Dataset tabellare

\ |STYLE271|\ : Tempestiva

+-------------------+-----------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                        |Tipo  |Obbligo|
+===================+===================================================================================+======+=======+
|Data               |Data elezione (giorno, mese, anno)                                                 |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE272|\      |Indicare se si tratta di:                                                          |Testo |M      |
|                   |                                                                                   |      |       |
|                   |* 1° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* 2° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* turno unico                                                                      |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE273|\      |Collegio elettorale o circoscrizione                                               |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE274|\      |Numero della sezione                                                               |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE275|\      |Consiglio regionale o Presidente della Regione                                     |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE276|\      |Inserire in questa colonna una riga per ciascuna delle seguenti informazioni:      |Testo |M      |
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
|\ |STYLE277|\      |Inserire una riga per ciascuna delle seguenti informazioni:                        |Numero|M      |
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

\ |STYLE278|\ : Risultati elettorali delle elezioni nazionali nel proprio comune o provincia

\ |STYLE279|\  Dataset tabellare

\ |STYLE280|\ : Tempestiva

+-------------------+-----------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                        |Tipo  |Obbligo|
+===================+===================================================================================+======+=======+
|Data               |Data elezione (giorno, mese, anno)                                                 |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE281|\      |Indicare se si tratta di:                                                          |Testo |M      |
|                   |                                                                                   |      |       |
|                   |* 1° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* 2° turno                                                                         |      |       |
|                   |                                                                                   |      |       |
|                   |* turno unico                                                                      |      |       |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE282|\      |Collegio elettorale o circoscrizione                                               |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE283|\      |Numero della sezione                                                               |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE284|\      |Camera dei deputati o Senato della Repubblica                                      |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------+------+-------+
|\ |STYLE285|\      |Inserire in questa colonna una riga per ciascuna delle seguenti informazioni:      |Testo |M      |
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
|\ |STYLE286|\      |Inserire una riga per ciascuna delle seguenti informazioni:                        |Numero|M      |
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

\ |STYLE287|\ : Risultati elettorali e dati sull’affluenza 

\ |STYLE288|\  Dataset tabellare

\ |STYLE289|\ : Tempestiva

+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                                                                                                                                                                                |Tipo  |Obbligo|
+===================+===========================================================================================================================================================================================================================================================+======+=======+
|Data               |Data elezione (giorno, mese, anno)                                                                                                                                                                                                                         |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE290|\      |In caso di più tornate elettorali, specificare il turno o indicare se turno unico (1° turno, 2° turno, turno unico)                                                                                                                                        |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE291|\      |Tipologia di elezione (es. Camera, Senato, Comunali, Circoscrizionali, Provinciali, Regionali, Europee, Referendum 1, Referendum 2, ecc.)                                                                                                                  |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE292|\      |Es. Camera dei Deputati, Senato della Repubblica, Consiglio comunale, Sindaco, Consiglio provinciale, Presidente della Provincia, Consiglio regionale, Presidente della Regione, Parlamento europeo, oppure l’oggetto del referendum (es. energia nucleare)|Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE293|\      |Collegio elettorale o Circoscrizione                                                                                                                                                                                                                       |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE294|\      |Numero della sezione                                                                                                                                                                                                                                       |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE295|\      |Inserire in questa colonna una riga per ciascuna delle seguenti informazioni:                                                                                                                                                                              |Testo |M      |
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
|\ |STYLE296|\      |Inserire una riga per ciascuna delle seguenti informazioni:                                                                                                                                                                                                |Numero|M      |
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

\ |STYLE297|\ : Informazioni sulla condizione lavorativa dei residenti (ad esempio occupato, in cerca di occupazione ecc.)

\ |STYLE298|\  Dataset tabellare

\ |STYLE299|\ : Trimestrale

Esempio: \ |LINK37|\  

+-------------------+-------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                              |Tipo  |Obbligo|
+===================+=========================================================================+======+=======+
|Anno               |Anno di riferimento                                                      |Numero|M      |
+-------------------+-------------------------------------------------------------------------+------+-------+
|\ |STYLE300|\      |Condizione lavorativa (ad esempio occupato, in cerca di occupazione ecc.)|Testo |M      |
+-------------------+-------------------------------------------------------------------------+------+-------+
|\ |STYLE301|\      |Numero di maschi                                                         |Numero|M      |
+-------------------+-------------------------------------------------------------------------+------+-------+
|\ |STYLE302|\      |Numero di femmine                                                        |Numero|M      |
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

\ |STYLE303|\ : Rete viaria 

\ |STYLE304|\  Dataset geografico (Shapefile)

\ |STYLE305|\ : Tempestiva

+-------------------+------------------------+-----+-------+
|Denominazione Campo|Descrizione             |Tipo |Obbligo|
+===================+========================+=====+=======+
|Toponimo           |Toponimo della strada   |Testo|M      |
+-------------------+------------------------+-----+-------+
|\ |STYLE306|\      |Nome del toponimo       |Testo|M      |
+-------------------+------------------------+-----+-------+
|\ |STYLE307|\      |Località                |Testo|M      |
+-------------------+------------------------+-----+-------+
|\ |STYLE308|\      |Senso di marcia (U/D/A):|Testo|M      |
|                   |                        |     |       |
|                   |* U - Unico             |     |       |
|                   |                        |     |       |
|                   |* D - Doppio            |     |       |
|                   |                        |     |       |
|                   |* A - Alternato         |     |       |
+-------------------+------------------------+-----+-------+
|\ |STYLE309|\      |Primo numero civico     |Testo|M      |
+-------------------+------------------------+-----+-------+
|\ |STYLE310|\      |Ultimo numero civico    |Testo|M      |
+-------------------+------------------------+-----+-------+

.. _h5457273b5f6970146f702b17c7f3550:

#5 Rete viaria - Toponimi stradali (DEFINITIVO)
-----------------------------------------------

\ |STYLE311|\ : Elenco Toponimi stradali

\ |STYLE312|\  Dataset tabellare

\ |STYLE313|\ : Tempestiva

Esempio: \ |LINK38|\  

+-------------------+----------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                               |Tipo |Obbligo|
+===================+==========================================================+=====+=======+
|Classe_Toponimo    |Indicare la classe toponimo (es. Via, Piazza, Largo, ecc.)|Testo|M      |
+-------------------+----------------------------------------------------------+-----+-------+
|\ |STYLE314|\      |Nome di Via, Piazza, Largo, ecc.                          |Testo|M      |
+-------------------+----------------------------------------------------------+-----+-------+
|\ |STYLE315|\      |Codice del toponimo                                       |Testo|M      |
+-------------------+----------------------------------------------------------+-----+-------+
|\ |STYLE316|\      |Inserire se si tratta di un dato storico (SI/NO)          |Testo|M      |
+-------------------+----------------------------------------------------------+-----+-------+

.. _h2c1d74277104e41780968148427e:




.. _h563b1f5f11515e35374069365613121:

#6 Rete viaria - Numeri civici (DEFINITIVO)
-------------------------------------------

\ |STYLE317|\ : Numeri civici georeferenziati

\ |STYLE318|\  Dataset tabellare

\ |STYLE319|\ : Tempestiva

Esempio: https://www.dati.lombardia.it/Territorio/Comune-Bergamo-Numerazione-civica/pcif-9jj7

+-------------------+------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                           |Tipo  |Obbligo|
+===================+======================================================+======+=======+
|Classe_Toponimo    |Indicare la classe toponimo (Via, Piazza, Largo, ecc.)|Testo |M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE320|\      |Nome di Via, Piazza, Largo, ecc.                      |Testo |M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE321|\      |Numero del civico                                     |Numero|M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE322|\      |Componente alfabetica del civico (es. A, Bis, ecc.)   |Testo |M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE323|\      |CAP                                                   |Numero|M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE324|\      |Sezione di censimento ISTAT                           |Numero|O      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE325|\      |Longitudine                                           |Numero|M      |
+-------------------+------------------------------------------------------+------+-------+
|\ |STYLE326|\      |Latitudine                                            |Numero|M      |
+-------------------+------------------------------------------------------+------+-------+

.. _h32623c3510287d7f3af50466d4e60:

#14      Cantieri stradali (DEFINITIVO)
---------------------------------------

\ |STYLE327|\ : Cantieri stradali attivi 

\ |STYLE328|\  Dataset geografico (Shapefile)

\ |STYLE329|\ : Tempestiva


+-------------------+--------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                 |Tipo |Obbligo|
+===================+============================================+=====+=======+
|Toponimo           |Via, Piazza, ecc.                           |Testo|M      |
+-------------------+--------------------------------------------+-----+-------+
|\ |STYLE330|\      |Nome della via, piazza, ecc.                |Testo|M      |
+-------------------+--------------------------------------------+-----+-------+
|\ |STYLE331|\      |Breve descrizione dei lavori in svolgimento |Testo|M      |
+-------------------+--------------------------------------------+-----+-------+
|\ |STYLE332|\      |Data di inizio lavoro                       |Data |M      |
+-------------------+--------------------------------------------+-----+-------+
|\ |STYLE333|\      |Data prevista di fine lavoro                |Data |M      |
+-------------------+--------------------------------------------+-----+-------+

.. _h2c1d74277104e41780968148427e:




.. _h1a736c403f6676679673a673f60363a:

#16 HotSpot Wifi (DEFINITIVO)
-----------------------------

\ |STYLE334|\ : Elenco hotspot wifi pubblici, georeferenziati o dataset geografico

\ |STYLE335|\  Dataset tabellare

\ |STYLE336|\ : Tempestiva

Esempio: \ |LINK39|\  

+-------------------+--------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                           |Tipo  |Obbligo|
+===================+======================================================================================+======+=======+
|Rete               |Nome della rete (SSID)                                                                |Testo |O      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE337|\      |Codice identificativo del punto di accesso (singolo HotSpot Wifi) attribuito dall’ente|Testo |M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE338|\      |Indicare la tipologia del punto di accesso (HotSpot/Dispositivo estensione)           |Testo |O      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE339|\      |Nome del sito dove si trova il punto di accesso (es. denominazione Biblioteca…)       |Testo |M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE340|\      |Punto di accesso attivo (si, no)                                                      |Testo |M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE341|\      |Codice accesso                                                                        |Testo |O      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE342|\      |Longitudine                                                                           |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE343|\      |Latitudine                                                                            |Numero|M      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+
|\ |STYLE344|\      |Indicare il raggio di copertura in metri                                              |Numero|O      |
+-------------------+--------------------------------------------------------------------------------------+------+-------+

 

.. _h5a2161623f35403f62b4f305243726a:

#19 Area per sgambatura cani (DEFINITIVO)
-----------------------------------------

\ |STYLE345|\ : Mappa aree per sgambatura cani

\ |STYLE346|\  Dataset geografico (Shapefile)

\ |STYLE347|\ : Tempestiva

+-------------------+----------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                     |Tipo  |Obbligo|
+===================+================================================================+======+=======+
|ID_Area            |Codice identificativo dell’area                                 |Numero|M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE348|\      |Comune in cui è ubicata l’area                                  |Testo |M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE349|\      |Via, Piazza, ecc.                                               |Testo |M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE350|\      |Nome della via, piazza, ecc.                                    |Testo |M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE351|\      |Indicare la superficie dell’area (mq)                           |Numero|M      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE352|\      |Indicare se sono presenti fontanelle (SI/NO)                    |Testo |O      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE353|\      |Indicare se sono presenti attrezzature per addestramento (SI/NO)|Testo |O      |
+-------------------+----------------------------------------------------------------+------+-------+
|\ |STYLE354|\      |Indicare se sono presenti panchine(SI/NO)                       |Testo |O      |
+-------------------+----------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2ca5320503f5437a26b171269386a:

#21 Pratiche edilizie (DEFINITIVO) 
-----------------------------------

\ |STYLE355|\ : Elenco Pratiche edilizie gestite dallo Sportello Unico per l’Edilizia

\ |STYLE356|\  Dataset tabellare

\ |STYLE357|\ : Mensile

Esempio: \ |LINK40|\  

+-------------------+--------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                             |Tipo  |Obbligo|
+===================+========================================================+======+=======+
|Anno               |Anno di riferimento                                     |Numero|M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE358|\      |Tipologia istanza (es. SCIA, PDC, ecc.)                 |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE359|\      |Codice identificativo dell’istanza                      |Testo |O      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE360|\      |Data di presentazione dell’istanza                      |Data  |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE361|\      |Numero di protocollo dell’istanza                       |Numero|O      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE362|\      |Numero del provvedimento (nel caso di PDC)              |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE363|\      |Data del provvedimento (nel caso di PDC)                |Data  |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE364|\      |Nominativo o Ragione sociale dell’istante \ |STYLE365|\ |Testo |O      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE366|\      |Descrizione dell’intervento oggetto dell’istanza        |Testo |M      |
+-------------------+--------------------------------------------------------+------+-------+
|\ |STYLE367|\      |Codice ecografico del fabbricato                        |Testo |O      |
+-------------------+--------------------------------------------------------+------+-------+

.. _h507e71435666451e1b704f12233b4852:

\* Ciascun ente valuta la pubblicazione del dato in base al principio del bilanciamento tra l’interesse pubblico a conoscere dati, informazioni e documenti per tutelare i diritti dei cittadini e l’interesse pubblico alla tutela dei diritti delle persone e delle organizzazioni private che potrebbero essere lesi dalla disponibilità di dati, informazioni e documenti.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h752c462f6e4e4179353571873311521:

#22 Elenco beni confiscati (DEFINITIVO) 
----------------------------------------

\ |STYLE368|\ : Elenco beni confiscati alla mafia e assegnati al comune

\ |STYLE369|\  Dataset tabellare

\ |STYLE370|\ : Mensile

+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                              |Tipo  |Obbligo|
+===================+=========================================================================================+======+=======+
|ID_Bene            |Codice identificativo del bene confiscato                                                |Testo |O      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE371|\      |Tipologia del bene confiscato (es. appartamento, villa, ecc.)                            |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE372|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                          |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE373|\      |Superficie del bene confiscato (mq)                                                      |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE374|\      |Nominativo o ragione sociale dell’assegnatario del bene                                  |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE375|\      |Breve descrizione del progetto in funzione del quale il bene confiscato è stato assegnato|Testo |O      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE376|\      |Destinazione d’uso del bene confiscato                                                   |Testo |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE377|\      |Riferimenti all’atto di concessione                                                      |Testo |O      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE378|\      |Data dell’atto di concessione                                                            |Data  |M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+
|\ |STYLE379|\      |Numero di anni della concessione                                                         |Numero|M      |
+-------------------+-----------------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h1534f311220496307c39787c131e20:

#29 Centri revisione auto (DEFINITIVO)
--------------------------------------

\ |STYLE380|\ : Centri revisione auto autorizzati dalla Provincia

\ |STYLE381|\  Dataset tabellare

\ |STYLE382|\ : Tempestiva

Esempio: \ |LINK41|\ 


+-------------------+---------------------------------------------------------------+-----+-------+
|Denominazione Campo|Descrizione                                                    |Tipo |Obbligo|
+===================+===============================================================+=====+=======+
|Nome               |Nome del centro di revisione                                   |Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE383|\      |Tipologia di revisione (es. auto, moto, ecc.)                  |Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE384|\      |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1|Testo|M      |
+-------------------+---------------------------------------------------------------+-----+-------+
|\ |STYLE385|\      |Numero di telefono del centro di revisione                     |Testo|O      |
+-------------------+---------------------------------------------------------------+-----+-------+

.. _h5e126927772356f4b3651622c12502f:

9.  TRASPARENZA 
================

.. _h6a113f1a7b5a1f2e7d29274624462967:

#2 Contributi e sussidi (DEFINITIVO)
------------------------------------

\ |STYLE386|\ : Dati relativi agli atti di concessione di sovvenzioni, contributi, sussidi ed ausili finanziari alle imprese e comunque di vantaggi economici di qualunque genere a persone ed enti pubblici e privati

\ |STYLE387|\  Dataset tabellare

\ |STYLE388|\ : Tempestiva

Obblighi normativi: D. lgs. 33/2013, in particolare artt. 26-27.

Vedi \ |LINK42|\  (FAQ N. 13) 


+-------------------+-------------------------------------------------------------------------------+-------+-------+
|Denominazione Campo|Descrizione                                                                    |Tipo   |Obbligo|
+===================+===============================================================================+=======+=======+
|Anno               |Anno di riferimento                                                            |Numero |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE389|\      |Codice identificativo del provvedimento                                        |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE390|\      |Data del provvedimento                                                         |Data   |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE391|\      |Nominativo o Ragione sociale del soggetto beneficiario del provvedimento       |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE392|\      |Indicare se si tratta di amministrazione pubblica, privato, Onlus o altro ente |Testo  |O      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE393|\      |Codice fiscale del soggetto beneficiario del provvedimento                     |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE394|\      |Partita IVA del soggetto beneficiario del provvedimento                        |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE395|\      |Oggetto del provvedimento                                                      |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE396|\      |Riferimenti della norma o titolo a base dell’attribuzione                      |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE397|\      |URL norma o titolo                                                             |Web URL|O      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE398|\      |Ufficio responsabile del provvedimento.                                        |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE399|\      |Cognome del responsabile del procedimento                                      |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE400|\      |Nome del responsabile del procedimento                                         |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE401|\      |Modalità di individuazione del soggetto beneficiario (es. aggiudicazione bando)|Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE402|\      |Importo del vantaggio economico corrisposto                                    |Numero |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE403|\      |Breve descrizione progetto allegato al provvedimento                           |Testo  |M      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE404|\      |URL progetto                                                                   |Web URL|O      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+
|\ |STYLE405|\      |Link al curriculum del soggetto beneficiario                                   |Web URL|O      |
+-------------------+-------------------------------------------------------------------------------+-------+-------+

.. _h7782e36e316052235761422844d44:

#23 Elenco canoni di locazione (DEFINITIVO)
-------------------------------------------

\ |STYLE406|\ : Elenco canoni di locazione o di affitto percepiti

\ |STYLE407|\  Dataset tabellare

\ |STYLE408|\ : Mensile

Obblighi normativi: D. lgs. 33/2013, in particolare art. 30.

+-------------------+---------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                            |Tipo  |Obbligo|
+===================+=======================================================================================+======+=======+
|Anno               |Anno di riferimento                                                                    |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE409|\      |Indicare la tipologia di locazione (Attiva/Passiva)                                    |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE410|\      |Nominativo o Ragione sociale del locatario                                             |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE411|\      |Nominativo o Ragione sociale del locatore                                              |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE412|\      |Per le informazioni relative all’ubicazione dell’immobile vedere Allegato 1 - Tabella 1|Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE413|\      |Destinazione dell’immobile (es. uffici)                                                |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE414|\      |Data di decorrenza del contratto                                                       |Data  |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE415|\      |Data di scadenza del contratto                                                         |Data  |M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE416|\      |Canone annuale di affitto percepito al netto delle spese                               |Numero|M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE417|\      |Altre spese non inserite nel canone annuale                                            |Numero|M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+
|\ |STYLE418|\      |Canone annuale di affitto versato                                                      |Numero|M      |
+-------------------+---------------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h2c1d74277104e41780968148427e:




.. _h6326371021e1b65335f1b3a15d202c:

#24 Elenco immobili di proprietà (DEFINITIVO)
---------------------------------------------

\ |STYLE419|\ : Elenco informazioni identificative degli immobili posseduti

\ |STYLE420|\  Dataset tabellare

\ |STYLE421|\ : Mensile

Obblighi normativi: D. lgs. 33/2013, in particolare art. 30.

+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                         |Tipo  |Obbligo|
+===================+====================================================================================================+======+=======+
|Ubicazione         |Per le informazioni di ubicazione vedere Allegato 1 - Tabella 1                                     |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE422|\      |Denominazione dell’unità immobiliare (es. Palazzo Pirelli) o descrizione area (es. area industriale)|Testo |O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE423|\      |Indicare la natura giuridica del bene patrimoniale tra:                                             |Testo |M      |
|                   |                                                                                                    |      |       |
|                   |* disponibile                                                                                       |      |       |
|                   |                                                                                                    |      |       |
|                   |* indisponibile                                                                                     |      |       |
|                   |                                                                                                    |      |       |
|                   |* demaniale                                                                                         |      |       |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE424|\      |es. Immobile                                                                                        |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE425|\      |Codice identificativo categoria (dato catastale).                                                   |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE426|\      |Sezione (dato catastale)                                                                            |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE427|\      |Codice identificativo foglio (dato catastale)                                                       |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE428|\      |Codice identificativo mappale (dato catastale)                                                      |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE429|\      |Codice identificativo subalterno (dato catastale)                                                   |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE430|\      |Classe_catastale                                                                                    |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE431|\      |Unità di misura della consistenza (mq, mc, vani)                                                    |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE432|\      |Grandezza del bene (solo numero riferito all’unità di misura del campo precedente)                  |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE433|\      |Rendita catastale                                                                                   |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE434|\      |Destinazione d’uso del bene                                                                         |Testo |M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE435|\      |Superficie del bene (espressa in metri quadrati).                                                   |Numero|M      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE436|\      |Valore di mercato del bene                                                                          |Numero|O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE437|\      |Data di acquisizione del bene                                                                       |Data  |O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE438|\      |Longitudine                                                                                         |Numero|O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE439|\      |Latitudine                                                                                          |Numero|O      |
+-------------------+----------------------------------------------------------------------------------------------------+------+-------+

.. _h4451d524d372a6ed467c1876264f6d:

#25 Monitoraggio procedimenti (DEFINITIVO) 
-------------------------------------------

\ |STYLE440|\ : Monitoraggio dei tempi dei procedimenti

\ |STYLE441|\  Dataset tabellare

\ |STYLE442|\ : Semestrale

+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                                  |Tipo  |Obbligo|
+===================+=============================================================================================+======+=======+
|Tipologia          |Tipologia del procedimento (d’ufficio o a istanza di parte)                                  |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE443|\      |Nome del procedimento                                                                        |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE444|\      |Breve descrizione del procedimento                                                           |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE445|\      |Indicare il termine massimo di conclusione del procedimento stabilito dalla legge (in giorni)|Numero|M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE446|\      |Indicare il termine effettivo di conclusione del procedimento (in giorni)                    |Numero|M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE447|\      |Ufficio responsabile del provvedimento                                                       |Testo |M      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE448|\      |Indicare motivi di eventuali sospensioni o ritardi                                           |Testo |O      |
+-------------------+---------------------------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h132c4945185112631f3367485d57c16:

#26 Enti controllati – Società partecipate (DEFINITIVO)
-------------------------------------------------------

\ |STYLE449|\ : Elenco e informazioni sulle Società partecipate

\ |STYLE450|\  Dataset tabellare

\ |STYLE451|\ : Tempestiva

+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo            |Descrizione                                                                                       |Tipo  |Obbligo|
+===============================+==================================================================================================+======+=======+
|Ente_pubblico – Ragione_Sociale|Denominazione ente                                                                                |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE452|\                  |Funzioni affidate all’Ente                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE453|\                  |.Attività svolte dall’Ente per ottemperare alle funzioni                                          |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE454|\                  |Eventuale quota di partecipazione societaria all’ente                                             |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE455|\                  |“Indeterminato” oppure scadenza prevista                                                          |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE456|\                  |Onere complessivo a qualsiasi titolo gravante per l'anno sul bilancio dell'amministrazione        |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE457|\                  |Numero dei rappresentanti dell'amministrazione negli organi di governo                            |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE458|\                  |Trattamento economico complessivo dei rappresentanti dell'amministrazione negli organi di governo |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE459|\                  |Anno di riferimento                                                                               |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE460|\                  |Risultati di bilancio dell’anno di riferimento (ultimo anno)                                      |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE461|\                  |Risultati di bilancio del penultimo anno                                                          |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE462|\                  |Risultati di bilancio del terzultimo anno                                                         |Numero|M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE463|\                  |Link al sito istituzionale                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+

.. _h7239514f337e4b15371432716b161761:

#27 Enti controllati – Enti pubblici vigilati (DEFINITIVO)
----------------------------------------------------------

\ |STYLE464|\ : Elenco e informazioni sugli Enti pubblici vigilati

\ |STYLE465|\  Dataset tabellare

\ |STYLE466|\ : Tempestiva

+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo            |Descrizione                                                                                       |Tipo  |Obbligo|
+===============================+==================================================================================================+======+=======+
|Ente_pubblico – Ragione_Sociale|Denominazione ente                                                                                |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE467|\                  |Funzioni affidate all’Ente                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE468|\                  |Attività svolte dall’Ente per ottemperare alle funzioni                                           |Testo |M      |
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

.. _h2c1d74277104e41780968148427e:




.. _h6057240426a371f372442d4776d7f:

#28 Enti controllati – Enti di diritto privato controllati (DEFINITIVO)
-----------------------------------------------------------------------

\ |STYLE479|\ : Elenco e informazioni sugli Enti di diritto privato controllati

\ |STYLE480|\  Dataset tabellare

\ |STYLE481|\ : Tempestiva

+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|Denominazione Campo            |Descrizione                                                                                       |Tipo  |Obbligo|
+===============================+==================================================================================================+======+=======+
|Ente_pubblico – Ragione_Sociale|Denominazione ente                                                                                |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE482|\                  |Funzioni affidate all’Ente                                                                        |Testo |M      |
+-------------------------------+--------------------------------------------------------------------------------------------------+------+-------+
|\ |STYLE483|\                  |.Attività svolte dall’Ente per ottemperare alle funzioni                                          |Testo |M      |
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

.. _h586361a7d1b58732243725f242:

#36 Provvedimenti dei dirigenti (DEFINITIVO)
--------------------------------------------

\ |STYLE494|\ : Elenchi dei provvedimenti adottati dai dirigenti

\ |STYLE495|\  Dataset tabellare

\ |STYLE496|\ : Mensile

Obblighi normativi: D. lgs. 33/2013, in particolare art. 23.

Vedi \ |LINK43|\  


+-------------------+----------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                 |Tipo  |Obbligo|
+===================+============================================================================+======+=======+
|Anno               |Anno di riferimento                                                         |Numero|M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE497|\      |Indicare la tipologia di provvedimento tra le seguenti:                     |Testo |O      |
|                   |                                                                            |      |       |
|                   |#. Scelta del contraente per l'affidamento di lavori, forniture e servizi   |      |       |
|                   |                                                                            |      |       |
|                   |#. Accordi stipulati dall'amministrazione                                   |      |       |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE498|\      |Numero identificativo del provvedimento                                     |Numero|M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE499|\      |Titolo del provvedimento                                                    |Testo |M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE500|\      |Dispositivo del provvedimento                                               |Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE501|\      |Data di approvazione del provvedimento.                                     |Data  |M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE502|\      |Nome dell’ufficio proponente                                                |Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE503|\      |Eventuale spesa prevista                                                    |Numero|O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE504|\      |Riferimenti ai documenti principali contenuti nel fascicolo del procedimento|Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h57b79594a60271c37774e4b797e5e68:

#37 Provvedimenti degli organi di indirizzo politico (DEFINITIVO)
-----------------------------------------------------------------

\ |STYLE505|\ : Elenchi dei Provvedimenti degli organi di indirizzo politico

\ |STYLE506|\  Dataset tabellare

\ |STYLE507|\ : Mensile

Obblighi normativi: D. lgs. 33/2013, in particolare art. 23.

Vedi \ |LINK44|\  


+-------------------+----------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                 |Tipo  |Obbligo|
+===================+============================================================================+======+=======+
|Anno               |Anno di riferimento                                                         |Numero|M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE508|\      |Scegliere tra le due opzioni:                                               |Testo |O      |
|                   |                                                                            |      |       |
|                   |* Giunta                                                                    |      |       |
|                   |                                                                            |      |       |
|                   |* Consiglio                                                                 |      |       |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE509|\      |Indicare la tipologia di provvedimento tra le seguenti:                     |Testo |O      |
|                   |                                                                            |      |       |
|                   |#. Scelta del contraente per l'affidamento di lavori, forniture e servizi   |      |       |
|                   |                                                                            |      |       |
|                   |#. Accordi stipulati dall'amministrazione                                   |      |       |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE510|\      |Numero identificativo del provvedimento                                     |Numero|M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE511|\      |Titolo del provvedimento                                                    |Testo |M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE512|\      |Dispositivo del provvedimento                                               |Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE513|\      |Data di approvazione del provvedimento                                      |Data  |M      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE514|\      |Nome dell’ufficio proponente                                                |Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE515|\      |Eventuale spesa prevista                                                    |Numero|O      |
+-------------------+----------------------------------------------------------------------------+------+-------+
|\ |STYLE516|\      |Riferimenti ai documenti principali contenuti nel fascicolo del procedimento|Testo |O      |
+-------------------+----------------------------------------------------------------------------+------+-------+

.. _h2c1d74277104e41780968148427e:




.. _h2e6413415f50581d7a6f24c6b663027:

10.  TURISMO
============

.. _h39547c1c3b3b73196a1e2b15b6df56:

#32 Accompagnatori turistici (DEFINITIVO) 
------------------------------------------

\ |STYLE517|\ : Elenco degli abilitati per l’esercizio della professione di accompagnatore turistico

\ |STYLE518|\  Dataset tabellare

\ |STYLE519|\ : Tempestiva

+-------------------+-----------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                    |Tipo  |Obbligo|
+===================+===============================================+======+=======+
|Comune             |Comune di riferimento                          |Testo |M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE520|\      |Anno di riferimento                            |Numero|M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE521|\      |Cognome dell’accompagnatore turistico abilitato|Testo |M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE522|\      |Nome dell’accompagnatore turistico abilitato   |Testo |M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE523|\      |Indicare la lingua conosciuta                  |Testo |M      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE524|\      |Indicare la lingua conosciuta                  |Testo |O      |
+-------------------+-----------------------------------------------+------+-------+
|\ |STYLE525|\      |Indicare la lingua conosciuta                  |Testo |O      |
+-------------------+-----------------------------------------------+------+-------+

.. _h6e806e58126f423e6813804173126a5a:

#43 Flussi turistici (DEFINITIVO)
---------------------------------

\ |STYLE526|\ : Dati statistici sui flussi turistici

\ |STYLE527|\  Dataset tabellare

\ |STYLE528|\ : Trimestrale

+-------------------+-----------------------------------------------------------------------------+------+-------+
|Denominazione Campo|Descrizione                                                                  |Tipo  |Obbligo|
+===================+=============================================================================+======+=======+
|Anno               |Anno di riferimento                                                          |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE529|\      |Mese di riferimento                                                          |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE530|\      |Comune di riferimento                                                        |Testo |M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE531|\      |Indicare se i dati si riferiscono al settore alberghiero o extra-alberghiero |Testo |M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE532|\      |N. di arrivi di turisti italiani nel mese di riferimento                     |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE533|\      |N. di presenze di turisti italiani nel mese di riferimento                   |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE534|\      |N. di arrivi di turisti stranieri nel mese di riferimento                    |Numero|M      |
+-------------------+-----------------------------------------------------------------------------+------+-------+
|\ |STYLE535|\      |N. di presenze di turisti stranieri nel mese di riferimento                  |Numero|M      |
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
|\ |STYLE536|\      |Nome del comune dell’area                    |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE537|\      |Codice catastale del Comune                  |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE538|\      |Tipologia toponimo: Via/Piazza ecc.          |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE539|\      |Nome  Via/Piazza ecc.                        |Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE540|\      |Numero civico (compresa lettera, se presente)|Testo|M      |
+-------------------+---------------------------------------------+-----+-------+
|\ |STYLE541|\      |CAP dell’area                                |Testo|M      |
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
|\ |STYLE542|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE543|\      |Orario di apertura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE544|\      |Orario di chiusura |Testo|       |
+-------------------+-------------------+-----+-------+
|\ |STYLE545|\      |Orario di apertura |Testo|       |
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
|\ |STYLE555|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE556|\         |Orario di apertura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE557|\         |Orario di chiusura |Testo|       |
+----------------------+-------------------+-----+-------+
|\ |STYLE558|\         |Orario di apertura |Testo|       |
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

* \ |STYLE582|\  (Dati la cui frequenza non è prevedibile, ma al verificarsi del cambiamento vengono pubblicati tempestivamente)

* \ |STYLE583|\  (Dati che vengono aggiornati in tempo reale o ogni N ore)

* \ |STYLE584|\ 

* \ |STYLE585|\  

* \ |STYLE586|\ 

* \ |STYLE587|\ 

* \ |STYLE588|\ 

* \ |STYLE589|\ 

* \ |STYLE590|\ 

* \ |STYLE591|\ 

* \ |STYLE592|\  

* \ |STYLE593|\ 

* \ |STYLE594|\ 

* \ |STYLE595|\ 

* \ |STYLE596|\ 

* \ |STYLE597|\  (Dati “storici”, che per loro natura non cambiano)

* \ |STYLE598|\  (Dati soggetti a cambiamento, ma i cui processi di aggiornamento non sono ancora definiti) 

Segue tabella di conversione con le frequenze standard per il \ |STYLE599|\ 


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

.. |STYLE8| replace:: **ordinamento crescente/ decrescente dei dati**

.. |STYLE9| replace:: **rappresentazione “percentuale”**

.. |STYLE10| replace:: **rappresentazione geografica**

.. |STYLE11| replace:: **sistema di coordinate WGS-84 EPSG 4326**

.. |STYLE12| replace:: **NB:**

.. |STYLE13| replace:: **Per i dataset con frequenza di aggiornamento "tempestiva" occorre, almeno mensilmente, aggiornare i metadati.**

.. |STYLE14| replace:: **non cambia l'ultimo aggiornamento dei dati ma l'ultimo aggiornamento dei metadati**

.. |STYLE15| replace:: **Descrizione:**

.. |STYLE16| replace:: **Tipologia:**

.. |STYLE17| replace:: **Frequenza minima:**

.. |STYLE18| replace:: **Foglio**

.. |STYLE19| replace:: **Mappale**

.. |STYLE20| replace:: **Part_cat**

.. |STYLE21| replace:: **Area_fuoco**

.. |STYLE22| replace:: **Area_tot**

.. |STYLE23| replace:: **Vincoli_15**

.. |STYLE24| replace:: **Vincoli_10**

.. |STYLE25| replace:: **Vincoli_5**

.. |STYLE26| replace:: **Descrizione:**

.. |STYLE27| replace:: **Tipologia:**

.. |STYLE28| replace:: **Frequenza minima:**

.. |STYLE29| replace:: **Toponimo**

.. |STYLE30| replace:: **Indirizzo**

.. |STYLE31| replace:: **Area_mq**

.. |STYLE32| replace:: **Descrizione:**

.. |STYLE33| replace:: **Tipologia:**

.. |STYLE34| replace:: **Frequenza minima:**

.. |STYLE35| replace:: **Denominazione**

.. |STYLE36| replace:: **Tipologia**

.. |STYLE37| replace:: **Codice_catastale**

.. |STYLE38| replace:: **Comune**

.. |STYLE39| replace:: **Superficie_mq**

.. |STYLE40| replace:: **Superficie_prato**

.. |STYLE41| replace:: **Recinzione**

.. |STYLE42| replace:: **Giochi_Bambini**

.. |STYLE43| replace:: **Animali_ammessi**

.. |STYLE44| replace:: **Fontanelle**

.. |STYLE45| replace:: **Orari**

.. |STYLE46| replace:: **Descrizione:**

.. |STYLE47| replace:: **Tipologia:**

.. |STYLE48| replace:: **Frequenza minima:**

.. |STYLE49| replace:: **Nome_Impianto**

.. |STYLE50| replace:: **Codice_catastale**

.. |STYLE51| replace:: **Comune**

.. |STYLE52| replace:: **Comuni_serviti**

.. |STYLE53| replace:: **Recettore**

.. |STYLE54| replace:: **Altezza**

.. |STYLE55| replace:: **Indirizzo**

.. |STYLE56| replace:: **Longitude**

.. |STYLE57| replace:: **Latitude**

.. |STYLE58| replace:: **Data_avvio**

.. |STYLE59| replace:: **Descrizione:**

.. |STYLE60| replace:: **Tipologia:**

.. |STYLE61| replace:: **Frequenza minima:**

.. |STYLE62| replace:: **Macro_Categoria_Rifiuti**

.. |STYLE63| replace:: **Categoria_Rifiuti**

.. |STYLE64| replace:: **ID_Categoria_Rifiuti**

.. |STYLE65| replace:: **Modalità_Raccolta**

.. |STYLE66| replace:: **Periodo**

.. |STYLE67| replace:: **Quantità**

.. |STYLE68| replace:: **Descrizione:**

.. |STYLE69| replace:: **Tipologia:**

.. |STYLE70| replace:: **Frequenza minima:**

.. |STYLE71| replace:: **Codice_Pratica**

.. |STYLE72| replace:: **Richiedente**

.. |STYLE73| replace:: **Protocollo**

.. |STYLE74| replace:: **Oggetto_Richiesta**

.. |STYLE75| replace:: **Data_Richiesta**

.. |STYLE76| replace:: **Link_pratica**

.. |STYLE77| replace:: **Descrizione:**

.. |STYLE78| replace:: **Tipologia:**

.. |STYLE79| replace:: **Frequenza minima:**

.. |STYLE80| replace:: **Ubicazione**

.. |STYLE81| replace:: **Tipologia**

.. |STYLE82| replace:: **Superficie**

.. |STYLE83| replace:: **Superficie_Altro**

.. |STYLE84| replace:: **Orari**

.. |STYLE85| replace:: **Longitude**

.. |STYLE86| replace:: **Latitude**

.. |STYLE87| replace:: **Descrizione**

.. |STYLE88| replace:: **Tipologia:**

.. |STYLE89| replace:: **Frequenza minima**

.. |STYLE90| replace:: **Ubicazione**

.. |STYLE91| replace:: **Tipo_Esercizio**

.. |STYLE92| replace:: **Tipo_Somministrazione**

.. |STYLE93| replace:: **Modalità_Somministrazione**

.. |STYLE94| replace:: **Superficie**

.. |STYLE95| replace:: **WiFi**

.. |STYLE96| replace:: **Longitude**

.. |STYLE97| replace:: **Latitude**

.. |STYLE98| replace:: **Orari**

.. |STYLE99| replace:: **Descrizione**

.. |STYLE100| replace:: **Tipologia:**

.. |STYLE101| replace:: **Frequenza minima**

.. |STYLE102| replace:: **Periodo_Rif**

.. |STYLE103| replace:: **Denominazione**

.. |STYLE104| replace:: **Tipo**

.. |STYLE105| replace:: **N_Edizione**

.. |STYLE106| replace:: **Descrizione**

.. |STYLE107| replace:: **Data_Inizio**

.. |STYLE108| replace:: **Ora_Inizio**

.. |STYLE109| replace:: **Data_Fine**

.. |STYLE110| replace:: **Ora_Fine**

.. |STYLE111| replace:: **Sito_Web**

.. |STYLE112| replace:: **Programma**

.. |STYLE113| replace:: **Nome_Organizzatore**

.. |STYLE114| replace:: **Email_Organizzatore**

.. |STYLE115| replace:: **Telefono_Organizzatore**

.. |STYLE116| replace:: **Gratuito**

.. |STYLE117| replace:: **Prezzo**

.. |STYLE118| replace:: **Longitude**

.. |STYLE119| replace:: **Latitude**

.. |STYLE120| replace:: **Descrizione**

.. |STYLE121| replace:: **Tipologia:**

.. |STYLE122| replace:: **Frequenza minima**

.. |STYLE123| replace:: **Nome**

.. |STYLE124| replace:: **Descrizione**

.. |STYLE125| replace:: **Tipologia**

.. |STYLE126| replace:: **Ubicazione**

.. |STYLE127| replace:: **Email**

.. |STYLE128| replace:: **Telefono**

.. |STYLE129| replace:: **Sito_web**

.. |STYLE130| replace:: **Note**

.. |STYLE131| replace:: **Longitude**

.. |STYLE132| replace:: **Latitude**

.. |STYLE133| replace:: **Descrizione**

.. |STYLE134| replace:: **Tipologia:**

.. |STYLE135| replace:: **Frequenza minima**

.. |STYLE136| replace:: **Ubicazione**

.. |STYLE137| replace:: **Telefono**

.. |STYLE138| replace:: **Email**

.. |STYLE139| replace:: **Descrizione**

.. |STYLE140| replace:: **Tipologia:**

.. |STYLE141| replace:: **Frequenza minima**

.. |STYLE142| replace:: **Descrizione**

.. |STYLE143| replace:: **Tipologia:**

.. |STYLE144| replace:: **Frequenza minima**

.. |STYLE145| replace:: **Periodo**

.. |STYLE146| replace:: **Dettagli**

.. |STYLE147| replace:: **Descrizione**

.. |STYLE148| replace:: **Tipologia:**

.. |STYLE149| replace:: **Frequenza minima**

.. |STYLE150| replace:: **Tipo**

.. |STYLE151| replace:: **Orari**

.. |STYLE152| replace:: **Deroghe**

.. |STYLE153| replace:: **Longitude**

.. |STYLE154| replace:: **Latitude**

.. |STYLE155| replace:: **Link**

.. |STYLE156| replace:: **Descrizione**

.. |STYLE157| replace:: **Tipologia:**

.. |STYLE158| replace:: **Frequenza minima**

.. |STYLE159| replace:: **Tipologia**

.. |STYLE160| replace:: **Ubicazione**

.. |STYLE161| replace:: **Orari**

.. |STYLE162| replace:: **Longitude**

.. |STYLE163| replace:: **Latitude**

.. |STYLE164| replace:: **Gratuito**

.. |STYLE165| replace:: **Descrizione**

.. |STYLE166| replace:: **Tipologia:**

.. |STYLE167| replace:: **Frequenza minima**

.. |STYLE168| replace:: **Descr**

.. |STYLE169| replace:: **Tipologia**

.. |STYLE170| replace:: **Sede**

.. |STYLE171| replace:: **Fondo**

.. |STYLE172| replace:: **Lung**

.. |STYLE173| replace:: **Larg**

.. |STYLE174| replace:: **Direzione**

.. |STYLE175| replace:: **Stato**

.. |STYLE176| replace:: **Ambito**

.. |STYLE177| replace:: **Descrizione**

.. |STYLE178| replace:: **Tipologia:**

.. |STYLE179| replace:: **Frequenza minima**

.. |STYLE180| replace:: **Tipo_Area**

.. |STYLE181| replace:: **Toponimo**

.. |STYLE182| replace:: **Indirizzo**

.. |STYLE183| replace:: **Descrizione**

.. |STYLE184| replace:: **Tipologia:**

.. |STYLE185| replace:: **Frequenza minima**

.. |STYLE186| replace:: **Toponimo**

.. |STYLE187| replace:: **Indirizzo**

.. |STYLE188| replace:: **Descrizione**

.. |STYLE189| replace:: **Tipologia:**

.. |STYLE190| replace:: **Frequenza minima**

.. |STYLE191| replace:: **Ubicazione**

.. |STYLE192| replace:: **Latitude**

.. |STYLE193| replace:: **Longitude**

.. |STYLE194| replace:: **N_Bici**

.. |STYLE195| replace:: **Note**

.. |STYLE196| replace:: **Descrizione**

.. |STYLE197| replace:: **Tipologia:**

.. |STYLE198| replace:: **Frequenza minima**

.. |STYLE199| replace:: **Ubicazione**

.. |STYLE200| replace:: **Telefono**

.. |STYLE201| replace:: **Email**

.. |STYLE202| replace:: **Descrizione**

.. |STYLE203| replace:: **Tipologia:**

.. |STYLE204| replace:: **Frequenza minima**

.. |STYLE205| replace:: **Ubicazione**

.. |STYLE206| replace:: **Stalli**

.. |STYLE207| replace:: **Longitude**

.. |STYLE208| replace:: **Latitude**

.. |STYLE209| replace:: **Descrizione**

.. |STYLE210| replace:: **Tipologia:**

.. |STYLE211| replace:: **Frequenza minima**

.. |STYLE212| replace:: **Ubicazione**

.. |STYLE213| replace:: **KW**

.. |STYLE214| replace:: **Modalità_Utilizzo**

.. |STYLE215| replace:: **Tipo_Presa**

.. |STYLE216| replace:: **Veicoli**

.. |STYLE217| replace:: **Data_Attivazione**

.. |STYLE218| replace:: **Longitude**

.. |STYLE219| replace:: **Latitude**

.. |STYLE220| replace:: **Descrizione**

.. |STYLE221| replace:: **Tipologia**

.. |STYLE222| replace:: **Frequenza minima**

.. |STYLE223| replace:: **Data**

.. |STYLE224| replace:: **Ora**

.. |STYLE225| replace:: **Località**

.. |STYLE226| replace:: **Natura_Incidente**

.. |STYLE227| replace:: **N_Illesi**

.. |STYLE228| replace:: **N_Feriti**

.. |STYLE229| replace:: **N_Morti**

.. |STYLE230| replace:: **Pedoni**

.. |STYLE231| replace:: **Velocipedi**

.. |STYLE232| replace:: **Ciclomotori_Motocicli**

.. |STYLE233| replace:: **Mezzi_pesanti**

.. |STYLE234| replace:: **Longitude**

.. |STYLE235| replace:: **Latitude**

.. |STYLE236| replace:: **Descrizione**

.. |STYLE237| replace:: **Tipologia:**

.. |STYLE238| replace:: **Frequenza minima**

.. |STYLE239| replace:: **Tipo_Infrazione**

.. |STYLE240| replace:: **Normativa**

.. |STYLE241| replace:: **Art.**

.. |STYLE242| replace:: **Data**

.. |STYLE243| replace:: **Tipo_Veicolo**

.. |STYLE244| replace:: **Ubicazione**

.. |STYLE245| replace:: **N_Sanzioni**

.. |STYLE246| replace:: **Longitude**

.. |STYLE247| replace:: **Latitude**

.. |STYLE248| replace:: **Descrizione**

.. |STYLE249| replace:: **Tipologia:**

.. |STYLE250| replace:: **Frequenza minima**

.. |STYLE251| replace:: **Provvedimento**

.. |STYLE252| replace:: **Controlli**

.. |STYLE253| replace:: **Verbali**

.. |STYLE254| replace:: **Descrizione**

.. |STYLE255| replace:: **Tipologia:**

.. |STYLE256| replace:: **Frequenza minima**

.. |STYLE257| replace:: **Tipo**

.. |STYLE258| replace:: **Controlli**

.. |STYLE259| replace:: **Verbali**

.. |STYLE260| replace:: **Descrizione**

.. |STYLE261| replace:: **Tipologia:**

.. |STYLE262| replace:: **Frequenza minima**

.. |STYLE263| replace:: **Tornata_elettorale**

.. |STYLE264| replace:: **Collegio_elettorale**

.. |STYLE265| replace:: **Sezione**

.. |STYLE266| replace:: **Soggetto_votato**

.. |STYLE267| replace:: **Voto**

.. |STYLE268| replace:: **N_Voti**

.. |STYLE269| replace:: **Descrizione**

.. |STYLE270| replace:: **Tipologia:**

.. |STYLE271| replace:: **Frequenza minima**

.. |STYLE272| replace:: **Tornata_elettorale**

.. |STYLE273| replace:: **Collegio_elettorale**

.. |STYLE274| replace:: **Sezione**

.. |STYLE275| replace:: **Soggetto_votato**

.. |STYLE276| replace:: **Voto**

.. |STYLE277| replace:: **N_Voti**

.. |STYLE278| replace:: **Descrizione**

.. |STYLE279| replace:: **Tipologia:**

.. |STYLE280| replace:: **Frequenza minima**

.. |STYLE281| replace:: **Tornata_elettorale**

.. |STYLE282| replace:: **Collegio_elettorale**

.. |STYLE283| replace:: **Sezione**

.. |STYLE284| replace:: **Soggetto_votato**

.. |STYLE285| replace:: **Voto**

.. |STYLE286| replace:: **N_Voti**

.. |STYLE287| replace:: **Descrizione**

.. |STYLE288| replace:: **Tipologia:**

.. |STYLE289| replace:: **Frequenza minima**

.. |STYLE290| replace:: **Tornata_Elettorale**

.. |STYLE291| replace:: **Tipo_Elezione**

.. |STYLE292| replace:: **Soggetto_votato**

.. |STYLE293| replace:: **Collegio_elettorale**

.. |STYLE294| replace:: **Sezione**

.. |STYLE295| replace:: **Voto**

.. |STYLE296| replace:: **N_Voti**

.. |STYLE297| replace:: **Descrizione**

.. |STYLE298| replace:: **Tipologia:**

.. |STYLE299| replace:: **Frequenza minima**

.. |STYLE300| replace:: **Condizione**

.. |STYLE301| replace:: **Maschi**

.. |STYLE302| replace:: **Femmine**

.. |STYLE303| replace:: **Descrizione**

.. |STYLE304| replace:: **Tipologia:**

.. |STYLE305| replace:: **Frequenza minima**

.. |STYLE306| replace:: **Indirizzo**

.. |STYLE307| replace:: **Località**

.. |STYLE308| replace:: **S_marcia**

.. |STYLE309| replace:: **Civico_inizio**

.. |STYLE310| replace:: **Civico_fine**

.. |STYLE311| replace:: **Descrizione**

.. |STYLE312| replace:: **Tipologia:**

.. |STYLE313| replace:: **Frequenza minima**

.. |STYLE314| replace:: **Nome_Toponimo**

.. |STYLE315| replace:: **Codice_Toponimo**

.. |STYLE316| replace:: **Storico**

.. |STYLE317| replace:: **Descrizione**

.. |STYLE318| replace:: **Tipologia:**

.. |STYLE319| replace:: **Frequenza minima**

.. |STYLE320| replace:: **Nome_Toponimo**

.. |STYLE321| replace:: **Numero**

.. |STYLE322| replace:: **Subalterno**

.. |STYLE323| replace:: **CAP**

.. |STYLE324| replace:: **Sezione_ISTAT**

.. |STYLE325| replace:: **Longitude**

.. |STYLE326| replace:: **Latitude**

.. |STYLE327| replace:: **Descrizione**

.. |STYLE328| replace:: **Tipologia:**

.. |STYLE329| replace:: **Frequenza minima**

.. |STYLE330| replace:: **Indirizzo**

.. |STYLE331| replace:: **Descrizione**

.. |STYLE332| replace:: **Data_Inizio**

.. |STYLE333| replace:: **Data_Fine**

.. |STYLE334| replace:: **Descrizione**

.. |STYLE335| replace:: **Tipologia:**

.. |STYLE336| replace:: **Frequenza minima**

.. |STYLE337| replace:: **ID_Accesso**

.. |STYLE338| replace:: **Tipologia_Accesso**

.. |STYLE339| replace:: **Sito**

.. |STYLE340| replace:: **Attivo**

.. |STYLE341| replace:: **Codice**

.. |STYLE342| replace:: **Longitude**

.. |STYLE343| replace:: **Latitude**

.. |STYLE344| replace:: **Raggio_Copertura_m**

.. |STYLE345| replace:: **Descrizione**

.. |STYLE346| replace:: **Tipologia:**

.. |STYLE347| replace:: **Frequenza minima**

.. |STYLE348| replace:: **Comune**

.. |STYLE349| replace:: **Toponimo**

.. |STYLE350| replace:: **Indirizzo**

.. |STYLE351| replace:: **Area_mq**

.. |STYLE352| replace:: **Fontane**

.. |STYLE353| replace:: **Attrezzi**

.. |STYLE354| replace:: **Panchine**

.. |STYLE355| replace:: **Descrizione**

.. |STYLE356| replace:: **Tipologia:**

.. |STYLE357| replace:: **Frequenza minima**

.. |STYLE358| replace:: **Tipologia**

.. |STYLE359| replace:: **ID_Istanza**

.. |STYLE360| replace:: **Data_Istanza**

.. |STYLE361| replace:: **Protocollo**

.. |STYLE362| replace:: **N_Provvedimento**

.. |STYLE363| replace:: **Data_Provvedimento**

.. |STYLE364| replace:: **Richiedente**

.. |STYLE365| replace:: **\***

.. |STYLE366| replace:: **Descrizione_ Intervento**

.. |STYLE367| replace:: **Codice_ecografico**

.. |STYLE368| replace:: **Descrizione**

.. |STYLE369| replace:: **Tipologia:**

.. |STYLE370| replace:: **Frequenza minima**

.. |STYLE371| replace:: **Tipologia**

.. |STYLE372| replace:: **Ubicazione**

.. |STYLE373| replace:: **Superficie_mq**

.. |STYLE374| replace:: **Assegnatario**

.. |STYLE375| replace:: **Progetto**

.. |STYLE376| replace:: **Destinazione_d’uso**

.. |STYLE377| replace:: **Atto_Concessione**

.. |STYLE378| replace:: **Data**

.. |STYLE379| replace:: **Durata_Anni**

.. |STYLE380| replace:: **Descrizione**

.. |STYLE381| replace:: **Tipologia:**

.. |STYLE382| replace:: **Frequenza minima**

.. |STYLE383| replace:: **Tipologia**

.. |STYLE384| replace:: **Ubicazione**

.. |STYLE385| replace:: **Telefono**

.. |STYLE386| replace:: **Descrizione**

.. |STYLE387| replace:: **Tipologia:**

.. |STYLE388| replace:: **Frequenza minima**

.. |STYLE389| replace:: **Numero_Provvedimento**

.. |STYLE390| replace:: **Data**

.. |STYLE391| replace:: **Beneficiario**

.. |STYLE392| replace:: **Tipologia_Beneficiario**

.. |STYLE393| replace:: **Codice_fiscale**

.. |STYLE394| replace:: **Partita_IVA**

.. |STYLE395| replace:: **Oggetto**

.. |STYLE396| replace:: **Norma_Titolo**

.. |STYLE397| replace:: **Link_Norma_Titolo**

.. |STYLE398| replace:: **Ufficio**

.. |STYLE399| replace:: **Cognome_Responsabile**

.. |STYLE400| replace:: **Nome_Responsabile**

.. |STYLE401| replace:: **Modalità**

.. |STYLE402| replace:: **Importo**

.. |STYLE403| replace:: **Progetto**

.. |STYLE404| replace:: **Link_Progetto**

.. |STYLE405| replace:: **Curriculum**

.. |STYLE406| replace:: **Descrizione**

.. |STYLE407| replace:: **Tipologia:**

.. |STYLE408| replace:: **Frequenza minima**

.. |STYLE409| replace:: **Tipologia_Locazione**

.. |STYLE410| replace:: **Locatario**

.. |STYLE411| replace:: **Locatore**

.. |STYLE412| replace:: **Ubicazione**

.. |STYLE413| replace:: **Destinazione**

.. |STYLE414| replace:: **Data_Inizio_Contratto**

.. |STYLE415| replace:: **Data_Fine_Contratto**

.. |STYLE416| replace:: **Canone_percepito**

.. |STYLE417| replace:: **Spese_accessorie**

.. |STYLE418| replace:: **Canone_versato**

.. |STYLE419| replace:: **Descrizione**

.. |STYLE420| replace:: **Tipologia:**

.. |STYLE421| replace:: **Frequenza minima**

.. |STYLE422| replace:: **Descrizione**

.. |STYLE423| replace:: **Natura_giuridica**

.. |STYLE424| replace:: **Tipologia_Bene**

.. |STYLE425| replace:: **Categoria_catastale**

.. |STYLE426| replace:: **Sezione**

.. |STYLE427| replace:: **Foglio**

.. |STYLE428| replace:: **Mappale**

.. |STYLE429| replace:: **Subalterno**

.. |STYLE430| replace:: **Classe**

.. |STYLE431| replace:: **Unità**

.. |STYLE432| replace:: **Consistenza**

.. |STYLE433| replace:: **Rendita**

.. |STYLE434| replace:: **Destinazione**

.. |STYLE435| replace:: **Superficie**

.. |STYLE436| replace:: **Valore**

.. |STYLE437| replace:: **Data_Acquisizione**

.. |STYLE438| replace:: **Longitude**

.. |STYLE439| replace:: **Latitude**

.. |STYLE440| replace:: **Descrizione**

.. |STYLE441| replace:: **Tipologia:**

.. |STYLE442| replace:: **Frequenza minima**

.. |STYLE443| replace:: **Titolo**

.. |STYLE444| replace:: **Descrizione**

.. |STYLE445| replace:: **Termine_massimo**

.. |STYLE446| replace:: **Tempi_effettivi**

.. |STYLE447| replace:: **Ufficio_Responsabile**

.. |STYLE448| replace:: **Note**

.. |STYLE449| replace:: **Descrizione**

.. |STYLE450| replace:: **Tipologia:**

.. |STYLE451| replace:: **Frequenza minima**

.. |STYLE452| replace:: **Funzioni_attribuite**

.. |STYLE453| replace:: **Attività_svolte**

.. |STYLE454| replace:: **Quota_Partecipazione**

.. |STYLE455| replace:: **Durata_Impegno**

.. |STYLE456| replace:: **Onere_Impegno**

.. |STYLE457| replace:: **Numero_Rappresentanti**

.. |STYLE458| replace:: **Trattamento_economico**

.. |STYLE459| replace:: **Ultimo_anno**

.. |STYLE460| replace:: **Risultati_Bilancio_Ultimo_anno**

.. |STYLE461| replace:: **Risultati_Bilancio_Penultimo_anno**

.. |STYLE462| replace:: **Risultati_Bilancio_Terzultimo_anno**

.. |STYLE463| replace:: **Sito_istituzionale**

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

.. |STYLE497| replace:: **Tipologia_ Provvedimento**

.. |STYLE498| replace:: **Numero_ Provvedimento**

.. |STYLE499| replace:: **Oggetto**

.. |STYLE500| replace:: **Contenuto**

.. |STYLE501| replace:: **Data_Approvazione**

.. |STYLE502| replace:: **Ufficio_proponente**

.. |STYLE503| replace:: **Spesa_prevista**

.. |STYLE504| replace:: **Estremi_Documenti_ Fascicolo**

.. |STYLE505| replace:: **Descrizione**

.. |STYLE506| replace:: **Tipologia:**

.. |STYLE507| replace:: **Frequenza minima**

.. |STYLE508| replace:: **Organo**

.. |STYLE509| replace:: **Tipologia_ Provvedimento**

.. |STYLE510| replace:: **Numero_ Provvedimento**

.. |STYLE511| replace:: **Oggetto**

.. |STYLE512| replace:: **Contenuto**

.. |STYLE513| replace:: **Data_Approvazione**

.. |STYLE514| replace:: **Ufficio proponente**

.. |STYLE515| replace:: **Spesa_prevista**

.. |STYLE516| replace:: **Estremi_Documenti_ Fascicolo**

.. |STYLE517| replace:: **Descrizione**

.. |STYLE518| replace:: **Tipologia:**

.. |STYLE519| replace:: **Frequenza minima**

.. |STYLE520| replace:: **Anno**

.. |STYLE521| replace:: **Cognome**

.. |STYLE522| replace:: **Nome**

.. |STYLE523| replace:: **Lingua 1**

.. |STYLE524| replace:: **Lingua 2**

.. |STYLE525| replace:: **Lingua n**

.. |STYLE526| replace:: **Descrizione**

.. |STYLE527| replace:: **Tipologia:**

.. |STYLE528| replace:: **Frequenza minima**

.. |STYLE529| replace:: **Mese**

.. |STYLE530| replace:: **Comune**

.. |STYLE531| replace:: **Settore**

.. |STYLE532| replace:: **Arrivi_italiani**

.. |STYLE533| replace:: **Presenze_italiani**

.. |STYLE534| replace:: **Arrivi_stranieri**

.. |STYLE535| replace:: **Presenze_stranieri**

.. |STYLE536| replace:: **Comune**

.. |STYLE537| replace:: **Codice_catastale**

.. |STYLE538| replace:: **Toponimo**

.. |STYLE539| replace:: **Indirizzo**

.. |STYLE540| replace:: **Civico**

.. |STYLE541| replace:: **CAP**

.. |STYLE542| replace:: **Lun_Chiusura**

.. |STYLE543| replace:: **Mar_Apertura**

.. |STYLE544| replace:: **Mar_Chiusura**

.. |STYLE545| replace:: **Mer_Apertura**

.. |STYLE546| replace:: **Mer_Chiusura**

.. |STYLE547| replace:: **Gio_Apertura**

.. |STYLE548| replace:: **Gio_Chiusura**

.. |STYLE549| replace:: **Ven_Apertura**

.. |STYLE550| replace:: **Ven_Chiusura**

.. |STYLE551| replace:: **Sab_Apertura**

.. |STYLE552| replace:: **Sab_Chiusura**

.. |STYLE553| replace:: **Dom_Apertura**

.. |STYLE554| replace:: **Dom_Chiusura**

.. |STYLE555| replace:: **Invernale_Lun_Chiusura**

.. |STYLE556| replace:: **Invernale_Mar_Apertura**

.. |STYLE557| replace:: **Invernale_Mar_Chiusura**

.. |STYLE558| replace:: **Invernale_Mer_Apertura**

.. |STYLE559| replace:: **Invernale_Mer_Chiusura**

.. |STYLE560| replace:: **Invernale_Gio_Apertura**

.. |STYLE561| replace:: **Invernale_Gio_Chiusura**

.. |STYLE562| replace:: **Invernale_Ven_Apertura**

.. |STYLE563| replace:: **Invernale_Ven_Chiusura**

.. |STYLE564| replace:: **Invernale_Sab_Apertura**

.. |STYLE565| replace:: **Invernale_Sab_Chiusura**

.. |STYLE566| replace:: **Invernale_Dom_Apertura**

.. |STYLE567| replace:: **Invernale_Dom_Chiusura**

.. |STYLE568| replace:: **Estivo_Lun_Apertura**

.. |STYLE569| replace:: **Estivo_Lun_Chiusura**

.. |STYLE570| replace:: **Estivo_Mar_Apertura**

.. |STYLE571| replace:: **Estivo_Mar_Chiusura**

.. |STYLE572| replace:: **Estivo_Mer_Apertura**

.. |STYLE573| replace:: **Estivo_Mer_Chiusura**

.. |STYLE574| replace:: **Estivo_Gio_Apertura**

.. |STYLE575| replace:: **Estivo_Gio_Chiusura**

.. |STYLE576| replace:: **Estivo_Ven_Apertura**

.. |STYLE577| replace:: **Estivo_Ven_Chiusura**

.. |STYLE578| replace:: **Estivo_Sab_Apertura**

.. |STYLE579| replace:: **Estivo_Sab_Chiusura**

.. |STYLE580| replace:: **Estivo_Dom_Apertura**

.. |STYLE581| replace:: **Estivo_Dom_Chiusura**

.. |STYLE582| replace:: **Tempestiva**

.. |STYLE583| replace:: **Tempo reale**

.. |STYLE584| replace:: **Giornaliera**

.. |STYLE585| replace:: **Settimanale**

.. |STYLE586| replace:: **Quindicinale**

.. |STYLE587| replace:: **Mensile**

.. |STYLE588| replace:: **Bimestrale**

.. |STYLE589| replace:: **Trimestrale**

.. |STYLE590| replace:: **Quadrimestrale**

.. |STYLE591| replace:: **Semestrale**

.. |STYLE592| replace:: **Annuale**

.. |STYLE593| replace:: **Biennale**

.. |STYLE594| replace:: **Triennale**

.. |STYLE595| replace:: **Quinquennale**

.. |STYLE596| replace:: **Decennale**

.. |STYLE597| replace:: **Mai**

.. |STYLE598| replace:: **Non definita**

.. |STYLE599| replace:: **DCAT-AP_IT**


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

