
.. _h4e7866c692d53746f521a302b4465d:

Ontologia FOAF ``RDF``
######################

\ |STYLE0|\ 

|REPLACE1|

\ |LINK1|\ 

È un modo per descrivere te stesso -- il tuo nome, l'indirizzo di posta elettronica, ed i tuoi amici -- usando ``XML``  e ``RDF``. Ciò consente ad un software di elaborare queste descrizioni, magari all'interno di un motore di ricerca automatico, allo scopo di trovare informazioni su di te e sulle comunità delle quali fai parte. FOAF può portare a nuove interessanti possibilità di sviluppo per le comunità online.

Copia semplicemente la descrizione FOAF che hai generato e incollala in un file. Pubblica questo file sul tuo sito web: è una buona idea chiamare questo file "\ |LINK2|\ ", in modo da permettere l'uso di una ricerca con Google per trovare file FOAF sul web.

[\ |LINK3|\ ]  [\ |LINK4|\ ]


.. code:: 

    <rdf:RDF
          xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
          xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#"
          xmlns:foaf="http://xmlns.com/foaf/0.1/"
          xmlns:admin="http://webns.net/mvcb/">
    <foaf:PersonalProfileDocument rdf:about="">
      <foaf:maker rdf:resource="#me"/>
      <foaf:primaryTopic rdf:resource="#me"/>
      <admin:generatorAgent rdf:resource="http://www.ldodds.com/foaf/foaf-a-matic"/>
      <admin:errorReportsTo rdf:resource="mailto:leigh@ldodds.com"/>
    </foaf:PersonalProfileDocument>
    <foaf:Person rdf:ID="me">
    <foaf:name>Ciro Spataro</foaf:name>
    <foaf:title>Sig.</foaf:title>
    <foaf:givenname>Ciro</foaf:givenname>
    <foaf:family_name>Spataro</foaf:family_name>
    <foaf:nick>cirospat</foaf:nick>
    <foaf:mbox_sha1sum>5c633d4ff63c096445cc161d60edbdb2ec295ad8</foaf:mbox_sha1sum>
    <foaf:homepage rdf:resource="https://cirospat.readthedocs.io"/>
    <foaf:depiction rdf:resource="https://cirospat.readthedocs.io/it/latest/_static/cirospat.jpg"/>
    <foaf:phone rdf:resource="tel:3333779425"/>
    <foaf:workplaceHomepage rdf:resource="https://www.comune.palermo.it/unita.php?apt=4&uo=1770&serv=394&sett=138"/>
    <foaf:workInfoHomepage rdf:resource="https://cirospat.readthedocs.io"/>
    <foaf:knows>
    <foaf:Person>
    <foaf:name>Giovanni</foaf:name>
    <foaf:mbox_sha1sum>bbaed82f0fd2509e45f8139df85b0d3deafcd38d</foaf:mbox_sha1sum></foaf:Person></foaf:knows>
    <foaf:knows>
    <foaf:Person>
    <foaf:name>Andrea</foaf:name>
    <foaf:mbox_sha1sum>7ea3b92d200233d2b8a4455a31f1e097e8cc6162</foaf:mbox_sha1sum></foaf:Person></foaf:knows>
    <foaf:knows>
    <foaf:Person>
    <foaf:name>Davide</foaf:name>
    <foaf:mbox_sha1sum>e1607678ab8d0d0b24f3bd42abb9278ea26cd2fc</foaf:mbox_sha1sum></foaf:Person></foaf:knows>
    <foaf:knows>
    <foaf:Person>
    <foaf:name>Giorgia</foaf:name>
    <foaf:mbox_sha1sum>17dd6d7cfaff0f1127f1c032c497d0ee853c7b1f</foaf:mbox_sha1sum></foaf:Person></foaf:knows>
    <foaf:knows>
    <foaf:Person>
    <foaf:name>Giovanna Roberta</foaf:name>
    <foaf:mbox_sha1sum>30aab1a18394b61d9f68eee616c09084337ceea2</foaf:mbox_sha1sum></foaf:Person></foaf:knows></foaf:Person>
    </rdf:RDF>

Da un \ |LINK5|\ . 

|REPLACE2|


+----------------------------------------------------------------------------------+
|Immagine in alto: \ |LINK6|\ . Pubblicato dal Metmuseum con Licenza Public Domain.|
+----------------------------------------------------------------------------------+


|REPLACE3|


.. bottom of content


.. |STYLE0| replace:: **FOAF (Friend Of A Friend)**


.. |REPLACE1| raw:: html

    <img src="https://collectionapi.metmuseum.org/api/collection/v1/iiif/392571/769337/main-image" width="500" />
.. |REPLACE2| raw:: html

    <img src="https://raw.githubusercontent.com/cirospat/newproject/master/docs/static/foaf.PNG" />
.. |REPLACE3| raw:: html

    <script id="dsq-count-scr" src="//guida-readthedocs.disqus.com/count.js" async></script>
    
    <div id="disqus_thread"></div>
    <script>
    
    /**
    *  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
    *  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables*/
    /*
    
    var disqus_config = function () {
    this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
    this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
    };
    */
    (function() { // DON'T EDIT BELOW THIS LINE
    var d = document, s = d.createElement('script');
    s.src = 'https://guida-readthedocs.disqus.com/embed.js';
    s.setAttribute('data-timestamp', +new Date());
    (d.head || d.body).appendChild(s);
    })();
    </script>
    <noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>

.. |LINK1| raw:: html

    <a href="http://www.ldodds.com/foaf/foaf-a-matic.it.html" target="_blank">Friend Of A Friend</a>

.. |LINK2| raw:: html

    <a href="https://raw.githubusercontent.com/cirospat/newproject/master/docs/foaf.rdf" target="_blank">foaf.rdf</a>

.. |LINK3| raw:: html

    <a href="https://www.w3.org/XML/" target="_blank">XML</a>

.. |LINK4| raw:: html

    <a href="https://www.w3.org/RDF/" target="_blank">RDF</a>

.. |LINK5| raw:: html

    <a href="https://twitter.com/gpirrotta/status/1055845619019980801" target="_blank">input didattico di Giovanni Pirrotta</a>

.. |LINK6| raw:: html

    <a href="https://www.metmuseum.org/art/collection/search/392571" target="_blank">John Bull and His Friends Commemorating the Peace</a>

