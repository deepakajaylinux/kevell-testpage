=================
Amazon S3 
=================

Zusammenfassung
-----------------

Amazon Simple Storage Service (Amazon S3), bietet Entwicklern und IT-teams mit hoch skalierbare, sichere, dauerhafte Objektspeicherung. Amazon S3 ist einfach zu bedienen, mit eine einfache Web-Services-Schnittstelle zum Speichern und Abrufen von beliebige Datenmengen von überall im Web. Mit Amazon S3 Zahlen Sie nur für die Lagerung, die Sie wirklich nutzen. Es gibt keine Mindestgebühr und keine Setup-Kosten.

Amazon S3 kann allein oder zusammen mit anderen AWS-Diensten wie Amazon Elastic Compute Cloud (Amazon EC2), Amazon Elastic Block Store (Amazon EBS), und Amazon-Gletscher, sowie Lagerung Drittanbieterpaketdepots und Gateways verwendet werden. Amazon S3 bietet kostengünstige Objektspeicherung für eine Vielzahl von Anwendungsfällen einschließlich Cloud-Anwendungen, Content-Verteilung, Backup und Archivierung, Disaster Recovery und große Datenanalyse.

Hilfe Befehl
----------------------

Dieser Befehl hilft, um die Nutzung von AWS S3 zu bestimmen. Der Benutzer wird kommen, über den anderen Weg/Format wissen, dieses Modul ausgeführt. Dieser Befehl führt den Endbenutzer, um diesen Befehl zu erfahren. Unten gegeben sind, den Befehl und den Screenshot von der gleichen.

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSS3 help

 ******************************


    This is an extension provided for Handling AWSS3.

    AWSS3, awss3 aws-s3

        - ensure-bucket-exists
        Lets you add bucket to AWSS3 if doesnt exists
        example: ptconfigure AWSS3 ensure-bucket-exists
                    --yes
                    --guess
        - add-object
        Lets you upload object to bucket
        example: ptconfigure AWSS3 add-object
                    --yes
                    --guess


        - remove-bucket
          Lets you remove bucket
          example: ptconfigure AWSS3 remove-bucket
                    --yes
                    --guess

        - remove-object-all
       Lets you remove all object from a bucket
          example: ptconfigure AWSS3 remove-object-all
                    --yes
                    --guess


            - remove-object
       Lets you remove a object from a bucket
          example: ptconfigure AWSS3 remove-object
                    --yes
                    --guess

        - list
        Will display data about your AWS S3
        example: ptconfigure AWSS3 list
                  --yes
                  --guess


        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1


 ------------------------------
 End Help
 ******************************


Ensure-bucket-exists
---------------------------

Dieser Befehl hilft AWSS3 wenn Eimer hinzu existiert nicht. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash

	ptconfigure AWSRoute53 create-hosted-zone --yes --guess

Add-object 
---------------------------

Dieser Befehl hilft, Objekt, um Eimer hochladen. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash
	
	ptconfigure AWSS3 add-object --yes –guess

Remove-bucket 
---------------------------

Dieser Befehl hilft, um Eimer zu entfernen. Die unten mit dem Befehl führt den Prozess.
 
.. code-block:: bash     

	ptconfigure AWSS3 remove-bucket --yes --guess

Remove-object-all
--------------------------

Dieser Befehl hilft, um alle Objekte aus einem Eimer zu entfernen. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash     
	
	ptconfigure AWSS3 remove-object-all --yes --guess


Remove-object	
--------------------------

Dieser Befehl können Sie ein Objekt aus einem Eimer entfernt. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash     
	
 	ptconfigure AWSS3 remove-object --yes --guess 

List
---------

Dieser Befehl hilft zum Anzeigen von Daten über die AWS-S3. Die unten mit dem Befehl führt den Prozess.

.. code-block:: bash 

	ptconfigure AWSS3 list --yes --guess

Alternative Parameter
----------------------------

Es gibt drei alternative Parameter, die in der Befehlszeile verwendet werden können.

AWSS3, awss3 aws-s3 

Vorteile
--------------

Langlebig: Amazon S3 bietet dauerhafte Infrastruktur um wichtige Daten zu speichern und richtet sich an Dauerhaftigkeit von 99.999999999 % der Objekte. Ihre Daten werden redundant über mehrere Einrichtungen und mehrere Geräte in jede Einrichtung.

Low-Cost: Amazon S3 können Sie große Datenmengen auf einem sehr niedrigen Preis zu speichern. Sie zahlen für das was Sie, ohne minimale Verpflichtungen oder vorab Gebühren brauchen.

Verfügbar: Amazon S3 ist für 99,99 % Verfügbarkeit der Objekte über ein bestimmtes Jahr entwickelt.  Amazon S3 wird auch unterstützt durch das Amazon S3 Service Level Agreement, sicherzustellen, dass Sie sich darauf verlassen können, wenn Sie es brauchen. Und Sie können eine AWS-Region für Latenz optimieren, Kosten zu minimieren oder regulatorischen Anforderungen.

Zu sichern: Amazon S3 Datenübertragung über SSL und automatische Verschlüsselung Ihrer Daten unterstützt, sobald sie hochgeladen werden. Sie können auch Eimer Richtlinien zum Verwalten von Berechtigungen für Objekte und steuern den Zugriff auf Ihre Daten mit AWS Identity und Access Management (IAM) konfigurieren.

Skalierbar: Mit Amazon S3, können Sie speichern, so viele Daten wie Sie wollen und sie, greifen Wenn Sie es brauchen. Du kannst aufhören raten, Ihre zukünftigen Speicherbedarfs und Skala oben und unten je nach Bedarf, geschäftliche Flexibilität drastisch zu erhöhen.

Event-Benachrichtigungen senden: Amazon S3 können Benachrichtigungen senden, wenn Objekte auf Amazon S3 hochgeladen werden. Amazon S3-Ereignisbenachrichtigungen können mit Amazon SQS oder Amazon SNS zugestellt oder direkt an AWS Lambda, sodass Sie Trigger Workflows, Warnungen oder sonstige Verarbeitung gesendet werden. Amazon S3-Ereignisbenachrichtigungen können Sie z. B. auslösen Transcodierung von Media-Dateien beim Upload sind, Verarbeitung von Datendateien, sobald diese verfügbar sind, oder Synchronisierung von Amazon S3-Objekten mit anderen Datenspeichern.
Hohe Leistung: Amazon S3 unterstützt mehrteilige lädt zur Maximierung der Netzwerkdurchsatz und Ausfallsicherheit und ermöglicht Ihnen, wählen Sie die AWS-Region zu speichern Ihre Daten in der Nähe der Endbenutzer und minimieren Netzwerklatenz. Und Amazon S3 ist mit Amazon CloudFront, ein Content-Delivery-Webdienst, der Inhalt an Endbenutzer mit geringer Latenz, hohe Geschwindigkeit der Datenübertragung und keine minimale Nutzung Verpflichtungen vertreibt integriert.

Integriert: Amazon S3 ist integriert mit anderen AWS-Diensten zu vereinfachen, hoch- und Herunterladen von Daten von Amazon S3 und erleichtern das Erstellen von Lösungen, die eine Reihe von AWS-Dienste verwenden. Amazon S3-Integrationen sind Amazon CloudFront Amazon Kinesis, Amazon RDS, Amazon-Gletscher, Amazon EBS, Amazon DynamoDB, Amazon Redshift, Amazon Route 53, Amazon EMR und AWS Lambda.
Einfach zu bedienen: Amazon S3 ist einfach zu bedienen mit einer webbasierten Management-Konsole und mobile app und vollen REST APIs und SDKs für die einfache Integration mit Drittanbieter-Technologien.

