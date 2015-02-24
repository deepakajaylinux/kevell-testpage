================
DigitalOcean
================

Zusammenfassung
-------------------------

Dieses Modul unterstützt die Anwender im Umgang mit Servern auf digitalen Ozean. Es umhüllt alle grundlegenden Bedürfnisse der Nutzer im Umgang mit Boxen auf digitalen Ozean.
Die anstehenden Themen erörtert, wie Sie dieses Modul im Rahmen dieses Modul verwenden, die verschiedenen Funktionen des digitalen Ozean.

Hilfe Befehl
-------------------

Der Befehl help dient als kurze Bedienungsanleitung. Es beschreibt, über das Hauptziel dieses Moduls. Es listet outs die alternativen Parameter, die in Erklärungen verwendet werden kann. Darüber hinaus ist es hebt auch die verschiedenen Funktionen mit digitalen Ozean unter diesem Modul zusammen mit der Syntax für sie. Der Befehl für die Hilfe-Option erklärt verwendet wird unten gezeigt,

.. code-block:: bash

		ptconfigure DigitalOcean help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Digitale Ozean.

.. code-block:: bash

 kevell@corp:/# ptconfigure DigitalOcean help
 ******************************


    This is an extension provided for Handling Servers on Digital Ocean.

    DigitalOcean, digitaloceanv1, digital-ocean-v1

        - box-add
        Lets you add boxes to Digital Ocean, and adds them to your papyrusfile
        example: ptconfigure digital-ocean box-add
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"

        - box-destroy
        Will destroy box/es in an environment for you, and remove them from the papyrus file
        example: ptconfigure digital-ocean box-destroy --yes --guess --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub" --digital-ocean-ssh-key-name="bastion"

        - box-destroy-all
        Will destroy all boxes in your digital ocean account - Careful - its irreversible
        example: ptconfigure digital-ocean box-destroy-all --yes --guess

        - save-ssh-key
        Will let you save a local ssh key to your Digital Ocean account, so you can ssh in to your nodes
        securely and without a password
        example: ptconfigure digital-ocean save-ssh-key
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"

        - list
        Will display data about your digital ocean account
        example: ptconfigure digital-ocean list
        example: ptconfigure digital-ocean list --yes
                    --guess # use project saved connection details if possible
                    --type=sizes # droplets, sizes, images, domains, regions, ssh_keys

 ------------------------------
 End Help
 ******************************

Funktionen von Digital Ozean
--------------------------------

Wie im obigen Befehl help dargestellt, hat dieses Modul verschiedenen Funktionen bei der Verwendung digitaler Ozean, wie unten aufgeführt

* Box_Add
* Box_Destroy
* Box_Destroy_All
* Save_ssh_Key
* Liste


Box_Add
------------

Diese Funktion soll die Zugabe Kästen an den digitalen Ozean und in der Hand fügen Sie sie der Papyrus-Datei. Dies kann einfach unter Verwendung der Syntax wie unten angegeben durchgeführt werden,
.. code-block:: bash

	ptconfigure digital-ocean box-add
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"
Um den Befehl über implementieren, Benutzer müssen die folgenden Felder im Format der oben genannten Syntax angeben.

* Digital Ozean ssh-Schlüsselpfad
* Digital Ozean ssh_key Namen



Box_Destroy
----------------

Diese Funktion zielt auf die Zerstörung Boxen in einer vorgegebenen Umgebung und in der Hand entfernen Sie sie aus dem Papyrus-Datei. Dies kann einfach unter Verwendung der Syntax wie unten angegeben durchgeführt werden,

.. code-block:: bash

	ptconfigure digital-ocean box-destroy --yes --guess --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub" 
        --digital-ocean-ssh-key-name="bastion"

Um den Befehl über implementieren, Benutzer müssen die folgenden Felder im Format der oben genannten Syntax angeben.

* Digital Ozean ssh-Schlüsselpfad
* Digital Ozean ssh_key Namen

Box_Destroy_All
----------------------

Diese Funktion soll die Vernichtung sämtlicher Boxen im digitalen Ozean Konto. Der Benutzer sollten vorsichtig sein bei der Umsetzung dieses verfügt, weil es ein unumkehrbarer Prozess. Um diese Funktion zu implementieren der Benutzer, um den Befehl anzuwenden, die nachstehend angegeben,

.. code-block:: bash
   
	ptconfigure digital-ocean box-destroy-all --yes --guess

Save_Ssh_key
-------------------

Diese Funktion ermöglicht es den Benutzern, eine lokale ssh, um Ihre digitalen Ozean zu speichern, damit die Benutzer in ihre Knoten sicher ohne Passwort ssh. Dies kann durch Verwendung unter den Befehl erreicht werden,

.. code-block:: bash

	ptconfigure digital-ocean save-ssh-key
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"
Um den Befehl über implementieren, Benutzer müssen die folgenden Felder im Format der oben genannten Syntax angeben.

* Digital Ozean ssh-Schlüsselpfad
* Digital Ozean ssh_key Namen

Liste
-----

Diese Funktion ermöglicht es den Benutzern, listet alle Daten über ihre digitalen Ozean Konto. Dies kann einfach durch das unten stehende Befehl umgesetzt werden,
       
.. code-block:: bash

	ptconfigure digital-ocean list

Or

.. code-block:: bash

        ptconfigure digital-ocean list --yes
                    --guess # use project saved connection details if possible
                    --type=sizes # droplets, sizes, images, domains, regions, ssh_keys


Alternative Parameter
----------------------------

Die alternative Parameter für dieses Modul, die beide in Erklärung verwendet werden,

DigitalOcean,   digitaloceanv1,   digital-ocean-v1

Vorteile
-----------

* Die verwendeten Hilfe und andere unterschiedliche Merkmale von apt erklärt Parameter wird nicht zwischen Groß- und Kleinschreibung.
* Es ist gut-to-do in beiden Cent os und als auch in Ubuntu.
* Dieses Modul umschließt alle Bedürfnisse der Anwender im Umgang mit digitalen Ozean.

