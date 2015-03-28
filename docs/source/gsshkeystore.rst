============
SshKeyStore 
============

Zusammenfassung
-----------------------

SSH oder Secure Shell, ist eine verschlüsselte Protokoll zu verwalten und mit Servern kommunizieren. Bei der Arbeit mit einem Linux-Server, die Chancen sind, werden Sie die meiste Zeit verbringen, in einer Terminal-Sitzung auf den Server über SSH verbunden ist.

SSH-Schlüssel sind eine Möglichkeit, vertrauenswürdige Computer zu identifizieren, ohne Einbeziehung Passwörter. SSH-Schlüssel bieten eine sichere Möglichkeit, die Anmeldung in einer Linux- und Unix-basierten Server.

OpenSSH-Server unterstützt verschiedene Authentifizierungsschemas . Die beiden beliebtesten sind wie folgt:

1. Passwörter basierte Authentifizierung

2. Öffentliche Schlüssel basierte Authentifizierung. Es ist eine Alternative Sicherheitsmethode, um die Verwendung von Kennwörtern. Diese 
   Methode basiert auf einem VPS empfohlen, Wolke, dedizierte oder sogar zu Hause basierten Server.

In Public-Key-Methode, die Sie in die Remote-Hosts und Server anmelden können, und Dateien zu übertragen, um sie, ohne mit Ihrem Account-Passwörter. Dieses Modul ermöglicht es Ihnen, die Anmeldeinformationen für einen Schlüssel auf einer Maschine zu finden.

Hilfe Befehl
----------------------

Diese Funktion dient, um die Verwendung von sshkeystore Modul bestimmen. Der Benutzer wird kommen, um über die andere Art und Weise / Format um dieses Modul ausführen kennen. Dieser Befehl leitet den Anwender, um den Zweck dieses Befehls kennen. Da unten sind die Kommando- und der Screenshot der gleiche.

.. code-block:: bash
        
        ptconfigure sshkeystore help

Der Screenshot für den obigen Befehl aufgelistet unten,

.. code-block:: bash

 kevell@corp:/# ptconfigure SshKeyStore help
 ******************************

  This command allows you to find credentials for a key on a machine

  SshKeyStore, sshkeystore, ssh-key-store

        - find
        Add an SSH Public Key to an account
        example: ptconfigure ssh-key-store find --key=daveylad
        example: ptconfigure ssh-key-store find --key=daveylad --prefer=user

 ------------------------------
 End Help
 ******************************

finden
--------

Wenn der Benutzer braucht, um eine SSH Public Key auf ein Konto hinzufügen, wird der unten angegebenen Befehl den Prozess auszuführen.

.. code-block:: bash
        
	        ptconfigure ssh-key-store find --key=daveylad


.. code-block:: bash

 kevell@corp:/# ptconfigure ssh-key-store find --key=id_rsa
 [Pharaoh Logging] Trying keystore keys
 Enter User home directory:
 /
 [Pharaoh Logging] User key not found at //.ssh/id_rsa
 Enter User home directory:
 /
 [Pharaoh Logging] Other User key not found at //.ssh/id_rsa
 [Pharaoh Logging] Root key found at /root/.ssh/id_rsa
 ******************************


 SshHarden Modifications:
 --------------------------------------------

 Ssh Key Store: Success
 /root/.ssh/id_rsa

 ------------------------------
 SshHarden Mods Finished
 ******************************



Alternative Parameter
--------------------------------

Es gibt zwei alternative Parameter, die in der Befehlszeile verwendet werden kann.

SshKeyStore, sshkeystore, ssh-key-store 

Example: ptconfigure sshkeystore help /ptconfigure ssh-key-store help

Vorteile
--------------

* Die privaten SSH-Schlüssel (der Teil, Passwort geschützt werden kann), wird nie im Netzwerk ausgesetzt. Die Passphrase wird nur verwendet, 
  um zu entschlüsseln der Schlüssel auf dem lokalen Rechner. Das bedeutet, dass netzwerkbasierte brute force nicht möglich sein wird gegen die 
  Passphrase.

* Der private Schlüssel wird in einem begrenzten Verzeichnis gespeichert. Der SSH-Client wird keine privaten Schlüssel zu erkennen, die 
  nicht i eingeschränkten gehalten werden Verzeichnisse. Der Schlüssel selbst müssen auch Berechtigungen (Lesen und Schreiben nur für den 
  Besitzer verfügbar) beschränkt. Dies bedeutet, dass andere Benutzer des Systems kann nicht snoopen.

* Jede Angreifer hofft, den privaten SSH-Schlüssel Passwort knacken müssen bereits Zugriff auf das System. Das heißt, sie wird bereits
  Zugriff auf Ihr Benutzerkonto oder den Root-Account. 

  Wenn Sie in dieser Position sind, kann das Passwort der Angreifer sofort verhindern Anmeldung in Ihrem anderen Servern. Das wird sich 
  hoffentlich Zeit für die Erstellung und Umsetzung eines neuen SSH-Schlüsselpaar, und entfernen Sie den Zugriff von der Ihnen kompromittierten   Schlüssel.
