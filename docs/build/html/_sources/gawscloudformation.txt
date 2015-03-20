==================
AWSCloudFormation
==================

Zusammenfassung
-------------------

AWS CloudFormation bietet Entwicklern und Systemadministratoren eine einfache Möglichkeit zum Erstellen und Verwalten einer Auflistung von verwandten AWS-Ressourcen bereitstellen und aktualisieren sie auf eine geordnete und vorhersagbare Weise.


AWS CloudFormation Beispielvorlagen verwenden können oder erstellen Sie eigene Vorlagen um die AWS-Ressourcen und damit verbundenen Abhängigkeiten oder Laufzeitparameter, benötigt zum Ausführen der Anwendung zu beschreiben. Du musst herausfinden, den Auftrag zur Bereitstellung von AWS-Dienste oder die Feinheiten machen diese Abhängigkeiten zu arbeiten. CloudFormation übernimmt dies für Sie. Nachdem die AWS-Ressourcen bereitgestellt werden, können Sie ändern und aktualisieren Sie sie in einer kontrollierten und vorhersehbaren Weise wirksam anwenden Versionskontrolle in der AWS-Infrastruktur die gleiche Weise, die Sie mit Ihrer Software zu tun.


Sie können bereitstellen und Aktualisieren einer Vorlage mit seiner zugeordneten Sammlung von Ressourcen (genannt einen Stapel) mithilfe der AWS Management Console, AWS Command Line Interface oder APIs. CloudFormation ist ohne zusätzliche Kosten verfügbar, und Sie zahlen nur für die AWS-Ressourcen benötigt zum Ausführen Ihrer Anwendungen.



Hilfe Befehl
----------------------

Dieser Befehl hilft, die Nutzung von AWS CloudFormation bestimmen. Der Benutzer wird kommen, über den anderen Weg/Format wissen, dieses Modul ausgeführt. Dieser Befehl führt den Endbenutzer, um diesen Befehl zu erfahren. Unten gegeben sind, den Befehl und den Screenshot von der gleichen.


.. code-block:: bash

 kevell@corp:/# ptconfigure AWSCloudFormation help

 ******************************


  This command allows you to install a The AWS Cloud Formation Command
  Line Tools. This tool is provided by

  AWSCloudFormation, aws-cloud-formation, aws-cloudformation

        - install
        Installs AWSCloudFormation. Note, you'll also need Java installed
        as it is a prerequisite for AWSCloudFormation.
        example: ptconfigure aws-cloud-formation install

 ------------------------------
 End Help
 ******************************

Installation
----------------

Falls der Benutzer durchführen, AWSCloudFormation Modul in der Maschine muss, die unten mit dem Befehl wird ausgeführt, den Prozess der Installation.


.. code-block:: bash
        
       ptconfigure aws-cloud-formation install

.. code-block:: bash 

 kevell@corp:/# ptconfigure aws-cloud-formation install

 Install AWSCloudFormation? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         AWS CloudFn!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-17956189939.sh
 chmod 755 /tmp/ptconfigure-temp-script-17956189939.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-17956189939.sh Permissions
 Executing /tmp/ptconfigure-temp-script-17956189939.sh
 Cloning into 'aws-cloudformation'...
 remote: Counting objects: 64, done.
 remote: Total 64 (delta 0), reused 0 (delta 0), pack-reused 64
 Unpacking objects: 100% (64/64), done.
 Checking connectivity... done.
 mv: cannot move ‘/tmp/aws-cloudformation/bin’ to ‘/opt/aws-cloudformation/bin’: Directory not empty
 mv: cannot move ‘/tmp/aws-cloudformation/lib’ to ‘/opt/aws-cloudformation/lib’: Directory not empty
 Temp File /tmp/ptconfigure-temp-script-17956189939.sh Removed
 PHP Notice:  Undefined index: object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: method in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: params in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Warning:  call_user_func_array() expects parameter 1 to be a valid callback, first array member is not a valid class name or object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: method in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: params in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Warning:  call_user_func_array() expects parameter 1 to be a valid callback, first array member is not a valid class name or object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 AWSCloudFormation: Success
 ------------------------------
 Installer Finished
 ******************************


Alternative Parameter
-----------------------------

Es gibt drei alternative Parameter, die in der Befehlszeile verwendet werden können.


AWSCloudFormation, aws-cloud-formation, aws-cloudformation 


Vorteile
--------------

Unterstützt eine breite Palette von AWS Ressourcen: AWS CloudFormation unterstützt eine breite Palette von AWS-Ressourcen, sodass Sie baut eine hochverfügbare, zuverlässige und skalierbare AWS-Infrastruktur für Ihre Anwendungsanforderungen. AWS CloudFormation unterstützt derzeit Ressourcen in den folgenden AWS-Diensten:


Auto Scaling

Amazon CloudFront

AWS CloudWatch

Amazon DynamoDB

Amazon EC2

Amazon ElastiCache

AWS Elastic Beanstalk

AWS Elastic Load Balancing

AWS Identity and Access Management

Amazon RDS

Amazon Redshift

Amazon Route 53

Amazon S3

Amazon SimpleDB

Amazon SNS

Amazon SQS

Amazon VPC

Einfach zu bedienen: CloudFormation erleichtert das organisieren und Bereitstellen einer Sammlung von AWS-Ressourcen und können Sie beschreiben, etwaige Abhängigkeiten oder spezielle Parameter zur Laufzeit übergeben. Sie können eine der vielen CloudFormation Beispielvorlagen--entweder wörtlich oder als Ausgangspunkt verwenden.


Das Rad muss nicht neu erfunden: eine Vorlage kann immer wieder verwendet werden, um identische Kopien von demselben Stapel erstellen (oder als Grundlage zu verwenden, um einen neuen Stapel zu starten). Sie können aufgezeichnet und Steuerung von regionsspezifischen Infrastruktur Variationen wie Amazon EC2 AMIs sowie Amazon Elastic Block Store (EBS) und Amazon RDS-Snapshot-Namen.


Transparent und offen: Vorlagen sind einfache JSON-formatierte Textdateien, die Ihre normale Quelle Kontrollmechanismen unterstellt, in privaten oder öffentlichen Orten wie Amazon S3 gespeichert und per e-Mail ausgetauscht werden können. Mit AWS CloudFormation, Sie können "öffnen die Motorhaube," um zu sehen welche AWS-Ressourcen genau einen Stapel bilden. Sie behalten die volle Kontrolle und haben die Möglichkeit, die AWS-Ressourcen als Teil eines Stapels erstellt ändern.


Deklarative und flexibel: Erstellen die Infrastruktur soll Sie auflisten, welche AWS-Ressourcen, die Konfigurationswerte, und Verbindungen, die Sie in einer Vorlage benötigen und lassen Sie die AWS CloudFormation erledigt den Rest mit ein paar einfachen Klicks in der AWS Management Console einen Befehl mithilfe der Befehlszeilenschnittstelle AWS oder ein einzelnes fordert durch Aufrufen der APIs. Du musst nicht die Informationen über das Erstellen und verbinden die jeweiligen AWS-Ressourcen über ihre Service-APIs zu erinnern; AWS CloudFormation tut dies für Sie. Du musst auch eine Vorlage von Grund auf neu zu schreiben, wenn Sie mit einer der zahlreichen Beispielvorlagen, die mit AWS CloudFormation kommen.


Über Parameter angepasst: Sie können Parameter verwenden, um Aspekte der Vorlage zur Laufzeit anpassen als Stapel gebaut ist. Beispielsweise können Sie übergeben die RDS Datenbankgröße, EC2 Instanz Typen, Datenbank und Web-Server-Port-Nummern zu AWS CloudFormation beim Erstellen eines Stapels. Eine parametrisierte Vorlage können Sie auch um mehrere Stapel zu erstellen, die auf kontrollierte Weise abweichen können. Beispielsweise können Ihre Amazon EC2-Instanz-Typen, Amazon CloudWatch Alarmgrenzen und Amazon RDS lesen-Replica Einstellungen unter AWS Regionen abweichen, erhalten Sie mehr Kunden-Traffic in den USA als in Europa. Sie können Vorlagenparameter verwenden, um die Einstellungen zu optimieren und Schwellen in den einzelnen Regionen getrennt und immer noch sicher sein, dass die Anwendung konsequent in den Regionen bereitgestellt wird.


Integration bereit: AWS CloudFormation können Sie mit der Entwicklung und Management-Tools Ihrer Wahl integrieren.


AWS CloudFormation veröffentlicht Progress-Ereignisse durch Amazon Simple Notification Service (SNS). Mit SNS können Stapel erstellen und Löschen von Fortschritt per e-Mail und mit anderen Prozessen programmgesteuert zu integrieren.


Keine Extra-Gebühr: AWS CloudFormation steht ohne Aufpreis zur Verfügung. Sie werden nur die normalen Tarife für die AWS-Ressourcen, die AWS CloudFormation erstellt und die Anwendung in Rechnung gestellt.


