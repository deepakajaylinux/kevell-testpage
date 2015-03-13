============
Rackspace
============

Zusammenfassung
-----------------

Rackspace bietet leistungsstarke , zuverlässige Infrastruktur in der Cloud erfolgreich zu sein. Es dauert mit vollem Funktionsumfang, optimierte Plattformen und ein Team von Experten , um Workloads .

Rackspace hat zwei Hauptgeschäftsbereiche- Cloud-Server und dedizierte Server . Rackspace hilft planen, bauen und betreiben Workloads in beiden Umgebungen je nach den individuellen Bedürfnissen des Kunden .

Cloud Server - Die Managed Infrastructure Service-Level bietet einen Kernsatz von Dienstleistungen erforderlich , um Kunden in die Cloud setzen , einschließlich Architektur Beratung, Sicherheitsunterstützung und Codeentwicklungshilfe ( über APIs und SDKs ) . Die Managed Operations Support-Level bietet alle Managed Infrastructure Services und zusätzliche proaktive Unterstützung .

Dedizierte Server - Der Managed Service-Level besteht aus On-Demand- Support , wo proaktive Dienstleistungen erbracht werden. 


Hilfe Befehl
----------------------

Diese Funktion dient , um die Verwendung von Rackspace bestimmen. Der Benutzer wird kommen, um über die andere Art und Weise / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender , um den Zweck dieses Befehls kennen. Da unten sind die Kommando- und der Screenshot der gleiche. 

.. code-block:: bash


 kevell@corp:/# ptconfigure Rackspace help

 ******************************


    This is an extension provided for Handling Servers on Rackspace.

    Rackspace, rackspace

        - box-add
        Lets you add boxes to Rackspace, and adds them to your papyrusfile
        example: ptconfigure rackspace box-add
                    --yes
                    --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --rackspace-ssh-key-name="bastion"

        - box-destroy
        Will destroy box/es in an environment for you, and remove them from the papyrus file
        example: ptconfigure rackspace box-destroy --yes --guess --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

        - box-destroy-all
        Will destroy all boxes in your Rackspace account - Careful - its irreversible
        example: ptconfigure rackspace box-destroy-all --yes --guess

        - save-ssh-key, sshkey, ssh-key
        Will let you save a local ssh key to your Rackspace account, so you can ssh in to your nodes with it
        securely and without a password
        example: ptconfigure rackspace save-ssh-key
                    --yes
                    --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --rackspace-ssh-key-name="bastion"

        - list
        Will display data about your Rackspace account
        example: ptconfigure rackspace list
        example: ptconfigure rackspace list --yes
                    --guess # use project saved connection details if possible
                    --rackspace-list-data-type=sizes # servers, sizes, images, domains, regions, ssh_keys

        - list-containers
        Will display Container data about your Rackspace account
        example: ptconfigure rackspace list-containers
        example: ptconfigure rackspace list-containers --yes
                    --guess # use project saved connection details if possible

        - list-objects
        Will display object of Containers data about your Rackspace account
        example: ptconfigure rackspace list-objects
        example: ptconfigure rackspace list-objects --yes
                    --guess # use project saved connection details if possible

 ------------------------------
 End Help
 ******************************


Box - Add
----------------

Dieser Befehl hilft, Boxen Rackspace hinzufügen und fügt sie den Papyrus -Datei. Die unten angegebenen Befehl wird den Prozess auszuführen.

.. code-block:: bash

 ptconfigure rackspace box-add --yes --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

Box - zerstören
-------------------

Dieser Befehl hilft, Box / es in einer Umgebung für Sie zu zerstören , und sie aus dem Papyrus -Datei. Die unten angegebenen Befehl wird den Prozess auszuführen.

.. code-block:: bash

 ptconfigure rackspace box-destroy --yes --guess --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

Box - zerstören -all
-----------------------

Dieser Befehl hilft, alle Kisten in Ihrem Konto Rackspace zu zerstören. Der wichtigste Teil ist es irreversibel ist .

.. code-block:: bash     

 ptconfigure rackspace box-destroy-all --yes --guess

Save- ssh- Schlüssel
---------------------

Dieser Befehl hilft, eine lokale SSH-Schlüssel zu Ihrem Rackspace Konto zu speichern , so dass Sie zu Ihrem Knoten mit sich sicher und ohne Passwort in ssh . Es gibt drei alternative Parameter für diesen Befehl verwendet - ssh -key, sshkey , ssh- Schlüssel . Die unten angegebenen Befehl wird den Prozess auszuführen.

.. code-block:: bash     
	
	ptconfigure rackspace save-ssh-key --yes --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"


Liste 
---------------------

Dieser Befehl hilft dabei, Daten über Ihre Rackspace Konto. Die unten angegebenen Befehl wird den Prozess auszuführen.

.. code-block:: bash 
	
	ptconfigure rackspace list
        
.. code-block:: bash 

	ptconfigure rackspace list --yes --guess # use project saved connection details if possible --rackspace-list-data-type=sizes # servers, sizes, images, domains, regions, ssh_keys

List- Container
---------------------

Dieser Befehl hilft, Container Daten über Ihre Rackspace Konto anzuzeigen. Die unten angegebenen Befehl wird den Prozess auszuführen.

.. code-block:: bash 
	
 	ptconfigure rackspace list-containers

.. code-block:: bash 

	ptconfigure rackspace list-containers --yes --guess # use project saved connection details if possible


List- Objekte
---------------------

Dieser Befehl hilft, Gegenstand Containers Daten über Ihre Rackspace Konto anzuzeigen. Die unten angegebenen Befehl wird den Prozess auszuführen.

.. code-block:: bash 

 	ptconfigure rackspace list-objects

.. code-block:: bash 

	ptconfigure rackspace list-objects --yes --guess # use project saved connection details if possible

Alternative Parameter
------------------------------       

Es gibt zwei alternative Parameter, die in der Befehlszeile verwendet werden kann.

Rackspace, rackspace


Vorteile
--------------

Rackspace bietet eine Komplettlösung für die Kunden fordern eine leistungsstarke, speziell gebaute Infrastruktur für relationale Datenbanken gesichert und von Ingenieuren unterstützt , die in MySQL Workloads spezialisiert konzipiert. Rackspace ist ein vollständig verwalteter Dienst für Kunden, die auf die Entwicklung ihrer Anwendungen konzentrieren und nicht über die zugrunde liegende Infrastruktur kümmern möchten. Der Service bietet bei Bedarf Sicherungen und Wiederherstellungen , die integrierte Überwachung , redundante Speicherung , Skalierbarkeit , um den Anforderungen Ihrer Anwendung und die vollständige Kontrolle über die Datenbank auf der Basis wachsen .
