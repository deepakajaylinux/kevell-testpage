==============
Nginx Control
==============

Zusammenfassung
-----------------------

Nginx (sprich: "Motor-x") ist ein Open-Source-Reverse-Proxy-Server für HTTP, HTTPS, SMTP, POP3 und IMAP-Protokolle, sowie ein System zum Lastenausgleich, HTTP-Cache und einem Web-Server (Ausgangsserver). Die nginx Projekt begann mit einem starken Fokus auf hohe Parallelität, hohe Leistung und geringe Speicherverbrauch. Es wird unter der 2-Klausel-BSD-ähnlichen Lizenz veröffentlicht und auf Linux, BSD Varianten, Mac OS X, Solaris, AIX, HP-UX, als auch auf anderen nix Aromen.

Nginx verwendet eine asynchrone ereignisgesteuerten Ansatz für die Bearbeitung von Anträgen, statt des Apache HTTP-Server-Modell, die standardmäßig mit einer Gewinde oder prozessorientierten Ansatz, in dem die Veranstaltung MPM ist für asynchrone Verarbeitung erforderlich. Modular ereignisgesteuerte Architektur Nginx ist mehr vorhersagbare Leistung bei hohen Belastungen zu schaffen.

Hilfe Befehl
----------------------

Diese Funktion dient, um die Verwendung von Nginx Modul bestimmen. Der Benutzer wird kommen, um über die verschiedenen Möglichkeiten / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash
	
	ptdeploy nginxcontrol help
       
 kevell@corp:/# ptdeploy NginxControl help
 ******************************


  This command is part of Default Modules and handles Nginx Server Control Functions.

  NginxControl, nginxcontrol, nginxctl

          - start
          Start the Nginx server
          example: ptdeploy nginxcontrol start

          - stop
          Stop the Nginx server
          example: ptdeploy nginxcontrol stop

          - restart
          Restart the Nginx server
          example: ptdeploy nginxcontrol restart

          - reload
          Reloads the Nginx server configuration without restarting
          example: ptdeploy nginxcontrol reload

 ------------------------------
 End Help
 ******************************


Start
----------------

Wenn der Benutzer braucht, um die Nginx Server zu starten, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash
	
	ptdeploy nginxcontrol start                           

Vor der Ausführung ist das System fragen Sie nach der Bestätigung, um fortzufahren, wenn Sie fortfahren 'J' eingeben möchten, wenn keine geben 'N'.

Stopp
----------------

Wenn der Benutzer braucht, um die Nginx Server zu stoppen, wird der unten angegebenen Befehl den Prozess auszuführen.
.. code-block:: bash
	
	ptdeploy nginxcontrol stop	

Vor der Ausführung ist das System fragen Sie nach der Bestätigung, um fortzufahren, wenn Sie fortfahren 'J' eingeben möchten, wenn keine geben 'N'.

Neustart
----------------

Wenn der Benutzer braucht, um die Nginx Server neu starten (wenn es irgendwelche Änderungen geschehen in der Konfigurationsdatei wird diese Option verwendet werden kann), wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash
 	
	ptdeploy nginxcontrol restart                          

Vor der Ausführung ist das System fragen Sie nach der Bestätigung, um fortzufahren, wenn Sie fortfahren 'J' eingeben möchten, wenn keine geben 'N'.

Neu Laden
----------------

Wenn der Benutzer die Nginx Server ohne Neustart neu laden muss, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash
	
	ptdeploy nginxcontrol reload

Vor der Ausführung ist das System fragen Sie nach der Bestätigung, um fortzufahren, wenn Sie fortfahren 'J' eingeben möchten, wenn keine 
geben 'N'.


Options
-----------
                             

.. cssclass:: table-bordered

 +--------------------------+-----------------------------------------------------------------+-------------------------------------------+
 | Parameters               | Alternative Parameter                                           | Kommentare                                |
 +==========================+=================================================================+===========================================+
 |ptdeploy ngnixcontrolhelp | Entweder der drei alternativen Parameter kann das Kommando      | Sobald der Benutzer bietet die            |
 |                          | verwendet werden - ngnixcontrol , NgnixControl and nginxcil     | Möglichkeit, beginnt Systems Verarbeitung |
 |                          | eg: ptdeploy ngnixcontrol help/ ptdeploy ngnixControl help|     |                                           |
 +--------------------------+-----------------------------------------------------------------+-------------------------------------------+

 

Vorteile
--------------
   
* Fähigkeit, mehr als 10.000 gleichzeitige Verbindungen mit einem geringen Speicherbedarf verarbeiten
* Umgang mit statischen Dateien, Index-Dateien, und die Auto-Indizierung
* Reverse-Proxy mit Cache-
* Der Lastausgleich mit In-Band-Gesundheits-Checks
* Fehlertoleranz
* TLS / SSL mit SNI und OCSP-Heften Unterstützung, über OpenSSL.
* FastCGI, SCGI, uwsgi Unterstützung mit Caching
* Name- und IP-Adressen-basierte virtuelle Server
* IPv6-kompatibel
* SPDY-Protokoll-Unterstützung
* WebSockets und HTTP / 1.1-Upgrade (101 Switching Protocols)
* FLV und MP4-Streaming
* Internet- Zugriffsauthentifizierung
* Gzip Kompression und Dekompression
* URL-Rewriting
* Custom Logging mit on-the-fly gzip-Komprimierung
* Rücklaufquote und gleichzeitigen Anforderungen zu begrenzen
* Bandbreitendrosselung* Server Side Includes 
* IP address-based geolocation 
* User tracking 
* WebDAV 
* XSLT data processing 
* Embedded Perl scripting

