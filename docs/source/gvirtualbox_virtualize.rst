=============
Virtualbox
=============

Zusammenfassung
-----------------------

Dieses Modul ermutigen Installation der Stimme. Bei ptvirtualize Modul vollständig durch virtuelle Box verwaltet. Es ist benutzerfreundlich mit Ubuntu und Cent-OS. Die Virtual Box-Paket installiert auf einem vorhandenen Host-Betriebssystem als Anwendung. Benutzer von Virtual Box können mehrere Gastbetriebssysteme unter einem Host-Betriebssystem zu laden. Virtual Box unterstützt hat Open Virtualization Format (OVF) .Dies ist komfortabel mit Ubuntu und Cent OS.

Hilfe Befehl
-----------------------

Der Befehl help führen den Benutzer zu virtuellen Box in ptvirtualize installieren. Dieser Befehl help führt den Benutzer zu einem virtuellen Host erstellen. Dies zeigt auch, um einen virtuellen Host einen virtuellen Host hinzufügen, entfernen Sie einen virtuellen Host, aktivieren Sie einen virtuellen Host, und deaktivieren.

Der Befehl help für Virtual Box ist nachfolgend dargestellt.

.. code-block:: bash

	ptvirtualize virtualbox help

Nach Eingang der obige Befehl, beginnt es funktioniert, um einen virtuellen Host-Editor hinzufügen. Es Katechese die Funktionen in den Screenshots.

Der folgende Screenshot zeigt etwa die Installation von Virtual Box.

.. code-block:: bash


Installation
---------------------

Dieses Modul den Benutzer anweisen, zu installieren. So aktivieren Sie virtuelle Box folgen Sie den Befehl wie,

ptvirtualize virtual box install

Then the system can enquire

ptvirtualize virtual box install? (Y/N) 

If the user enters Y then it will be installed, else it will exit the screen.


Options
--------------


.. cssclass:: table-bordered

 +------------------------------+-------------------------------------------+------------+-------------------------------------------+
 | Parameters                   | Alternative parameter                     | Option     | Kommentare                                | 
 +==============================+===========================================+============+===========================================+
 |Install virtual box? (Y/N)    | Anstelle der Verwendung Virtualbox der    | Yes        | Unter ptvirtualize Modul erfolgreich      |
 |                              | Benutzer verwenden können, virtual box    |            | installiert                               |
 +------------------------------+-------------------------------------------+------------+-------------------------------------------+
 |Install virtual box? (Y/N)    | Anstelle der Verwendung Virtualbox der    | No         | Verlassen Sie das Bild                    |
 |                              | Benutzer verwenden können, virtual box|   |            |                                           |
 +------------------------------+-------------------------------------------+------------+-------------------------------------------+



Vorteile
---------------

* Voice können über dieses Modul installiert werden.
* Beide ISO-Images und Host verbundenen physischen Geräten können als CD / DVD-Laufwerke montiert werden.
* Das DVD-Bild von einer Linux-Distribution heruntergeladen und direkt von VirtualBox verwendet werden.
