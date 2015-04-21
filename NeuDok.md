### Sandkasten - die Testdokumentation

**Dies ist eine neu erstellte Datei, die manuell (im Editor) editiert wurde.**


Snipletts aus Aufsätze


Datei schreiben (Semikolon-separiert):

setwd("/home/xy/Dokumente/yz")

write.csv2(ortbbmerge, file="einleitung.csv")



Bearbeiten von Tabellen

Variante 1: 0 und 1 werden ersetzt, mit "labels"

ortbb11$Konsens <- factor(ortbb11$Konsens, labels = c("Sonstige Ergebnisse", "Konsens"))

Variante 2: es wird eine Spalte angefügt, die 0 und 1 übersetzt, mit "recode"

ortbb11$Konsens.text <- recode(ortbb11$Konsens, recodes = '1 = "Konsens"; 0 = "Sonstige Ergebnisse"')
