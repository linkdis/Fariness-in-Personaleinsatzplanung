# Fariness-in-Personaleinsatzplanung
Code zu meiner Bachelorarbeit für Kapitel 4. 


# Schichtplanungsoptimierung mit PuLP

## Anforderungen

Bevor du den Code ausführst, stelle sicher, dass du die erforderlichen Abhängigkeiten installiert hast.
Das Skript verwendet die Bibliotheken `pulp` für lineare Optimierung und `numpy` für statistische Berechnungen.

### Installation der Abhängigkeiten

Öffne eine Konsole oder ein Terminal und installiere die benötigten Pakete mit folgendem Befehl:

```sh
pip install pulp numpy
```

Falls du `conda` verwendest, kannst du alternativ diesen Befehl nutzen:

```sh
conda install -c conda-forge pulp numpy
```

## Code ausführen

Sobald die Abhängigkeiten installiert sind, kann das Skript direkt ausgeführt werden. Dazu:

1. Speichere das Python-Skript in einer Datei, z. B. `schichtplanung.py`.
2. Öffne ein Terminal oder eine Eingabeaufforderung in dem Verzeichnis, in dem sich die Datei befindet.
3. Führe den Code mit folgendem Befehl aus:

```sh
python schichtplanung.py
```

## Funktionsweise

Das Skript löst ein Schichtplanungsproblem unter Berücksichtigung folgender Bedingungen:

- Jeder Mitarbeiter kann pro Tag nur eine Schicht arbeiten.
- Jede Schicht benötigt genau drei Mitarbeiter.
- Zwischen zwei Schichten gibt es eine Mindestruhezeit.
- Es gibt eine Begrenzung der maximalen Arbeitstage in Folge.
- Mitarbeiterpräferenzen werden gewichtet und in der Zielfunktion berücksichtigt.

Nach der Optimierung gibt das Skript die folgenden Ergebnisse aus:

- Eine optimale Schichtzuweisung für alle Tage und Mitarbeiter.
- Die Anzahl der Nachtschichten, Wochenendschichten und Gesamtschichten pro Mitarbeiter.
- Verletzungen von Präferenzwünschen.

## Fehlerbehebung

Falls ein `ModuleNotFoundError` für `pulp` oder `numpy` auftritt, stelle sicher, dass die Pakete korrekt installiert wurden.

Falls das Problem weiterhin besteht, überprüfe, ob du das richtige Python-Environment verwendest:

```sh
python -m pip install pulp numpy
```


