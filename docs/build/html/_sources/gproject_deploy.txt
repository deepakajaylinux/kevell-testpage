==============
Project
==============

Zusammenfassung
-----------------------

In der heutigen Wirtschaft und Wissenschaft ein Projekt als Gemeinschaftsunternehmen festgelegt, an denen Forschung oder Design, die sorgfältig geplant wird, um ein bestimmtes Ziel zu erreichen. Projekte können weiter als temporäre und nicht dauerhafte soziale Systeme oder Systeme, die Arbeit von Teams innerhalb oder zwischen Organisationen aufgebaut sind, um bestimmte Aufgaben unter Zeitdruck zu tun definiert werden. Ein laufendes Projekt ist in der Regel genannt (oder entwickelt sich zu) eines Programms.

Dieser Befehl ist Teil der Standard-Module und übernimmt Projektfunktionen Initialisierung, wie die Konfiguration eines Projekts oder einer Projektbehälter und auch die Installation Jenkins-Build-Dateien in eine laufende Jenkins Beispiel.

Hilfe Befehl
----------------------

Dieser Befehl hilft, die Nutzung von Projektmodul zu bestimmen. Der Benutzer wird kommen, um über die verschiedenen Möglichkeiten / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen. Da unten sind die Befehls- und die Screenshot der gleiche.

.. code-block:: bash
	
	ptdeploy project help
       

 kevell@corp:/# ptdeploy Project help
 ******************************


  This command is part of Default Modules and handles Project initialisation functions, like configuring a project, or a project
  container and also installing Jenkins build files into a running Jenkins instance.

  Project, project, proj


          - container
          make a container folder for revisions (like /var/www/applications/*APP NAME*)
          example: ptdeploy proj container
          example: ptdeploy proj container --yes --proj-container="/var/www/applications/the-app"

          - init
          initialize Dapper project
          example: ptdeploy proj init
          example: ptdeploy proj init --yes

          - build-install
          copy jenkins project stored in repo to running jenkins so you can run builds
          example: ptdeploy proj build-install
          example: ptdeploy proj build-install
                        --jenkins-fs-dir=/var/lib/jenkins # --guess will set this to /var/lib/jenkins
                        --original-build-dir="/var/www/applications/the-app/build/config/ptconfigure/Project/jenkins-builds"
                        --target-job-name="Project_Build"
                        --new-job-dir="Project_Build_Alternate_Name"  # If target one is not available

 ------------------------------
 End Help
 ******************************

Behälter
----------------

Dieser Befehl hilft, einen Container Ordner für Änderungen (wie / var / www / Anwendungen / * Name der App*)


Wenn der Benutzer zu installieren muss, kann der Benutzer die folgenden Befehle für DBIstall ausgeben. Das System wird den Prozess der Installation durchzuführen.

.. code-block:: bash
	
	 ptdeploy proj container

 kevell@corp:/# ptdeploy proj container
 Do you want to Modify Project Container Settings? (Y/N) 
 Y
 Do you want to initialize this as a ptdeploy project Container? (Y/N) 
 Y
 What is your Project Container directory?
 /root/gg
 Project Container directory created
 /root/gg space /root/ggMoving to Container
 /root/gg
 Showing Container Directory
 Project Container file created
 ******************************


 Seems Fine...Project Editor Finished
 ******************************



init
----------------

Wenn der Benutzer dapper Projekt initialisieren muss, kann der Benutzer die folgenden Befehle. Das System wird den Prozess auszuführen.

.. code-block:: bash
	
	 ptdeploy proj init


.. code-block:: bash

 kevell@corp:/# ptdeploy proj init
 Do you want to Modify Project Settings To initialise Project? (Y/N) 
 Y
 Do you want to initialize this as a ptdeploy project? (Y/N) 
 Y
 ******************************


 Seems Fine...Project Editor Finished
 ******************************



Errichten-Installation
--------------------------

Wenn die Bedürfnisse der Nutzer zu kopieren Jenkins Projekts in Repo gespeichert zu laufen Jenkins, kann der Benutzer die folgenden Befehle. Das System wird den Prozess auszuführen.

.. code-block:: bash
	
	 ptdeploy proj build-install

Type text or a website address or translate a document.

Alternative Parameter
--------------------------------

Es gibt zwei alternative Parameter, die im Befehl verwendet werden kann.

Project, project and proj

eg: ptdeploy Project help/  ptdeploy proj help
                       

Vorteile
--------------

* Hilft einen Container Ordner für Revisionen
* Hilft, dapper Projekt initialisieren

