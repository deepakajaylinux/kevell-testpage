========
Dnsify
========

Zusammenfassung
-------------------------

Diese Module Umschläge alle wichtigen Bedürfnisse der Anwender die Verwaltung DNS. Dieses Thema ist es, wie Sie dieses Modul verwenden zu diskutieren und über verschiedene Funktionen bei der Verwendung dnsify.


Hilfe Befehl
-------------------

Der Befehl help führt den Anwender beim Umgang mit diesem Modul, um zu handhaben und führen verschiedene Funktionen aus einer Box. Es listet outs die alternativen Parameter, und hebt die Syntax für die verschiedenen Funktionen der Verwendung und Modifizierung einer Box. Die Syntax für die Hilfe-Option unter dem dnsify Moduls ist unten dargestellt,

.. code-block:: bash

	cleopatra DNSify help


The syntax for declaring the help command is not case sensitive which is an added advantage. The following screenshot visualize you about the help command under dnsify.

.. code-block:: bash

 kevell@corp:/# cleopatra Dnsify help 
 ****************************** 


  This command provides a generic Box Management wrapper around all of the Box Providers (Cloud and Otherwise) so that we have a 
  generic way to create and destroy boxes. 

  DNSify, dnsify 

        - install-generic-autopilots 
        Install the generic Dnsify autopilot templates for a Tiny or Medium (Current Default) set of Environments 
        example: cleopatra dnsify install-generic-autopilots 
        example: cleopatra dnsify install-generic-autopilots 
                    --yes 
                    --guess # will set --destination-dir=*this dir +*build/config/cleopatra/dnsify/autopilots/ 
                    --template-group=tiny 
                    --destination-dir=*path-to-destination* 

        - box-add 
        Installs a Box through a cloud provider 
        example: cleopatra dnsify box-add --environment-name="*environment*" 
            --server-prefix="my-app" 
            --provider="DigitalOcean" // DigitalOcean, Rackspace, VSphere 
            --image-id="3101045" // DO=3101045 , RAX=ffd597d6-2cc4-4b43-b8f4-b1006715b84e 
            --size-id="66" // DO = 66, RAX = 2 
            --region-id="2" // DO = 2, RAX = LON 
            --box-amount=1 // An Integer number of boxes to create 
            --force-name="a-box-name" // optional, will override other options for name creation. may cause a conflict if creating more than 1 box. 
            --parallax // optional, when adding more than one box, if the provider supports it we can execute all requests in parallel 

        - box-remove 
        Removes a Box from the papyrus 
        example: cleopatra dnsify box-remove --environment-name="staging" --environment-version="5.0" --provider="apt-get" 

        - box-destroy 
        Removes a Box from both papyrus and the cloud provider 
        example: cleopatra dnsify box-destroy --environment-name="staging" 
            --destroy-all-boxes 
            --destroy 

        - list-papyrus 
        List all servers in papyrus, or those of a particular environment 
        example: cleopatra dnsify list-papyrus --yes 
        example: cleopatra dnsify list-papyrus --yes --environment-name="staging" 


 ------------------------------ 
 End Help 
 ****************************** 

Verschiedene Funktionen der dnsify
-------------------------------------


Diese Themen beschrieben über die verschiedenen Funktionen dnsify unter diesem Modul, wie nachstehend aufgeführt


* Installieren Sie generische Autopiloten
* Hinzufügen Box
* Entfernen Box
* Löschen einer Box
* Liste


Installieren Sie generische Autopiloten
-------------------------------------------

Diese Funktion soll die Installation geltenden Autopiloten zu einem kleinen oder mittleren Reihe von Umgebungen. Dies kann durch den Befehl, wie unten angegeben durchgeführt werden,

.. code-block:: bash
	
	cleopatra dnsify install-generic-autopilots 
                    --yes 
                    --guess # will set --destination-dir=*this dir +*build/config/cleopatra/dnsify/autopilots/ 
                    --template-group=tiny 
                    --destination-dir=*path-to-destination* 


Wie in der oben genannten Syntax dargestellt der Benutzer müssen Sie die folgenden Felder, um die generische Autopiloten installiert werden 
soll.

* Zielverzeichnis
* Template-Gruppe


Hinzufügen Box
-----------------

Diese Funktion soll das Hinzufügen einer Box über einen Cloud-Anbieter, indem Sie einfach mit dem folgenden Befehl

.. code-block:: bash

 example: cleopatra dnsify box-add --environment-name="*environment*" 
            --server-prefix="my-app" 
            --provider="DigitalOcean" // DigitalOcean, Rackspace, VSphere 
            --image-id="3101045" // DO=3101045 , RAX=ffd597d6-2cc4-4b43-b8f4-b1006715b84e 
            --size-id="66" // DO = 66, RAX = 2 
            --region-id="2" // DO = 2, RAX = LON 
            --box-amount=1 // An Integer number of boxes to create 
            --force-name="a-box-name" // optional, will override other options for name creation. may cause a conflict if creating more than 1 box. 
            --parallax // optional, when adding more than one box, if the provider supports it we can execute all requests in parallel 

Der Benutzer muss die folgenden Felder angeben, wie im obigen Befehl dargestellt,

* Umgebungsnamen
* Server-Präfix
* Anbieter
* Bild-ID
* Box Menge (Sollte eine ganze Zahl sein, die Anzahl der Kästchen bezeichnen hinzugefügt werden)
* Waffenname (Feld Name)
* Parallaxe (Es ist optional, sie kann bei Zugabe von mehr als einem Feld verwendet werden.)


Entfernen Box
------------------

Diese Funktion zielt darauf ab, einen Rahmen aus der Papyrus. Dies kann durch Verwendung unter den Befehl durchgeführt werden,

.. code-block:: bash

	cleopatra dnsify box-remove --environment-name="staging" --environment-version="5.0" --provider="apt-get"

Der Benutzer muss die folgenden Felder angeben, wie im obigen Befehl dargestellt,

* Umgebungsnamen
* Umwelt-Version
* Anbieter

Die Zerstörung einer Box
--------------------------

Diese Funktion zielt darauf ab, einen Rahmen aus der Papyrus. Diese Funktion kann einfach mit dem folgenden Befehl durchgeführt werden,

.. code-block:: bash

	cleopatra dnsify box-destroy --environment-name="staging" 
            --destroy-all-boxes 
            --destroy

Der oben genannte Befehl ist für die Vernichtung aller Boxen einer bestimmten Umgebung verwendet.

Liste
-------


 Das Hauptziel dieser Funktion ist es, listet alle Server eines bestimmten Papyrus oder in einer Umgebung. Die Syntax für das Auflisten aller Server ist wie unten dargestellt,

.. code-block:: bash

	cleopatra dnsify list-papyrus --yes --environment-name="staging"

Der oben genannte Befehl listet Papyrus einer angegebenen Umgebung.



Alternative Parameter
-----------------------------

Die alternative Parameter für dieses Modul, die beide in Erklärung verwendet werden,

* DNSify
* dnsify


Vorteile
-----------

* Die in Hilfe und andere Operationen der Box Syntax wird nicht zwischen Groß- und Kleinschreibung.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Alle wichtigen Funktionen für die Verwaltung eines Kästchen DNS-Management wird im Rahmen dieses einzigen Modul gewickelt.



