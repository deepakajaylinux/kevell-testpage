==========
Memcached
==========

Zusammenfassung
---------------

Der Hauptaspekt dieses Moduls ist für die Installation und Aktualisierung der memcache mit der neuesten Version.
Memcached ist ein Mehrzweck-Distributed-Memory-Caching-System. Es wird häufig verwendet, um durch die Zwischenspeicherung von Daten und Objekten im Arbeitsspeicher, um die Anzahl, wie oft eine externe Datenquelle (wie zB einer Datenbank oder API) hinausgehen, darf gelesen werden beschleunigen dynamische Datenbank-gestützte Websites.


Lassen Sie uns über den Prozess der Installation und Verwendung dieses Moduls im kommenden Themen sehe

Hilfe Befehl
---------------------

Der Befehl help führt den Anwender über den Zweck und als auch über die Möglichkeiten, die in der Memcached-Modul enthalten sind. Es listet einige der alternativen Parameter der Memcached-Modul. Es beschreibt auch die Syntax für die Installation des Memcached Moduls. Der Befehl help für Memcached-Modul ist wie unten dargestellt.

.. code-block:: bash

		ptconfigure  Memcached help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Memcached.

.. code-block:: bash

 kevell@corp:/# ptconfigure Memcached help

 ******************************


  This command allows you to update Memcached.

  Memcached, memcached

        - install
        Installs the latest version of memcache
        example: ptconfigure  memcached install

 ------------------------------
 End Help
 ******************************

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter Memcached.
Nach der Eingabe des Befehls oben, passiert folgendes Verfahren im Tabellenformat angezeigt.

.. cssclass:: table-bordered


 +-------------------------+-------------------------------------------+-------------+------------------------------------------+
 | Parameter               |  Alternative Parameter                    | Optionen    | Kommentare                               |
 +=========================+===========================================+=============+==========================================+
 |Install Memcached? (Y/N) | Statt of memcached wir verwenden können,  | Y(Yes)      | Wenn der Benutzer wünschen, den          |
 |                         | Memcached also.                           |             | Installationsprozess können sie          |
 |                         |                                           |             | Eingang als Y gehen                      |
 +-------------------------+-------------------------------------------+-------------+------------------------------------------+
 |Install Memcached? (Y/N) | Statt of memcached wir verwenden können,  | N(No)       | Wenn der Benutzer wünschen, den          |
 |                         | Memcached also.                           |             | Installationsprozess können sie          |
 |                         |                                           |             | Eingang als N. beenden|                  |
 +-------------------------+-------------------------------------------+-------------+------------------------------------------+

Der folgende Screenshot kann Ihnen eine bildliche Darstellung in Bezug auf den Prozess der Installation.

Funktionen des Memcached
-------------------------------

Während der Verwendung des Memcached kann der Prozess zu lesen und umzusetzen, die folgenden Funktionen, die im memcached enthalten sind,

* Memcache :: hinzufügen - Setzen Sie einen Artikel auf den Server
* Memcache :: addServer - zum Verbindungspool hinzufügen Memcached Server
* Memcache :: close - Close Memcached-Server-Verbindung
* Memcache :: connect - Offene Memcached-Server-Verbindung
* Memcache :: Dekrement - Wert Decrement Elements
* Memcache :: löschen - Los Löschen vom Server
* Memcache :: flush - alle vorhandenen Einträge auf dem Server
* Memcache :: get - abrufen Artikel vom Server
* Memcache :: getExtendedStats - Holen Sie Statistiken für alle Server im Pool
* Memcache :: GetServerStatus - Gibt den Serverstatus
* Memcache :: getStats - Get Statistiken des Servers
* Memcache :: getVersion - Return Version des Servers
* Memcache :: Schritt - Wert Schrittweite Elements
* Memcache :: pconnect - Offene Memcached Server persistente Verbindung
* Memcache :: ersetzen - Wert der bestehenden Artikel ersetzen
* Memcache :: set - Speichern Sie Daten auf dem Server
* Memcache :: setCompressThreshold - Aktivieren Sie die automatische Komprimierung von großen Werten
* Memcache :: setServerParams - Änderungen Server Parameter und Status zur Laufzeit

Vorteile
------------

* Die in Hilfe und Installation verwendet muss nicht beachtet werden, welche ein zusätzlicher Vorteil ist, während im Vergleich zu anderen 
  Parametern.
* Es ist gut-to-do sowohl Ubuntu und sowie Cent OS.
* Dies wird Modul installiert die Memcached in aktualisierte Version.
* Wenn das Modul bereits in der Benutzermaschine vorhandene es wird eine Meldung angezeigt werden, da sie bereits vorhanden sind.

