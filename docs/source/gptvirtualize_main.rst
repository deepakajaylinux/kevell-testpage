PTVirtualize
=============



Beim Vergleich mit ptconfigure ist die ptvirtualize eine virtuelle Maschine-Management-Tool, das die Funktionen für virtuelle Maschinen und Entwicklung Umweltmanagement bietet.

Durch die Verwendung von DevOps sie verwaltet die Konfiguration der virtuellen Maschine ermöglicht, die verschiedenen Arten der Beitragszahler auch in einer hochkomplexen Entwicklungsumgebung.

Es erleichtert die Automatisierung, Standardisierung und die Verwaltung der Einrichtung zu virtualisierten Umgebung. Seine Funktionalitäten beinhaltet Configuration Management, Test Automation-Management, Automated Deployment, Build und Release Management, Entwicklung Umweltmanagement und diese Funktionen durchgeführt werden.

In ptvirtualize das Configuration Management, Systems Automation und Infrastruktur ist in php umrahmt. Bearbeiten eines PHP-Skript ist sehr einfach, da es keine Kompilierung Schritt durchzuführen.

Die ptvirtualize ist objektorientiert, das nicht nur den Datentyp, sondern auch die Arten von Operationen, die auf die Daten angewendet werden kann, zu bereichern. Daher, während Vergleichen objektorientierte Programmiertechniken als Verfahrensprogrammiertechniken, die die objektorientierte Programmierung können die Endbenutzer auf Module, müssen nicht geändert werden, wenn ein neuer Typ von Objekt hinzugefügt erstellen.

Die ptvirtualize ist erweiterbar, als ob jede Zusatzmodul benötigt der Benutzer Rahmen und gestalten Sie das Modul nach ihren Anforderungen können und sie schließen kann.

Durch die Verwendung der Funktionalität der Template-Option extra Vorlagen können hinzugefügt werden, wenn erforderlich. Die Option SSH ermöglicht, eine SSH-Schlüssel Wert zu setzen. Die SFTP erleichtert die Lesbarkeit und Schreibfähigkeit zwischen den zwei verschiedenen OS mit Virtual Box.

Bedarf
-----------------

Wenn Sie die ptvirtualize verwenden möchten, stellen Sie sicher, ob der Virual Box wird in Ihrem Computer installiert ist, zusammen mit dem virtuellen Feld Gasterweiterungen Funktionalität


Code für die Installation von Virtual Box
-------------------------------------------

.. code-block:: bash

        sudo ptconfigure virtualbox install --yes --guess --with-guest-additions

Installation
-------------

Es gibt zwei Möglichkeiten, um die ptvirtualize Werkzeug, um Ihren Computer zu installieren:

1)Installation via ptconfigure

2)Installing ptvirtualize alone


Installation über ptconfigure
-------------------------------

wenn Sie ptconfigure Werkzeug in Ihrem Rechner haben, dann ist es einfach, die ptvirtualize indem Sie den Code wie unten angegeben zu installieren,

.. code-block:: bash


        sudo ptconfigure ptvirtualize install --yes --guess

Hier kann das Wort erraten ignoriert, während Sie Ihr eigenes Verzeichnis während der Installation werden.

Installieren ptvirtualize allein
-----------------------------------

Wenn Sie die ptvirtualize Werkzeug, um Ihre Maschine ohne je nach ptconfigure Tool installieren wollen, ist es einfacher, mit dem Befehl,

.. code-block:: bash

        sudo apt-get install php5 git
        
this command will install php5 and git on your machine. After that use the following command,::

        git clone http://github.com/PharaohTools/ptvirtualize && sudo php ptvirtualize/install-silent

the command on the above mentioned can be used if you don't want to select the location during the installation. If you wish to do so, use the following command::

        git clone http://github.com/PharaohTools/ptvirtualize && sudo php ptvirtualize/install

Methoden in Nutzung
---------------------------

Hier wollen wir sehen, wie man die Befehle unter dem Werkzeug und seine Nutzung zu verwenden.

wenn Sie geben Sie einfach den folgenden Befehl ein, ::

    ptvirtualize

Wie in der Abbildung unten werden Sie die Anzeige aller unter diesem Tool Module erhalten. ::


 kevell@corp:/# ptvirtualize
 ******************************
 Pharaoh Tools - Virtualize
 ******************************


 Virtualize by Golden Contact Computing
 -------------------

 About:
 -----------------
 Virtualize is for controlling Virtual Machines in Development Environments.

 -------------------------------------------------------------
 
 Available Commands:
 ---------------------------------------

 AutoSSH - AutoSSH - Use your Papyrus details to automatically SSH or SFTP into your Virtualize box
 Box - Box - Manage Base Boxes for Virtualize
 Destroy - Destroy - Stop a Virtualize Box
 Flirtify - Virtualize Flirtify - Generate a Phalgrantfile
 Halt - Halt - Stop a Virtualize Box
 Invoke - SSH Invocation Functions
 PharaohTools - Pharaoh Tools Provisioner Integration
 Provision - Provision - Stop a Virtualize Box
 Resume - Resume - Stop a Virtualize Box
 SFTP - SFTP Functionality
 Shell - Shell Provisioner Integration
 Status - Status - Stop a Virtualize Box
 SystemDetection - System Detection - Detect the Running Operating System
 Up - Up - Create and Start a Virtualize Box
 Virtualbox - Virtualbox Provider Integration

 ******************************



Hilfe Befehl:
---------------

Es ist einfach, um den Befehl Hilfe verwenden,

.. code-block:: bash

	ptvirtualize Module Hilfe

Dieser Befehl hilft Ihnen, wie die einzelnen Module arbeitet, und auch über das, was sind die Maßnahmen, die sie durchführen.
Die folgende Abbildung erklärt Ihnen, wie Sie den Befehl help wird verwendet, um das Modul autossh erklären. ::

    kevell@Corp:/#ptvirtualize AutoSSH help

    ******************************
    Pharaoh Tools - Virtualize
    ******************************


    This command allows you to autoSSH a ptvirtualize box

    AutoSSH, auto-ssh, autossh, ssh, SSH

        - cli
        Open an SSH Cli to your ptvirtualize Box
        example: ptvirtualize auto-ssh cli --yes --guess

        - sftp-put
        SFTP Put a file on to your ptvirtualize Box
        example: ptvirtualize auto-ssh sftp-put --yes --guess --source=/path/to/source --target=/path/to/target

        - sftp-get
        SFTP Get a file from your ptvirtualize Box
        example: ptvirtualize auto-ssh sftp-get --yes --guess --source=/path/to/source --target=/path/to/target

    ------------------------------
    End Help
    ******************************

kurze Beispiel
-----------------

lassen Sie uns über ein kurzes Beispiel in Bezug auf die ptvirtualize hier zu sehen.

create a directory, or simply use a current web project as your new Pharaoh project mkdir /var/www/my-test-project && cd /var/www/my-test-project

install virtualbox to your machine if you don't have it already, it's simple by using the command as follows,::

    sudo ptconfigure virtualbox install --yes --guess --with-guest-additions

add a default ptconfigure Configuration Management Autopilot file using the following command::

    sudo ptconfigure cleofy install-generic-autopilots --yes --guess --template-group=ptvirtualize

flirtify ptvirtualize flirt now --template-group=default-php

install, configure and start the virtual machine ptvirtualize up now




Das Spiel mit ptvirtualize Module
------------------------------------

.. toctree::
   :maxdepth: 3


 gautossh_virtualize
 gbox_virtualize
 gdestroy_virtualize
 gflirtify_virtualize
 ghalt_virtualize
 ginvoke_virtualize
 gpharaohtools_virtualize
 gresume_virtualize
 gsftp_virtualize
 gshell_virtualize
 gstatus_virtualize
 gsystemdetection_virtualize
 gup_virtualize
 gvirtualbox_virtualize


