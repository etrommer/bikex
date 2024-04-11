# Was ist das?
Aus diesem Repository wird die BikeX-Seite erstellt. Das passiert mit [Zola](https://www.getzola.org/), einem sog. Static Site Generator. Zola generiert aus eine Textdateien und Vorlagen eine komplette Website.

# Was brauche ich?
Wenn du etwas ändern willst musst du eigentlich nur eine Sache können:
[Markdown](https://www.markdownguide.org/cheat-sheet/)

# Wo muss ich etwas ändern?
## Text
Alle Texte findest du im Ordner `content`. Die Seiten der einzelnen Festivals liegen direkt in `content`, die in der Kopfzeile verlinkten Seiten (Impressum und FAQ) im Unterordner `pages`. Festivalseiten müssen als Erstes diese Informationen enthalten:
```markdown
+++
title = "Name des Festivals"
date = 2024-07-21 # Datum der Anreise
updated = 2024-03-26 # Letzte Änderung an der Seite (muss bei Änderungen manuell angepasst werden)
description = "Beschreibung" # Die Kurzbeschreibung für die Startseite
+++
```
darunter folgt normaler Markdown-Text.

Jede Datei gibt es in zwei Ausführungen:
- `<festivalname>.md`: Die deutsche Version der Beschreibung
- `<festivalname>.en.md`: Die englische Version
Beide Dateien müssen ausgefüllt werden damit die Seite am Ende zweisprachig vorhanden ist.

## Dateien
Fotos, Videos, GPX-Tracks usw. müssen im Ordner `static` hochgeladen werden. Von dort können sie normal via Markdown in den Beschreibungen verlinkt werden. Eine Datei `static/foo/bar/test.gpx` zum Beispiel so:
```markdown
[Linktext](/foo/bar/test.gpx)
```

# Was muss ich sonst noch tun?
Eigentlich nichts. Die Website wird bei Änderungen im Repository automatisch aktualisiert. Das kann eventuell einige Minuten dauern.
