=======
Cleofy
=======

Zusammenfassung
-------------------------

Dieses Modul zielt darauf ab, die Benutzer bei der Schaffung eines Standard-Set von Autopilot-Dateien für das Projekt. Wir wollen sehen, wie dieses Modul über Funktionen cleofy von den kommenden Themen zu verwenden, und auch.

Hilfe Befehl
--------------------

Der Befehl help ist eine kurze Bedienungsanleitung, die die Benutzer sich bewusst sein, erhalten über die Nutzung erleichtert, Methoden der Umgang mit diesem Modul, um verschiedene Funktionen auszuführen. Außerdem werden outs die alternativen Parameter, die in Erklärungen verwendet werden kann. Sie weist auf die Syntax Beispiel für die Verwendung und den Zugriff auf verschiedene Funktionen unter cleofy.

Der Befehl für die Hilfe-Option unter cleofy erklärt verwendet wird unten gezeigt,

.. code-block:: bash

	cleopatra cleofy help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter cleofy.

.. code-block:: bash


 kevell@corp:/# cleopatra cleofy help

 ******************************


 This command is part of a default Module Core and provides you with a method by which you can create a standard set of Autopilot files for your project from the command line.  


 Cleofy, cleofy  

 - list        
 	List all of the autopilot files in your build/config/cleopatra/autopilots        
	example: cleopatra cleofy list        

 - standard        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for your project.        
	example: cleopatra cleofy standard        

 - tiny        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for a project with a "tiny" style infrastructure.        	example: cleopatra cleofy tiny        

 - medium        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for a project with a "medium" style infrastructure.        	example: cleopatra cleofy medium        

 - medium-web        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for a project with a "medium" style infrastructure,
        with web but not database.        
 	example: cleopatra cleofy medium-web        

 - db-cluster        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for your project.        
 	example: cleopatra cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*                    

 - install-generic-autopilots        
	Install the generic Cleofy autopilot templates for a Tiny or Medium (Current Default) set of Environments        
 example: cleopatra cleofy install-generic-autopilots        
	example: cleopatra cleofy install-generic-autopilots        
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/cleopatra/cleofy/autopilots/                    
 --template-group=tiny # tiny, medium, dbcluster, phlagrant || db-cluster, workstation                    
 --destination-dir=*path-to-destination*                    

 ------------------------------
 End Help
 ******************************


Funktionen cleofy
------------------------


Dieses Thema stellt über die verschiedenen Funktionen der cleofy unter diesem Modul, wie unten aufgeführt,

* Liste
* Standard
* Sehr Klein
* Medium
* Medium-web
* DB-Cluster
* Install_generic_autopilots


Liste
-------

Diese Funktion soll in dem alle Autopilot-Dateien im angegebenen Verzeichnis (build / config / cleopatra / Autopiloten). Die Syntax für die Anwendung dieser Funktion ist unten dargestellt,

.. code-block:: bash

	cleopatra cleofy list



Standard
------------

Diese Funktion hilft bei der Erstellung eines Standardsatz von cleopatra Autopiloten (in build / config / cleopatra / Autopiloten) für das Projekt der Nutzer. Diese Funktion kann einfach durch die Verwendung unter den Befehl anzuwenden,

.. code-block:: bash

	cleopatra cleofy standard


Sehr Klein
--------------

Diese Funktion zielt auf die Schaffung einen Standardsatz von cleopatra Autopiloten (in build / config / cleopatra / Autopiloten) für ein Projekt mit winzigen Infrastruktur. Zur Durchführung dieser Funktionen verwenden Sie folgenden Befehl, wie unten,

.. code-block:: bash

	cleopatra cleofy tiny

Medium
-----------

Diese Funktion zielt auf die Schaffung einen Standardsatz von cleopatra Autopiloten (in build / config / cleopatra / Autopiloten) für ein Projekt mit mittel Infrastruktur. Zur Durchführung dieser Funktionen verwenden Sie folgenden Befehl, wie unten,

.. code-block:: bash

	cleopatra cleofy medium

Medium_Web
-------------------

Diese Funktion zielt auf die Schaffung einen Standardsatz von cleopatra Autopiloten (in build / config / cleopatra / Autopiloten) für ein Projekt mit mittel Infrastruktur mit Web, aber nicht Datenbank. Zur Durchführung dieser Funktionen verwenden Sie folgenden Befehl, wie unten,

.. code-block:: bash

	cleopatra cleofy medium-web

DB_cluster
---------------

Diese Funktion zielt auf die Schaffung einen Standardsatz von cleopatra Autopiloten (in build / config / cleopatra / Autopiloten) für die Benutzer-Projekt.

Zur Durchführung dieser Funktionen verwenden Sie folgenden Befehl, wie unten,

.. code-block:: bash

	cleopatra cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*                    

Install_generic_autopilots
--------------------------------

Diese Funktion hilft bei der Installation von generischen Autopilot-Vorlagen für kleine oder mittlere Reihe von Umwelt, indem Sie einfach mit dem Befehl als gegeben
unten,


	
.. code-block:: bash
	
	cleopatra cleofy install-generic-autopilots        
Or,

.. code-block:: bash

	cleopatra cleofy install-generic-autopilots
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/cleopatra/cleofy/autopilots/                    
 --template-group=tiny # tiny, medium, dbcluster, phlagrant || db-cluster, workstation                    
 --destination-dir=*path-to-destination*                    


Um den Befehl zu implementieren, wie oben angegeben, kann der Benutzer müssen die folgenden Felder angeben, wie angegeben,

* Ziel-Verzeichnis
* Vorlagengruppe


Alternative Parameter
-----------------------------

Die alternative Parameter für dieses Modul, die beide in Erklärung verwendet werden,

* Cleofy,
* cleofy

Vorteile
------------

* Die verwendeten Hilfe und andere unterschiedliche Merkmale von apt erklärt Parameter wird nicht zwischen Groß- und Kleinschreibung.
* Es ist gut-to-do in beiden Cent os und als auch in Ubuntu.
* Dieses Modul umschließt alle Bedürfnisse eines Projektes bei der Schaffung von Standard-Set von Autopiloten.


