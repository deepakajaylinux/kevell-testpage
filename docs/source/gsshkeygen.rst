============
SshKeygen
============

Zusammenfassung
--------------------------

Es ist ein Hilfsmittel, um den Schlüsselwert zu generieren. Dieses Modul ist mit zwei Schlüsselarten. Sie sind dsa, rsa. DSA-Schlüssel-Bit-Wert ist 1024 und die RSA-Schlüssel-Bit-Wert ist mehr als 768. Nur dann kann es funktionieren. Es ist handlich in Aufgabe mit Ubuntu und Cent-OS.

Hilfe Befehl
---------------

Dieser Befehl help erklärt über die Installation eines bestimmten Moduls. Der Befehl help leicht durch den Endverbraucher bedienen. Der folgende Befehl geführte den Benutzer über die Installation

.. code-block:: bash
		
		ptconfigure Sshkeygen  help

Nachdem er den Befehl, wird der Befehl die Hilfe-Optionen aufgelistet. Die folgenden Screenshots geben visuellen Effekt für den Einsatz dieses Moduls.

.. code-block:: bash

 kevell@corp:/# ptconfigure SshKeygen help
 ******************************


  This command allows you to install an SSH Key Pair.

  SshKeygen, ssh-keygen, sshkeygen

        - install
        Installs a new SSH Key
        example: ptconfigure ssh-keygen install
        example: ptconfigure ssh-keygen install --yes --bits=4096 --type=rsa --path="/home/dave/.ssh/id_rsa" --comment="Daves"

        - uninstall
        Removes an SSH Key
        example: ptconfigure ssh-keygen uninstall

 ------------------------------
 End Help
 ******************************


Installation
-------------

Die Installation ist nicht ein schwieriger Prozess, um dieses Modul unter ptconfigure lediglich durch Verwendung des Befehls unten angegeben zu installieren,

.. code-block:: bash

		ptconfigure sshkeygen install


Nach Eingabe Eingänge SSH-Schlüssel gen erfolgreich installiert werden. Die folgenden Screenshots geben visuellen Effekt für den Einsatz dieses Moduls.

.. code-block:: bash

 kevell@corp:/# ptconfigure ssh-keygen install
 Install SSH Key Generation? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         sshkeygen!        *
 *******************************
 Enter number of bits for SSH Key (multiple of 1024):
 1024
 Choose Key type (rsa/dsa)
 (0) rsa 
 (1) dsa 
 1
 Enter path to store private key (public key will be same with .pub):
 /root/SSH/abcd
 Plain text comment appended to public key. None is fine
 kevell
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 SshKeygen: Success
 ------------------------------
 Installer Finished
 ******************************



Options
---------


.. cssclass:: table-bordered

 +--------------------------+-------------------------+--------------+--------------------------------------------------------+
 | Parameters               | Verzeichnis (Standard)  | Optionen     | Kommentare                                             |
 +==========================+=========================+==============+========================================================+
 |Install Key Generation    | Yes                     |              | Es wird die Schlüsselgenerierung unter ptconfigure     |
 |                          |                         |              | installieren                                           |
 +--------------------------+-------------------------+--------------+--------------------------------------------------------+
 |Install Key Generation    | No                      |              | Der Benutzer hat zu einem Ausgang.                     |
 +--------------------------+-------------------------+--------------+--------------------------------------------------------+
 |Choose key type           | rsa                     | 0            | Es wird die Schlüsselgenerierung unter ausgewählten    |
 |                          |                         |              | Schlüsseltyp installieren                              |
 +--------------------------+-------------------------+--------------+--------------------------------------------------------+
 |Choose key type           | dsa                     | 1            | Es wird die Schlüsselgenerierung unter ausgewählten    |
 |                          |                         |              | Schlüsseltyp installieren                              |
 +--------------------------+-------------------------+--------------+--------------------------------------------------------+
 |path                      | /root/ssh/filename      |              | Es wird die Datei mit den öffentlichen und den         |
 |                          |                         |              | privaten Schlüssel zu erstellen                        |
 +--------------------------+-------------------------+--------------+--------------------------------------------------------+
 |Command appended in file  | yes                     | -            | Der Benutzer muss anfügen                              |
 +--------------------------+-------------------------+--------------+--------------------------------------------------------+
 |Command appended in file  | No                      |              | Vom doc verlassen|                                     |
 +--------------------------+-------------------------+--------------+--------------------------------------------------------+
 


Vorteile
-----------

Wir können von entfernten Ort zu arbeiten. Der Benutzer muss, um das System für die Pfad anweisen. Auto-Generation möglich ist. Wir können die Datei angehängt werden, wann immer Sie brauchen. Wir können die Schlüssel ohne Passwort teilen. Nicht Groß- und Kleinschreibung.
