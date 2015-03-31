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

	ptconfigure cleofy help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter cleofy.

.. code-block:: bash


 kevell@corp:/# ptconfigure cleofy help

 ******************************


 This command is part of a default Module Core and provides you with a method by which you can create a standard set of Autopilot files for your project from the command line.  


 Cleofy, cleofy  

 - list        
 	List all of the autopilot files in your build/config/ptconfigure/autopilots        
	example: ptconfigure cleofy list        

 - standard        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for your project.        
	example: ptconfigure cleofy standard        

 - tiny        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for a project with a "tiny" style infrastructure.        	example: ptconfigure cleofy tiny        

 - medium        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for a project with a "medium" style infrastructure.        	example: ptconfigure cleofy medium        

 - medium-web        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for a project with a "medium" style infrastructure,
        with web but not database.        
 	example: ptconfigure cleofy medium-web        

 - db-cluster        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for your project.        
 	example: ptconfigure cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*                    

 - install-generic-autopilots        
	Install the generic Cleofy autopilot templates for a Tiny or Medium (Current Default) set of Environments        
 example: ptconfigure cleofy install-generic-autopilots        
	example: ptconfigure cleofy install-generic-autopilots        
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/cleofy/autopilots/                    
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

Diese Funktion soll in dem alle Autopilot-Dateien im angegebenen Verzeichnis (build / config / ptconfigure / Autopiloten). Die Syntax für die Anwendung dieser Funktion ist unten dargestellt,

.. code-block:: bash

	ptconfigure cleofy list



Standard
------------

Diese Funktion hilft bei der Erstellung eines Standardsatz von ptconfigure Autopiloten (in build / config / ptconfigure / Autopiloten) für das Projekt der Nutzer. Diese Funktion kann einfach durch die Verwendung unter den Befehl anzuwenden,

.. code-block:: bash

	ptconfigure cleofy standard


.. code-block:: bash

 kevell@corp:/# ptconfigure cleofy standard

 Cleofy This? (Y/N) 
 y
 Environment 1  : 
 Default Settings for Any App not setup for environment  enter them now.
 Value for: Name of this Environment
 test1
 Value for: Default Temp Dir (should usually be /tmp/)

 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-bastion.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-build-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-cleo-dapper.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-db-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-db-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-git.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-standalone-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-web-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-web-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-bastion.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-build-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-cleo-dapper-new.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-cleo-dapper-update.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-db-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-db-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-git.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-standalone-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-web-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-web-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-prep-any-box.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-prep-ubuntu.php
 ******************************


 Success
 In Cleofy
 ******************************




Sehr Klein
--------------

Diese Funktion zielt auf die Schaffung einen Standardsatz von ptconfigure Autopiloten (in build / config / ptconfigure / Autopiloten) für ein Projekt mit winzigen Infrastruktur. Zur Durchführung dieser Funktionen verwenden Sie folgenden Befehl, wie unten,

.. code-block:: bash

	ptconfigure cleofy tiny


.. code-block:: bash


 kevell@corp:/# ptconfigure cleofy tiny 

 Cleofy This? (Y/N) 
 y 
 Use existing environment settings? (Y/N) 
 y 
 Do you want to modify entries applicable to any app in environment kevells (Y/N) 
 n 
 Settings for cleo not setup for environment kevells enter them manually. 
 Environment 1 kevells : 
 Do you want to add another environment? (Y/N) 
 n 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-cleo-dapper.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-new.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-update.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-any-box.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-ubuntu.php 
 ****************************** 


 Success 
 In Cleofy 
 ****************************** 

Medium
-----------

Diese Funktion zielt auf die Schaffung einen Standardsatz von ptconfigure Autopiloten (in build / config / ptconfigure / Autopiloten) für ein Projekt mit mittel Infrastruktur. Zur Durchführung dieser Funktionen verwenden Sie folgenden Befehl, wie unten,

.. code-block:: bash

	ptconfigure cleofy medium

.. code-block:: bash

 kevell@corp:/# ptconfigure cleofy medium 

 Cleofy This? (Y/N) 
 y 
 Use existing environment settings? (Y/N) 
 y 
 Do you want to modify entries applicable to any app in environment kevells (Y/N) 
 n 
 Settings for cleo not setup for environment kevells enter them manually. 
 Environment 1 kevells : 
 Do you want to add another environment? (Y/N) 
 n 
 Enter name of environment with your Stage web nodes 
 kevells 
 Enter name of environment with your Stage database nodes 
 kevells 
 Enter name of environment with your Prod web nodes 
 kevells 
 Enter name of environment with your Prod database nodes 
 kevells 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-cleo-dapper.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-new.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-update.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-any-box.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-ubuntu.php 
 ******************************    


 Success 
 In Cleofy 
 ****************************** 


Medium_Web
-------------------

Diese Funktion zielt auf die Schaffung einen Standardsatz von ptconfigure Autopiloten (in build / config / ptconfigure / Autopiloten) für ein Projekt mit mittel Infrastruktur mit Web, aber nicht Datenbank. Zur Durchführung dieser Funktionen verwenden Sie folgenden Befehl, wie unten,

.. code-block:: bash

	ptconfigure cleofy medium-web

.. code-block:: bash


 kevell@corp:/# ptconfigure cleofy medium-web 

 Cleofy This? (Y/N) 
 y 
 Use existing environment settings? (Y/N) 
 y 
 Do you want to modify entries applicable to any app in environment kevells (Y/N) 
 n 
 Settings for cleo not setup for environment kevells enter them manually. 
 Environment 1 kevells : 
 Do you want to add another environment? (Y/N) 
 n 
 Enter name of environment with your Stage web nodes 
 kevells 
 Enter name of environment with your Prod web nodes 
 kevells 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-cleo-dapper.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-new.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-update.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-any-box.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-ubuntu.php 
 ****************************** 


 Success 
 In Cleofy 
 ****************************** 


DB_cluster
---------------

Diese Funktion zielt auf die Schaffung einen Standardsatz von ptconfigure Autopiloten (in build / config / ptconfigure / Autopiloten) für die Benutzer-Projekt.

Zur Durchführung dieser Funktionen verwenden Sie folgenden Befehl, wie unten,

.. code-block:: bash

	ptconfigure cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*                    

.. code-block:: bash


 kevell@corp:/# ptconfigure cleofy db-cluster 

 Cleofy This? (Y/N) 
 y 
 Use existing environment settings? (Y/N) 
 y 
 Do you want to modify entries applicable to any app in environment kevells (Y/N) 
 n 
 Settings for cleo not setup for environment kevells enter them manually. 
 Environment 1 kevells : 
 Do you want to add another environment? (Y/N) 
 n 
 Enter name of environment with your Databasenodes 
 kevells 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-cleo-dapper.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-new.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-update.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-any-box.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-ubuntu.php 
 ****************************** 


 Success 
 In Cleofy 
 ****************************** 


Install_generic_autopilots
--------------------------------

Diese Funktion hilft bei der Installation von generischen Autopilot-Vorlagen für kleine oder mittlere Reihe von Umwelt, indem Sie einfach mit dem Befehl als gegeben
unten,


	
.. code-block:: bash
	
	ptconfigure cleofy install-generic-autopilots        
Or,

.. code-block:: bash

	ptconfigure cleofy install-generic-autopilots
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/cleofy/autopilots/                    
 --template-group=tiny # tiny, medium, dbcluster, phlagrant || db-cluster, workstation                    
 --destination-dir=*path-to-destination*                    


Um den Befehl zu implementieren, wie oben angegeben, kann der Benutzer müssen die folgenden Felder angeben, wie angegeben,

* Ziel-Verzeichnis
* Vorlagengruppe

.. code-block:: bash


 kevell@corp:/# ptconfigure cleofy install-generic-autopilots 

 Enter Template Group: 
 (0) tiny 
 (1) medium 
 0 
 Enter Destination Directory: 
 /tmp/ 
 [Pharaoh Logging] Performing file copy from /opt/ptconfigure-enterprise/src/Modules/Cleofy/Templates/Generic/Tiny to /tmp/ 
 ****************************** 
  

 Cleofy Listing: 
 --------------------------------------------  

 Success 

 ------------------------------ 
 Cleofy Generic Autopilot Install Finished 
 ****************************** 


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


