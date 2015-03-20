===============
JArticle
===============

Zusammenfassung
----------------

Es verwaltet die Jarticle Details. Dadurch können Sie einen Artikel als Modul zu verwenden. Joomla bietet ein extrem breites Spektrum an Optionen für die Erstellung unterschiedlicher Arten von Inhalten und auf Ihrer Website zu strukturieren.


In Joomla ist ein Artikel ein Inhaltselement bestehend aus Text, eventuell mit Links zu anderen Ressourcen (z.B. Bilder). Artikel sind die Grundeinheiten der Informationen in das Content-System und die unterste Ebene in der Content-Hierarchie. Jeder Artikel wird in genau eine Kategorie. Eine Kategorie kann in einer anderen Kategorie, so dass es eine Sub-Kategorie sein. Es ist auch möglich, Uncategorized Artikel haben. Diese Artikel gibt es ohne jede Kategorie zugeordnet wird.


Hilfe Befehl
----------------------

Dieser Befehl hilft, um die Verwendung des Jarticle-Moduls zu bestimmen. Der Benutzer wird kommen, über die verschiedenen Möglichkeiten/Format wissen, dieses Modul ausgeführt. Dieser Befehl führt den Endbenutzer, um diesen Befehl zu erfahren. Im folgenden sind mit dem Befehl und der Screenshot von der gleichen.


.. code-block:: bash
        
	jrush  jarticle help


.. code-block:: bash

 kevell@corp:/# jrush  jarticle help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to manage Joomla JArticles (Component, Module or Plugin).

  JArticle, jarticle

        - disable
        Deletes a jarticle
        example: jrush jarticle disable

        - enable
        Enables a jarticle
        example: jrush jarticle enable

        - info
        Display the details of a jarticle
        example: jrush jarticle info


 ------------------------------
 End Help
 ****************************************



Enable
----------------

Wenn der Benutzer zu eine bestimmte Artikel zu aktivieren muss die unten mit dem Befehl wird ausgeführt, den Prozess der Installation.


.. code-block:: bash
        
	jrush jarticle enable ..config file=”bootstrap file path”


Info
------

Wenn der Benutzer über die Informationen eines Artikels wissen muss. Die unten mit dem Befehl hilft Ihnen


.. code-block:: bash
        
	jrush jarticle info ..config file=”bootstrap file path”


Die bildliche Darstellung der oben genannte Befehl ist im folgenden aufgeführt,


.. code-block:: bash

 kevell@corp:/# jrush jarticle info --config-file="/var/www/html/joomla/configuration.php"
 Enter a JArticle ID. To enter title/alias/asset-id use --jarticle-title, --jarticle-alias or --jarticle-asset-id parameters
 2
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JArticle Information:
 -------------------------

 Article ID: 2
 Asset ID: 35
 Alias: about-us
 Title: About Us
 Created By: 825
 Created By Alias: Joomla
 State: 1
 ------------------------------
 JArticle Manage Finished
 ****************************************


Disable
----------------

Wenn der Benutzer zu eine bestimmte Artikel deaktivieren muss die unten mit dem Befehl wird ausgeführt, den Prozess der Installation.


.. code-block:: bash
        
	jrush jarticle disable ..config file=”bootstrap file path”

Alternative Parameter
----------------------------


Eines der zwei alternative Parameter einsetzbar in Befehl –

jarticle, JArticle

eg:  jrush jarticle disable/ jrush JArticle disable                                 




Vorteile
--------------

* Stellen Sie eine optionale Methode zum organisieren Ihre Artikel 
* es enthält Text und kann Bilder und andere Arten von Inhalten enthalten * hilft, die Informationen über einen Artikel auf einfache Weise 
* aktivieren und deaktivieren ein Artikels in einem Schritt kann

