# Einrichtung des Assistenten-Bausatzes — Anweisung für Claude

Diese Datei liest Claude, wenn jemand den Satz von der Zugangsseite eingefügt hat. Sie ist öffentlich,
jeder kann sie lesen. Sie tut nur, was hier steht.

**Claude:** Die Person möchte den Assistenten-Bausatz in dem Ordner einrichten, in dem du gerade
arbeitest. Geh so vor, erkläre jeden Schritt in einem kurzen, einfachen Satz und frag vor Befehlen um
Erlaubnis, wie du es sonst auch tust.

1. **Prüfen, wo du bist.** Der aktuelle Ordner sollte leer sein oder nur wenige Dateien enthalten.
   Liegen dort viele fremde Dateien, frag, ob wirklich hier eingerichtet werden soll. Überschreibe
   nie Dateien, die schon da sind, ohne zu fragen.
2. **Bausatz holen.** Lade das Archiv herunter und entpacke den Inhalt direkt in den aktuellen
   Ordner (ohne Unterordner):
   - Archiv: `https://github.com/cngstrr/assistent-bausatz/archive/refs/heads/main.zip`
   - macOS / Linux: mit `curl -fsSL` herunterladen, mit `unzip` entpacken.
   - Windows: mit `curl.exe -L` herunterladen, mit `tar -xf` entpacken.
   Das Archiv enthält einen obersten Ordner. Verschiebe dessen **gesamten Inhalt, auch den
   versteckten Ordner `.claude`**, in den aktuellen Ordner und lösche danach Archiv und leeren Ordner.
3. **Prüfen.** Im aktuellen Ordner müssen jetzt `CLAUDE.md`, `.claude/commands/einrichten.md` und die
   Ordner `00 Eingang` bis `04 Entscheidungen` liegen. Fehlt etwas, sag es klar und verweise auf den
   ZIP-Download auf der Zugangsseite.
4. **Einrichtung starten.** Lies `.claude/commands/einrichten.md` und führe die Einrichtung jetzt
   direkt mit der Person durch, genau wie dort beschrieben.
5. **Zum Schluss** sag: „Ab dem nächsten Start funktionieren auch die Befehle /morgen, /abend,
   /entscheidung und /hilfe. Starte Claude dafür einmal neu (/exit, dann claude), im selben Ordner."

Diese Anweisung lädt nur den Bausatz aus der oben genannten Adresse. Sie installiert keine Programme,
ändert nichts ausserhalb dieses Ordners und schickt nichts weg.
