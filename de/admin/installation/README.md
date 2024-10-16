# Installation

Hier erhalten sie Informationen über die Installation.

**Seiteninhalt**
<!-- toc -->

1. [Installation per Composer](#installation-per-composer)
2. [Serverkonfiguration](#serverkonfiguration)
3. [Installation per Contao-Manager](#installation-per-contao-manager)

**Für die manuelle Installation**, können die benötigten Dateien hier heruntergeladen werden: https://github.com/ContaoDMS

Nach der Installation stehen die Werkzeuge des Contao-DMS im Backend zur Verfügung: 
 
![Contao-DMS Backend Werkzeuge](4-dms-backend-tools.png)

* (Dateityp-Sets) *ist ein extra Add-On und muss separat installiert werden*


## Installation per Composer

Für die Installation per Composer sind alle Pakete unter https://packagist.org/packages/contao-dms/ zu finden. Für die Suche im Contao Backend reicht es `contao-dms/` einzugeben. Dann werden alle zur Verfügung stehen Pakte angezeigt.
Das Paket https://packagist.org/packages/contao-dms/bundle-all enthält das ContaoDMS sowie auch das Dateityp-Sets Add-On.


## Serverkonfiguration

Unter Umständen muss man eine eigene `php.ini` ins Web-ROOT der Installation legen um z.B. Arbeitsspeicher Limits oder Ausführungszeiten zu definieren. Sind diese zur gering kann es vorkommen, dass größere Dateien nicht hochgeladen werden können.

Ein Beispiel für den Inhalt einer solchen `php.ini` Datei sieht wie folgt aus:

    # increase memory limits and execution time
    upload_max_filesize = 5M
    memory_limit = 512M
    max_execution_time = 50000
    post_max_size = 40M

## Installation per Contao-Manager

1. Contao-Manager aufrufen (z.B. meine-Domain.de/contao-manager.phar.php)
2. Login Contao-Manager 
3. nach Durchlauf der Systemüberprüfung weiter zum **Contao-Manager**
4. In der Suche nach **Contao DMS** suchen.
5. Es werden alle zur Verfügung stehenden Pakete angezeigt:

![ContaoDMS Pakete suchen](5-paket-hinzufuegen.png)

6. Das Paket **ContaoDMS Bundle all** enthält das ContaoDMS sowie auch das Dateityp-Sets Add-On.
7. mit **Hinzufügen** das Paket zur Installation bereitstellen
8. anschließend im Menü den Punkt **Pakete** wählen:

![Pakete aufrufen](6-pakete-aufrufen.png)

9. und jetzt auf **Änderungen anwenden**:

![Änderungen anwenden](7-aenderungen-anwenden.png)

10. Die Pakete werden aktualisiert:

![Pakete werden aktualisiert](8-pakete-werden-aktualisiert.png)

11. weiter zu **Datenbank aktualisieren**:

![Weiter zu Datenbank aktualisieren](9-zu-db-aktualisieren.png)

12. Weiterleitung zum Contao Installtool
12. Login
13. nun die Datenbank aktualisieren:

![Datenbank im Installtool aktualisieren](11-db-aktualisieren.png)

14. anschließend zum Backend (Login)
15. Im Backend sind nun die ContaoDMS Werkzeuge zu sehen:

![ContaoDMS im Backend](12-dms-rubriken-im-backend.png)
