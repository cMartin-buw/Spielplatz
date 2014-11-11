---
output: html_document
---
Spielplatz
==========

## Sandkasten

**Dies ist ein Sandkasten zum Testen und Kennenlernen der GID-Funktionalitäten.**

Zunächst habe ich in RStudio einige Formatierungen hinzugefügt, um zu testen, ob diese beim knittern richtig dargestellt werden.

Im nächsten Schritt werde ich versuchen die geänderte Version auf github hochzuladen.

*Offenbar muss dem push ein commit vorhergehen*

Ich teste nun noch einmal den Vorgang mit commit.

Die Vorgehensweise ist also:
* Änderungen vornehmen
* Version speichern
* im GH-Menü (oben links) - *Version control*
  + commit (oder *Strg + Alt + m*)
  + Kommentar einfügen und commit ausführen
  + **Beachten: es muss ein Haken an der .md-Datei gesetzt sein**
  + Push ausführen
* Browser-Refresh des Github-Fensters, um die Änderung darzustellen
 
beim Einfügen von Anführungszeichen und dem Benutzten der *Amend previous commit* - Checkbox traten Fehler auf. Ich teste nun, welcher der beiden Faktoren diesen verursacht hat.

Zunächst verwende ich "Anführungszeichen" ohne Amend-Checkbox.

Die Anführungszeichen verursachen keinen Fehler und werden in github dargestellt.
Also werde ich die "Amend"-Option benutzen.

Hierbei tritt der Fehler wieder auf:
*To git@github.com:cMartin-buw/Spielplatz.git
 ! [rejected]        master -> master (non-fast-forward)
error: Fehler beim Versenden einiger Referenzen nach 'git@github.com:cMartin-buw/Spielplatz.git'
Hinweis: Aktualisierungen wurden zurückgewiesen, weil die Spitze Ihres aktuellen
Hinweis: Branches hinter seinem externen Gegenstück zurückgefallen ist. Führen Sie
Hinweis: die externen Änderungen zusammen (z.B. 'git pull ...') bevor Sie "push"
Hinweis: erneut ausführen.
Hinweis: Siehe auch die Sektion 'Note about fast-forwards' in 'git push --help'
Hinweis: für weitere Details.*
Offenbar erzeugt "Amend" einen Versionskonflikt.
