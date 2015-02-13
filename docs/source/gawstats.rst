=========
Awstats
=========


Zusammenfassung
-----------------

Dieses Modul fördert die Installation von Awstats, mit der neuesten Version. AWStats ist ein open-Source-Web-Analytics, reporting-Tool, geeignet zur Analyse von Daten von Internet-Diensten wie Web, streaming Media, Mail und FTP-Servern. AWStats analysiert und analysiert Server-Log-Dateien, Erstellung von HTML-Berichten.

AWStats (Advanced Web Statistics) ist ein leistungsfähiges, voll funktionsfähige Web-Server-Logfile-Analyzer zeigt Sie alle Ihre Web-Statistiken, einschließlich: Besucher, Seiten, Hits, Stunden, Suchmaschinen, Schlüsselwörter verwendet, um Ihre Website, broken Links, Roboter und vieles mehr finden.

Lassen Sie uns sehen Sie, die Details dieser Awstats, die Funktionen und Anforderungen von Awstats in anstehende Themen zu installieren.


Hilfe Befehl
------------------

Der Help-Befehl führt die Benutzer über den Zweck und auch als zu den Optionen, die in dem AWStats-Modul enthalten sind. Es listet die alternative Ausgabeparameter von AWStats-Modul. Es beschreibt auch die Syntax für die Installation von AWStats-Modul. Der Help-Befehl für AWStats-Modul wird gezeigt wie unten beschrieben.

.. code-block:: bash

                cleopatra AWStats Help

Die Syntax zum Deklarieren des Help-Befehls ist nicht Groß-/Kleinschreibung einen zusätzlichen Vorteil. Der folgende Screenshot visualisieren Sie über den Befehl Help unter AWStats.

Installation
-------------------


Der Befehl für die Installation der AWStats auf dem Benutzer-Computer verwendet wird unten gezeigt.

.. code-block:: bash

		cleopatra AWStats install


Nach Eingabe des obigen Befehls, geschieht Folgendes, wie in tabellarischer Form dargestellt.

.. cssclass:: table-bordered

 +-----------------------------+----------------------------------------+------------------+------------------------------------------------+
 | Parameter                   | Alternative Parameter                  | Optionen         | Kommentare                                     |
 +=============================+========================================+==================+================================================+
 |Install AWStats? (Y/N)       | Anstelle von AWStats können wir auch   | Y(Yes)           | Wenn der Benutzer den Installationsvorgang     |
 |                             | Awstats Verwendung awstats.            |                  | fortsetzen möchten, können sie als Y eingeben. |
 +-----------------------------+----------------------------------------+------------------+------------------------------------------------+
 |Install AWStats? (Y/N)       | Anstelle von AWStats können wir auch   | N(No)            | Wenn der Benutzer den Installationsvorgang zu  |
 |                             | Awstats Verwendung awstats.            |                  | beenden möchten können sie eingeben, als N.|   |
 +-----------------------------+----------------------------------------+------------------+------------------------------------------------+

Wenn der Benutzer die Installation wird fortgesetzt, wird der folgende Prozess während der Installation von beteiligt:

* Liest die Paketliste.
* Baut der Abhängigkeitsstruktur.
* Installiert die erforderlichen zusätzlichen Pakete
* Die vorgeschlagene Pakete installiert.
* Die neuen Pakete installiert.


Schließlich Ruft die Installation von Awstats erfolgreich wie in den folgenden Screenshots dargestellt abgeschlossen:

.. code-block:: bash


Features von Awstats
------------------------------

Eine vollständiges Protokoll-Analyse ermöglicht AWStats Ihnen zeigen, dass die folgende Informationen:


* Anzahl der Besuche und Besucher
* Besuche von Dauer und zuletzt besucht
* Authentifizierte Benutzer und letzte authentifizierte Besuche
* Tage der Woche und Stoßzeiten (Seiten, Hits, KB für jeden Tag und jede Stunde)
* Domains/Länder der Gastgeber Besucher (Seiten, Hits, KB)
* Gastgeber-Liste, letzten Besuche und nicht aufgelöste IP-Adressen-Liste
* Am meisten angesehen, Eingangs-und Ausgangsseiten
* Dateitypen
* Web-Kompression-Statistiken (für Mod_gzip oder Mod_deflate)
* Verwendeten Browser (Seiten, Hits, kb für jeden Browser)
* OS verwendet (Seiten, Hits, für jedes Betriebssystem KB)
* Robot-Besuche
* Wurm-Attacken
* Download und Fortsetzung Erkennung
* Suchmaschinen, Phrasen und Schlüsselwörter verwendet, um Ihre Website zu finden
* HTTP-Fehler (Seite nicht gefunden mit letzten Referer, usw.)
* Bildschirm Größe Bericht
* Wie oft Ihre Website "Favoriten Lesezeichen hinzugefügt wird"
* Verhältnis von Browsern, die unterstützen: Java, Flash, Quicktime-Leser, WMA-Leser, RealG2 Reader, PDF-Reader
* Bericht für Belastungsverhältnis ausgewogene Server Cluster
* Andere personalisierte Berichte...


Es unterstützt auch die folgenden Features:


* Können alle Protokollformate analysieren
* Werke von der Kommandozeile aus und über einen Browser als CGI (durch dynamische Filter-Funktionen für einige Diagramme)
* Aktualisierung der Statistiken kann bei Bedarf über das Webinterface und nicht nur aus Ihrem Planer gemacht werden
* Unbegrenzten Protokolldateigröße, Unterstützung Split-Log-Dateien (load balancing System)
* Unterstützen Sie "fast sortierten" Log-Dateien auch für Eingangs-und Ausgangsseiten
* Reverse-DNS-Lookup vor oder während der Analyse unterstützt DNS-Cache-Dateien
* Land-Erkennung von IP-Lage oder Domänennamen
* WhoIS-links
* Viele Optionen/Filter und Plugins kann verwendet werden
* Multi benannte Websites unterstützt (virtuelle Server)
* Cross Site Scripting Attacken Schutz
* Mehrere Sprachen
* Kein Bedarf an seltenen Perl-Bibliotheken
* Dynamische Berichte als CGI-Ausgaben
* Statische Berichte in einem oder gerahmt HTML- oder XHTML-Seiten
* Experimentelle PDF-export
* Aussehen und Farben können Ihr Site-Design (CSS) entsprechen.
* Hilfe und Tooltips auf HTML Seiten gemeldet
* Einfach zu bedienen (nur eine Konfigurationsdatei zu bearbeiten)
* Analysedatenbank kann im XML-Format (für XSLT-Verarbeitung,...) gespeichert werden
* Ein Webmin-Modul
* Kostenlos (GNU GPL) mit Quellen (Perl-Skripte)
* Auf allen Plattformen verfügbar


Anforderungen von Awstats
-----------------------------------------

Um AWStats CGI-Skript zu verwenden, benötigen Sie die folgenden Anforderungen:

* Ihre Server melden Webzugriff in einer Protokolldatei können Sie lesen.
* Um Awstats, von Kommandozeile auszuführen, muss Ihr Betriebssystem zum Ausführen von Perl-Skripten (.pl Dateien) können.
* Perl-Modul "Codieren" muss vorhanden sein.


Um Awstats als CGI (für Echtzeit-Statistiken) auszuführen, muss Ihr Webserver auch solche Skripte ausführen können.


 Ist dies nicht der Fall, Sie können dies beheben, indem letzte Perl Version herunterladen:

 http://www.activestate.com/ActivePerl/ (Windows)
 
 http://www.perl.com/pub/Language/Info/Software.html (All OS)


Dateien
-----------------

Die Verteilung von AWStats-Paket enthält die folgenden Dateien:


.. cssclass:: table-bordered

 +------------------------------------+---------------------------------------------------+
 | Packages                           | Dateien                                           |
 +====================================+===================================================+
 |README.TXT                          | Diese Datei                                       |
 +------------------------------------+---------------------------------------------------+
 |docs/LICENSE                        | GNU General Public Licence                        |
 +------------------------------------+---------------------------------------------------+
 |docs/*                              | AWStats Dokumentation (Installation/Nutzung...)   |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/cgi-bin/awstats.pl          | DIE AWSTATS-HAUPTPROGRAMM (CLI/CGI)               |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/cgi-bin/awredir.pl          | Ein Tool zur Ausfahrt Klicks verfolgen            |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/cgi-bin/awstats.model.conf  | Eine Modell-Konfigurationsdatei                   |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/cgi-bin/lang                | Verzeichnis mit Sprachen-Dateien                  |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/cgi-bin/lib                 | Verzeichnis mit Awstats Referenz info             |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/cgi-bin/plugins             | Verzeichnis mit optionalen plugins                |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/icon/browser                | Verzeichnis mit Browser-icons                     |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/icon/clock                  | Verzeichnis mit Uhr-Symbole                       |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/icon/cpu                    | Verzeichnis mit cpu-Symbole                       |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/icon/flags                  | Verzeichnis mit Land-Flaggen-icons                |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/icon/os                     | Verzeichnis mit OS-Symbole                        |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/icon/other                  | Verzeichnis mit allen anderen Symbolen            |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/classes                     | Java-Applet für Graphapplet plugin                |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/css                         | Beispiele für CSS-Dateien                         |
 +------------------------------------+---------------------------------------------------+
 |wwwroot/js                          | JavaScript-Quellen für "Sonstiges" feature        |
 +------------------------------------+---------------------------------------------------+
 |tools/*                             | Andere bereitgestellten tools                     |
 +------------------------------------+---------------------------------------------------+
 |tools/webmin/awstats-x.x.wbm        | Ein Webmin-Modul für AWStats                      |
 +------------------------------------+---------------------------------------------------+
 |tools/xslt/awstats61.xsd            | AWStats XML-Datenbank-Schema-Deskriptor           |
 +------------------------------------+---------------------------------------------------+
 |tools/xslt/*                        | Demo manipuli AWStats XML datenbazo|              |
 +------------------------------------+---------------------------------------------------+

                            


Vorteile
--------------

* Die Parameter in der Hilfe verwendet und Installation und un Installationsvorgänge Groß-/Kleinschreibung keinen zusätzlichen Vorteil, 
  während im Vergleich zu anderen ist.
* Es ist gut situierten, in beiden Ubuntu und auch als Cent OS.
* Dieses Modul wird installiert die Awstats in aktualisierte Version.
* Wenn das Modul bereits in den Benutzer-Computer vorhanden ist, wird es eine Meldung angezeigt, wie dieses bereits vorhanden ist.
* AWStats unterstützt die meisten wichtigen Web Server Log Dateiformate einschließlich Apache (NCSA kombiniert/XLF/ELF-Protokollformat oder 
  Common Log Format (CLF)), WebStar, IIS (W3C-Protokolldateiformat) und viele andere gemeinsame Web Server Log-Formate.
* Entwickler können dem AWStats-Projekt über SourceForge.net beitragen.
* In Perl geschrieben, kann AWStats auf fast jedem Betriebssystem bereitgestellt werden
* Es ist ein Server-Verwaltungstool, mit Paketen für die meisten Linux-Distributionen verfügbar.
* AWStats kann auf einer Workstation für den lokalen Gebrauch in Situationen wie MS Windows, installiert werden, wo Log-Dateien von einem 
  remote-Server heruntergeladen werden kann.
 
