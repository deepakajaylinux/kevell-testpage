=======
Boxify
=======


Zusammenfassung
-------------------------

Diese Module Umschläge alle wichtigen Bedürfnisse der Anwender bei der Erstellung und Verwaltung sowie die Box. Dieses Thema ist es, wie Sie dieses Modul verwenden zu diskutieren und über verschiedene Funktionen bei der Verwendung boxify.

Hilfe Befehl
-------------------

Der Befehl help führt den Anwender beim Umgang mit diesem Modul, um zu handhaben und führen verschiedene Funktionen aus einer Box. Es listet outs die alternativen Parameter, und hebt die Syntax für die verschiedenen Funktionen der Verwendung und Modifizierung einer Box. Die Syntax für die Hilfe-Option unter dem boxify Moduls ist unten dargestellt,

.. code-block:: bash

	ptconfigure Boxify help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter boxify.

.. code-block:: bash


 kevell@corp:/# ptconfigure Boxify help 
 ****************************** 


  This command provides a generic Box Management wrapper around all of the Box Providers (Cloud and Otherwise) so that we have a 
  generic way to create and destroy boxes. 

  Boxify, boxify 

        - install-generic-autopilots 
        Install the generic Boxify autopilot templates for a Tiny or Medium (Current Default) set of Environments 
        example: ptconfigure boxify install-generic-autopilots 
        example: ptconfigure boxify install-generic-autopilots 
                    --yes 
                    --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/boxify/autopilots/ 
                    --template-group=tiny 
                    --destination-dir=*path-to-destination* 

        - box-add 
        Installs a Box through a cloud provider 
        example: ptconfigure boxify box-add --environment-name="*environment*" 
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
        example: ptconfigure boxify box-remove --environment-name="staging" --environment-version="5.0" --provider="apt-get" 

        - box-destroy 
        Removes a Box from both papyrus and the cloud provider 
        example: ptconfigure boxify box-destroy --environment-name="staging" 
            --destroy-all-boxes 
            --destroy 

        - list-papyrus 
        List all servers in papyrus, or those of a particular environment 
        example: ptconfigure boxify list-papyrus --yes 
        example: ptconfigure boxify list-papyrus --yes --environment-name="staging" 


 ------------------------------ 
 End Help 
 ****************************** 

Verschiedene Funktionen der boxify
-----------------------------------------

Diese Themen beschrieben über die verschiedenen Funktionen boxify unter diesem Modul, wie nachstehend aufgeführt

* Installieren Sie generische Autopiloten
* Hinzufügen Box
* Entfernen Box
* Löschen einer Box
* Liste


Installieren Sie generische Autopiloten
-------------------------------------------------

Diese Funktion soll die Installation geltenden Autopiloten zu einem kleinen oder mittleren Reihe von Umgebungen. Dies kann durch den Befehl, wie unten angegeben durchgeführt werden,

.. code-block:: bash
	
	ptconfigure boxify install-generic-autopilots 
                    --yes 
                    --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/boxify/autopilots/ 
                    --template-group=tiny 
                    --destination-dir=*path-to-destination* 
Wie in der oben genannten Syntax dargestellt der Benutzer müssen Sie die folgenden Felder, um die generische Autopiloten installiert werden 
soll.

* Zielverzeichnis
* Template-Gruppe


Hinzufügen Box
-----------------


Diese Funktion soll das Hinzufügen einer Box über einen Cloud-Anbieter, einfach, indem Sie den folgenden Befehl,

.. code-block:: bash

	example: ptconfigure boxify box-add --environment-name="*environment*" 
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

	ptconfigure boxify box-remove --environment-name="staging" --environment-version="5.0" --provider="apt-get" 

Der Benutzer muss die folgenden Felder angeben, wie im obigen Befehl dargestellt,

* Umgebungsnamen
* Umwelt-Version
* Anbieter

Die Zerstörung einer Box
----------------------------

Diese Funktion zielt darauf ab, einen Rahmen aus der Papyrus. Diese Funktion kann einfach mit dem folgenden Befehl durchgeführt werden,

.. code-block:: bash

	ptconfigure boxify box-destroy --environment-name="staging" 
            --destroy-all-boxes 
            --destroy

Der oben genannte Befehl ist für die Vernichtung aller Boxen einer bestimmten Umgebung verwendet.

Liste
--------

Das Hauptziel dieser Funktion ist es, listet alle Server eines bestimmten Papyrus oder in einer Umgebung. Die Syntax für das Auflisten aller Server ist wie unten dargestellt,

.. code-block:: bash

	ptconfigure boxify list-papyrus --yes --environment-name="staging"

Der oben genannte Befehl listet Papyrus einer angegebenen Umgebung.

Alternative Parameter
-----------------------------

Die alternative Parameter für dieses Modul, die beide in Erklärung verwendet werden,

* Boxify
* boxify


Vorteile
-----------

* Die in Hilfe und andere Operationen der Box Syntax wird nicht zwischen Groß- und Kleinschreibung.
* Es ist gut-to-do in beiden Cent OS und als auch in Ubuntu.
* Alle wichtigen Funktionen der Verwaltung einer Box wird im Rahmen dieses einzigen Modul gewickelt.


