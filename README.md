# VLKS-Innenanzeige

**Derzeit noch WIP! Script nicht voll funktionsfähig.**

Dies ist eine fiktive TFT-Innenanzeige für die VLKS Landkreis Stein. Das Vorbild ist der Innenmonitor der VKP im Kreis Plön.

## Aktueller Stand
Die Innenanzeige kann bereits eingebaut werden. Texturen, Model und Textfelder sind bereits fertig bzw. korrekt konfiguriert. Das Script ist bisher unvollständig. Es kann lediglich booten.

## Installation/Einbau
Die Innenanzeige kann wiefolgt in einen Bus eingebaut werden:

1. Alle Dateien (model, script, texture) in den jeweiligen Bus-Ordner einfügen
2. Model-Eintrag in der Model.cfg einfügen (siehe Datei "Modeleintrag.cfg") - die Texttextur-Indizes müssen natürlich angepasst werden. :)
3. Scripte in die Bus-Datei einfügen:
    - "script\VLKS_Innenanzeige\varlist.txt" unter [varnamelist]
    - "script\VLKS_Innenanzeige\stringvarlist.txt" unter [stringvarnamelist]
    - "script\VLKS_Innenanzeige\script.txt" unter [script]
    - "script\VLKS_Innenanzeige\constfile.txt" unter [constfile]
4. Folgende Macroaufrufe in der main.osc des Busses einfügen:
    - (M.L.VLKS_Innenanzeige_init) im {init}-Bereich
    - (M.L.VLKS_Innenanzeige_frame) im {frame}-Bereich
