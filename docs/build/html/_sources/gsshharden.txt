=============
SshHarden
=============

Zusammenfassung
-----------------------

Dieses Modul hilft bei der Erstellung und Bearbeitung von sshhardens. Der ssh verhärten erleichtert Sicherheitsfunktionen für die Benutzer SSH-Konten.

Hilfe Befehl
----------------

Der Befehl help führt die Benutzer über den Zweck und als auch über die Möglichkeiten, die in der SSH verhärten Modul enthalten sind. Der Befehl help Listen aus der alternativen Parameter SSH verhärten. Es beschreibt auch die Syntax für die Verwendung von SSH verhärten zu Securify. Der Befehl help für SSH verhärten wird unten gegeben.

.. code-block:: bash

	ptconfigure SshHarden help

Die Syntax für die Deklaration den Befehl help ist nicht case sensitive was ein zusätzlicher Vorteil ist. Der folgende Screenshot visualisieren Sie den Befehl help unter SSH Harden.

.. code-block:: bash

	Kevell@corp:/# ptconfigure SshHarden help
	
	******************************


        This command allows you to modify create or modify sshhardens

	SshHarden, sshharden, ssh-harden

        - securify
        Add some security to your SSH accounts
        example: ptconfigure ssh-harden securify

	------------------------------
	End Help
	******************************

Securify
-----------

Der Befehl für die Nutzer securifying SSH Konto über SSH verhärten verwendet wie folgt dar:

.. code-block:: bash

	ptconfigure ssh-harden securify

Nach der Eingabe des Befehls wie oben die Installation von Ssh Härten gegeben beginnt wie im Tabellenformat angezeigt.

.. cssclass:: table-bordered

 +-------------------------+-------------------------------------------+-------------+-----------------------------------------+
 | Paramaters              | Alternative Parameter                     | Optionen    | Kommentare                              |
 +=========================+===========================================+=============+=========================================+
 |Install Ssh Hardening?   | anstelle von Ssh HardeningDie folgenden   | Y(Yes)      | Wenn der Benutzer wünschen, den         |
 |(Y/N)                    | Alternativen können ebenfalls verwendet   |             | Installationsprozess können sie Eingang |
 |                         | werden: SshHarden, sshharden, ssh-harden. |             | als Y. gehen                            |
 +-------------------------+-------------------------------------------+-------------+-----------------------------------------+
 |Install Ssh Hardening?   | anstelle von Ssh HardeningDie folgenden   | N(No)       | Wenn der Benutzer wünschen, den         |
 |(Y/N)                    | Alternativen können ebenfalls verwendet   |             | Installationsprozess können sie Eingang | 
 |                         | werden: SshHarden, sshharden, ssh-harden. |             | als N. Beenden|                         |
 +-------------------------+-------------------------------------------+-------------+-----------------------------------------+

Wenn der Benutzer geht die Installation von Ssh verhärten, die securifying ssh Konto von Benutzern ermöglicht wird eingeleitet. Während der Prozess der Ausführung auftritt, wird der sshd Konfigurations modifiziert, dass Root SSH-Login und sowie sshd Konfigurations geändert wird, die Passwortbasierte SSH-Login verbietet verbietet. schließlich wird es die ssh-Dienst neu gestartet und die Ergebnisse der abgeschlossenen Ssh Harden Modifikationen. Der folgende Screenshot erklärt die oben genannten Verfahren bildlich.

.. code-block:: bash

 kevell@corp:/# ptconfigure sshharden securify
 Install Ssh Hardening? (Y/N) 
 y
 [Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
 [Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
 [Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
 [Pharaoh Logging] [File] Writing File /etc/ssh/sshd_config
 [Pharaoh Logging] /etc/ssh/sshd_config modified to disallow root ssh login
 [Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
 [Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
 [Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
 [Pharaoh Logging] [File] Writing File /etc/ssh/sshd_config
 [Pharaoh Logging] /etc/ssh/sshd_config modified to disallow password based ssh login
 [Pharaoh Logging] Restarting ssh service
 ssh stop/waiting
 ssh start/running, process 12828
 ******************************


 SshHarden Modifications:
 --------------------------------------------

 Ssh Hardening: Success

 ------------------------------
 SshHarden Mods Finished
 ******************************





Vorteile
------------

* Diese Ssh verhärten wirkt wie ein Verstärker, der die Sicherheitsfunktionen der Nutzer SSH-Konten ermöglicht.
* Die in Hilfe und securifying verwendeten Parameter werden die Installationsvorgänge nicht beachtet, welche ein zusätzlicher Vorteil ist, 
  während im Vergleich zu andere.
* Dieses Modul ermöglicht Änderung der ssh verhärten Config, die Wurzel ssh Login, Passwort basierte SSH-Login verbietet.

