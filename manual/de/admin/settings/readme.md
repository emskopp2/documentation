# Settings

## Grundeinstellungen im Backend

Nach der Installation sollten zuerst einige Grundeinstellungen vorgenommen werden.

Zu finden unter:

→ System → Einstellungen → Dokumenten Management System


### Basisverzeichnis: 
Wo sollen die Dokumente abgelegt werden? Standard und empfohlen ist: tl_files/dms

### Maximale Upload Größe: 
Wie groß dürfen die Dateien sein die hochgeladen werden? 
Diese Größe darf die PHP Einstellung für upload_max_filesize nicht überschreiten.


### Dokumente standardmäßig veröffentlichen:
Ist diese Option aktiviert wird die Checkbox zum Veröffentlichen im Verwaltungsmodul (Frontend) immer angekreuzt.

## Dokumentenablage aufbauen

Bevor man mit dem eigentlichen Aufbau der Dokumentenablage beginnt indem man Dateitypen-Sets erstellt, Kategorien anlegt und Zugriffsrechte zuweist, sollten schon Mitgliedergruppen in der Benutzerverwaltung von Contao angelegt sein oder legt diese nun an dieser Stelle an. 

Dies kann zwar auch zu einem späteren Zeitpunkt erfolgen allerdings macht das Vorhandensein von Mitgliedergruppen die nächsten Arbeitsschritte effizienter. 



### Dateityp-Sets erstellen
Dateitypen-Sets erleichtern die Zuweisung erlaubter Dateitypen die in eine Kategorie abgelegt werden dürfen erheblich.

Im Modul DMS → Dateityp-Sets → dann auf „Neues Dateityp-Set“

Name: Aussagekräftigen Namen vergeben (z.B. PDF Dokumente)
Beschreibung: optionale Angabe einer Beschreibung
Erlaubte Dateitypen: pdf (Gross oder Kleinschreibung spielt keine Rolle)
Dateityp-Set veröffentlichen: Checkbox aktivieren

Speichern nicht vergessen ;-)

Jetzt hat man ein Dateityp-Set vom Typ pdf angelegt.

Auf diese Weise können beliebig viele Sets angelegt werden.

Sollen mehrere Dateitypen in einem Set enthalten sein, werden diese im Feld „Erlaubte Dateitypen“ durch Komma getrennt eingetragen. Z.B. doc, docx oder jpg, gif, tif
