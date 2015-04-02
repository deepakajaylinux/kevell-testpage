===============
GitCommand
===============

Zusammenfassung
------------------

Git ist eine freie und Open-Source- verteiltes Versionskontrollsystem entwickelt, um alles, von kleinen bis zu sehr großen Projekte schnell und effizient zu behandeln.


Hilfe Befehl
---------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten , die in der git -Modul enthalten sind. Es listet einige der alternativen Parameter git -Modul. Der Befehl help für git -Modul wird wie unten dargestellt.

.. code-block:: bash

	ptconfigure gitcommand help

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure gitcommand help

 ******************************



  This command handles Git Functionality

  Git, GitCommand, git-command, gitcommand

  - checkout-branch
    checkout a branch
    example: ptconfigure git checkout-branch --branch=*branchname*

  - create-checkout-branch
    checkout a branch, creating a new branch if needed
    example: ptconfigure git create-checkout-branch --branch=*branchname*

  - delete-branch
    delete a branch
    example: ptconfigure git delete-branch --branch=*branchname*
    
  - ensure-branch
    ensure a branch
    example: ptconfigure git ensure-branch --branch=*branchname*
    
  - add
    add new files to a git repository
    example: ptconfigure git add 
	
  - commit
    commit new messages to a git repository
    example: ptconfigure git  commit --message=*some commit message*

  - push
    push to a git repo
    example: ptconfigure git push --branch=*origin yourbranch*
  
  - pull
    pull a git repo
    example: ptconfigure git pull --branch=*origin yourbranch*

 ------------------------------
 End Help
 ******************************


Checkout-branch
-------------------

Der Befehl git checkout können Sie zwischen den Zweigen erstellt von git branch navigieren. Dieser Befehl Kasse eine Niederlassung und der Ausführungsprozess wird , wie unten dargestellt ,

.. code-block:: bash

	ptconfigure git checkout-branch --branch=*branchname*

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git checkout-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevellbranch
 [Pharaoh Logging] [GitCommand] Attempting to create branch kevellbranch
 Switched to branch 'kevellbranch'
 Now in: /opt/ptconfigure-enterprise 

 ******************************


 0 : In GitCommand View
 ******************************



Create-checkout-branch
---------------------------

Die git erstellen Kasse Zweig können Sie eine Niederlassung Kasse , die Schaffung einer neuen Niederlassung , wenn nötig. Der Ausführungsprozess dieses Befehls , wie gezeigt wird
unten ,


.. code-block:: bash

	ptconfigure git create-checkout-branch --branch=*branchname*

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git checkout-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevellbranch
 [Pharaoh Logging] [GitCommand] Attempting to create branch kevellbranch
 Switched to branch 'kevellbranch'
 Now in: /opt/ptconfigure-enterprise 

 ******************************


 0 : In GitCommand View
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure git create-checkout-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 karthi
 [Pharaoh Logging] [GitCommand] Attempting to create branch karthi
 Switched to a new branch 'karthi'
 Now in: /opt/ptconfigure-enterprise

 ******************************


 0 : In GitCommand View
 ******************************


delete-branch
-----------------

Dieser Befehl wird verwendet , um einen Zweig löschen, wenn vorhanden . Der Ausführungsprozess des Befehls ist , wie unten gezeigt ,

.. code-block:: bash

	ptconfigure git delete-branch --branch=*branchname*

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git delete-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevell
 [Pharaoh Logging] [GitCommand] Branch kevell exists, deleting...
 git branch -d mmmm
 Now in: /opt/ptconfigure-enterprise 

 ******************************


 0 : In GitCommand View
 ******************************


ensure-branch
----------------

Dieser Befehl wird verwendet, um eine Filiale besteht zu gewährleisten, wenn nicht eine neue Niederlassung schafft . Der Ausführungsprozess dieses Befehls ist unten aufgelistet ,

.. code-block:: bash

	ptconfigure git ensure-branch --branch=*branchname*

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git ensure-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevell
 [Pharaoh Logging] [GitCommand] Branch kevell does not exist, creating...
 Switched to a new branch 'kevell'
 Now in: /opt/ptconfigure-enterprise

 ******************************


 0 : In GitCommand View
 ******************************

.. code-block:: bash

 kevell@corp:/# ptconfigure git ensure-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 karthi
 [Pharaoh Logging] [GitCommand] Branch karthi already exists, continuing...
 Now in: /opt/ptconfigure-enterprise

 ******************************


 1 : In GitCommand View
 ******************************

Add
------

Der Befehl git add wird verwendet, um neue Dateien in das Git Repository hinzuzufügen. Der Ausführungsprozess dieses Befehls ist unten aufgelistet ,

.. code-block:: bash

	ptconfigure git add 

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git add
 
 Enter the file path to add ? (Enter nothing to add all new & modified files in the git repo).
 test1
 [Pharaoh Logging] All new files in the git repository were added
 ******************************


 0 : In GitCommand View
 ******************************

Commit
---------

Dieser Befehl wird verwendet , um neue Nachrichten auf die Git Repository zu begehen. Der Ausführungsprozess des Befehls ist , wie unten gezeigt ,

.. code-block:: bash

	ptconfigure git  commit --message=*some commit message*

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git commit

 Enter message to commit:
 testing
 [Pharaoh Logging] Git commit successfully
 ******************************


 0 : In GitCommand View
 ******************************


Push
----------

Dieser Befehl wird verwendet , um Dateien auf dem git-Repository schieben . Der Ausführungsprozess des Befehls ist , wie unten gezeigt ,

.. code-block:: bash

	ptconfigure git push --branch=*origin yourbranch*

Die bildliche Darstellung der obigen Befehl aufgelistet unten ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git push

 What branch?
 origin master
 Username for 'https://github.com': muralivel
 Password for 'https://muralivel@github.com': 
 Counting objects: 5, done.
 Delta compression using up to 2 threads.
 Compressing objects: 100% (3/3), done.
 Writing objects: 100% (5/5), 394 bytes | 0 bytes/s, done.
 Total 5 (delta 0), reused 0 (delta 0)
 To https://github.com/muralivel/kumar.git
  * [new branch]      master -> master
 [Pharaoh Logging] Git push to branch origin master successfully
 ******************************


 0 : In GitCommand View
 ******************************


Pull
----------

Dieser Befehl wird verwendet , um ein Git Repository zu ziehen. Der Ausführungsprozess des Befehls ist , wie unten gezeigt ,

.. code-block:: bash

	ptconfigure git pull --branch=*origin yourbranch*

Die bildliche Darstellung der obige Befehl wird , wie unten dargestellt ,

.. code-block:: bash


 kevell@corp:/# ptconfigure git pull

 What branch?
 origin master
 remote: Counting objects: 3, done.
 remote: Compressing objects: 100% (2/2), done.
 Unpacking objects: 100% (3/3), done.
 remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
 From https://github.com/muralivel/kumar
 * branch            master     -> FETCH_HEAD
   4f390f3..c3e9feb  master     -> origin/master
 [Pharaoh Logging] Git pull from branch origin master successfully
 ******************************


 0 : In GitCommand View
 ******************************



Alternative Parameter
--------------------------

Es gibt vier Parameter, die in alternativen Befehlszeile verwendet werden kann .

Git, GitCommand, git-command, gitcommand


Vorteile
--------------

* Freie und Open Source-
* Schnelle und kleine
* Implizite Backup
* Sicherheits
* Keine Notwendigkeit von leistungsfähiger Hardware
* Einfachere Verzweigung


