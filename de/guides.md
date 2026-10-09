---
lang: de
ref: guides
layout: page
title: Benutzerhandbuch
description: >
  Schritt-für-Schritt-Anleitungen, um ein ScoreBoard-Overlay in OBS, Streamlabs, Wirecast
  oder Meld einzurichten: Text-Timer, Scoreboard-Hintergrund, Zehntelsekunden-Timer und Teamaufstellungen.
image: /img/scoreboard_for_mac_light.png
permalink: /de/guides/
---

Anleitungen, um ein Scoreboard in OBS hinzuzufügen – dieselben TXT- und Bilddateiquellen funktionieren genauso in Streamlabs, Wirecast und Meld.

_Die Bezeichnungen in OBS sind für die deutsche Oberfläche angegeben, in Klammern für die englische._

- [Häufige Fragen](#faq)
- [Erste Schritte](#getting-started)
- [Ausgegebene Text- und Bilddateien](#output-text-and-image-files)
- [Timer/Zähler in OBS hinzufügen](#how-to-add-a-text-timer-or-counter-in-obs)
- [Scoreboard-Hintergrund hinzufügen](#how-to-add-a-scorebug-background-image-in-obs)
- [Zehntelsekunden richtig anzeigen](#how-to-display-tenths-of-a-second-in-obs)
- [Teamaufstellungen anzeigen](#how-to-show-team-rosters-in-an-obs-broadcast)

---

## Häufige Fragen {#faq}

**Wie füge ich auf dem Mac ein Live-Sportscoreboard zu OBS hinzu?**  
Installiere ScoreBoard für Mac und füge dann die ausgegebenen TXT-Dateien in OBS als Quellen vom Typ *Text (FreeType 2)* und die Promo-/Logobilder als Quellen vom Typ *Bild* hinzu – siehe [Erste Schritte](#getting-started) unten.

**Warum aktualisiert sich meine Textquelle in OBS nicht sofort?**  
Standardmäßig liest OBS Textdateien etwa einmal pro Sekunde neu ein. Für schnellere Aktualisierungen (z. B. Zehntelsekunden auf einem Timer) verwende das Plugin Advanced Scene Switcher – siehe [Zehntelsekunden anzeigen](#how-to-display-tenths-of-a-second-in-obs).

**Kann ich Teamaufstellungen im Stream zeigen?**  
Ja – trage die Aufstellung als Text in das Statusfeld eines Teams ein und/oder füge sie als Bild über die Promo-Schaltflächen hinzu, und zeige sie dann mit Text- und Bildquellen in OBS an – siehe [Teamaufstellungen anzeigen](#how-to-show-team-rosters-in-an-obs-broadcast).

**Funktioniert das auch in Streamlabs, Wirecast oder Meld statt OBS?**  
Ja. ScoreBoard gibt einfache TXT- und Bilddateien aus, die jede Streaming-Software mit Text- oder Bilddateiquellen genauso lesen kann wie OBS.

**Brauche ich ein Hintergrundbild für das Scoreboard oder reichen Textquellen?**  
Beides geht. Textquellen allein zeigen die Live-Werte; ein Hintergrundbild dahinter (siehe [Scoreboard-Hintergrund hinzufügen](#how-to-add-a-scorebug-background-image-in-obs)) sorgt für ein gestaltetes Erscheinungsbild.

---

## Erste Schritte {#getting-started}

**Scoreboard für OBS unter macOS** ist eine benutzerfreundliche App für Sportbegeisterte, Kommentatoren und Streamer, die Live-Spielstände von zwei Teams oder Spielern in ihren OBS-Studio-Szenen anzeigen möchten. Die schlanke App vereinfacht die Verwaltung und Einbindung eines Scoreboards, damit du dich auf das Spiel und dein Publikum konzentrieren kannst.

**Mach deine Sportübertragungen besser mit Scoreboard für OBS unter macOS – einfach, effektiv und für Livestreams gemacht!**

## Ideale Einsatzbereiche {#ideal-use-cases}

- Sportveranstaltungen (Fußball, Basketball, Volleyball usw.)  
- E-Sport- und Gaming-Turniere  
- Live-Kommentar- und Analyse-Streams  

## Funktionen {#features}

- **Live-Aktualisierung des Spielstands:** Ändere den Spielstand ganz einfach in Echtzeit während eines Spiels.  
- **Einbindung über Textdateien:** Die App erstellt und aktualisiert automatisch `.txt`-Dateien mit den Scoreboard-Daten, kompatibel mit der OBS-Studio-Quelle *Text (FreeType 2)*.  
- **Geringer Ressourcenbedarf:** Die App ist für macOS optimiert und läuft auch auf leistungsschwachen Systemen flüssig.  
- **Intuitive Oberfläche:** Einfache, übersichtliche Oberfläche zur Verwaltung von Teams, Spielständen und weiteren Spieldetails.
- **Anpassbares Layout:** Passe das Aussehen des Scoreboards an den Stil deines Streams an, einschließlich Schriftgröße, Farbe und Position. Das geschieht im Streaming-Programm, zum Beispiel in OBS.  

## So funktioniert es {#how-it-works}

1. **App einrichten**  
   - Installiere ScoreBoard für Mac auf deinem Computer:  
      - [Im Mac App Store kaufen](https://apps.apple.com/app/id1579159150)  
      - [Kostenlose Version herunterladen](/free-apps/ScoreBoard-free.zip) und entpacken – von Apple notarisiert und sicher  
   - Öffne die App und gib die Namen der Teams/Spieler sowie weitere Grundeinstellungen ein.  

2. **Spielstand in Echtzeit aktualisieren**  
   - Ändere den Spielstand mit den übersichtlichen Bedienelementen der App.  
   - Die App speichert die aktualisierten Werte automatisch in `.txt`-Dateien. Standardordner: `Downloads/ScoreBoard Outputs`.

3. **Mit OBS Studio verbinden**  
   - Erstelle in OBS eine neue Quelle *Text (FreeType 2)* oder ziehe die gewünschte Textdatei einfach in das OBS-Fenster.  
   - Aktiviere die Option „Aus Datei lesen“ (*Read from File*) und wähle die von der App erstellte `.txt`-Datei aus.  
   - Passe die Textquelle in OBS an: Position, Größe, Schrift, Farbe usw.  

4. **Streamen oder aufnehmen**  
   - Wenn du den Spielstand in ScoreBoard änderst, erscheinen die Änderungen sofort in OBS. OBS liest die Dateien automatisch von der Festplatte (etwa einmal pro Sekunde) und zeigt das Ergebnis an.  

---

## Ausgegebene Text- und Bilddateien {#output-text-and-image-files}

Standardmäßig schreibt ScoreBoard diese Dateien in den Ordner `Downloads/ScoreBoard Outputs` (einen anderen Ordner kannst du in den Einstellungen wählen). Jede `.txt`-Datei wird live aktualisiert, während du das Spiel steuerst, und wird in OBS als Quelle **Text (FreeType 2)** hinzugefügt; jede `.png`-Datei als Quelle **Bild** – siehe [Erste Schritte](#getting-started) oben.

### Textdateien {#text-files}

| Datei | Inhalt | Beispiel |
|---|---|---|
| `Timer.txt` | Haupt-Spieluhr/Stoppuhr | `12:45` |
| `Timer_Extra.txt` | Zusätzlicher Timer mit zwei Voreinstellungen (z. B. Wurfuhr) | `14` |
| `Home_Name.txt` / `Away_Name.txt` | Teamnamen | `Eagles` |
| `Match_Name.txt` | Name des Spiels/Events | `Semifinal` |
| `Period.txt` | Aktueller Spielabschnitt/Viertel/Halbzeit (auch OT, 2OT, 3OT…) | `2nd` |
| `Home_Goal.txt` / `Away_Goal.txt` | Hauptspielstand (Tore/Punkte) jedes Teams | `3` |
| `Home_Shots.txt` / `Away_Shots.txt` | Zusätzlicher Schusszähler jedes Teams | `18` |
| `Home_Points.txt` / `Away_Points.txt` | Zusätzlicher Punktezähler jedes Teams | `2` |
| `Home_Status.txt` / `Away_Status.txt` | Beschreibung/Status des Teams – auch für [Teamaufstellungen](#how-to-show-team-rosters-in-an-obs-broadcast) | `#9 J. Smith` |
| `Match_Status.txt` | Beschreibung/Status des Spiels | `Final` |
| `Home_Penalties_Numbers.txt` / `Away_Penalties_Numbers.txt` | Nummern der Spieler mit laufender Strafe, eine pro Zeile | `12` |
| `Home_Penalties_Timers.txt` / `Away_Penalties_Timers.txt` | Restzeit jeder laufenden Strafe, eine pro Zeile | `1:32` |
| `NHL_Penalties_Title.txt` | Bezeichnung der Über-/Unterzahlsituation für die kürzeste laufende Strafe | `5 ON 4` |
| `NHL_Penalties_Time.txt` | Restzeit der kürzesten laufenden Strafe | `1:32` |

### Bilddateien {#image-files}

| Datei | Inhalt |
|---|---|
| `Home_Logo.png` / `Away_Logo.png` / `Match_Logo.png` | Team-/Spiellogo |
| `Home_Promo.png` / `Away_Promo.png` / `Match_Promo.png` | Promo-Grafik, z. B. ein Bild der Teamaufstellung |
| `Home_Penalty_Card.png` / `Away_Penalty_Card.png` | Grafik der Gelben/Roten Karte |

Nicht jede Datei ist für jede Sportart relevant: Schüsse und Punkte sind unabhängige Zähler, die du passend zu deiner Sportart umbenennen kannst, und die beiden NHL-Strafdateien werden nur aktualisiert, solange eine Strafe läuft.

---

## Text-Timer oder -Zähler in OBS hinzufügen {#how-to-add-a-text-timer-or-counter-in-obs}

![Hinzufügen einer Text-Timer-Quelle in OBS, verknüpft mit einer TXT-Datei von ScoreBoard](/tutorial-img/how_add_text_to_obs.gif)

### 1. OBS Studio öffnen  
Starte OBS Studio auf deinem Computer.

### 2. Neue Szene erstellen (optional)  
Wenn du deine Einrichtung ordnen möchtest, erstelle eine neue Szene:  
- Klicke im Bereich **Szenen** (*Scenes*) auf die Schaltfläche **+**.  
- Gib der Szene einen Namen und speichere sie.

### 3. Textquelle hinzufügen  
- Klicke im Bereich **Quellen** (*Sources*) auf die Schaltfläche **+**.  
- Wähle in der Liste **Text (FreeType 2)**.  
*Oder ziehe die gewünschte Textdatei einfach aus dem Finder in das OBS-Fenster.*

### 4. Textquelle benennen  
- Gib einen aussagekräftigen Namen für die Quelle ein (z. B. `Main Timer`).  
- Klicke auf **OK**, um die Quelle zu erstellen.

### 5. Lesen aus Datei aktivieren  
- Aktiviere im Eigenschaftenfenster der Textquelle das Kontrollkästchen **Aus Datei lesen** (*Read from File*).  
- So wird der Text automatisch aus einer TXT-Datei aktualisiert.

### 6. TXT-Datei auswählen  
- Klicke neben dem Feld für den Dateipfad auf **Durchsuchen** (*Browse*).  
- Navigiere zu deiner lokalen TXT-Datei, wähle sie aus und klicke auf **Öffnen** (*Open*).

### 7. Text auf der Arbeitsfläche platzieren  
- Ziehe das Textfeld im Vorschaubereich an die gewünschte Stelle in deiner Szene.  
- Passe die Größe bei Bedarf an.

### 8. Aussehen anpassen  
- Passe den Textstil über **Schriftart**, **Größe** und **Farbe** (*Font*, *Size*, *Color*) an.  
- Probiere Ausrichtung, Verlauf und Hintergrund aus, damit der Text zu deinem Layout passt.

### 9. Dateiaktualisierung testen  
- Ändere den Wert des Zählers in ScoreBoard, starte zum Beispiel einen Timer.  
- Prüfe, ob die Änderungen sofort in OBS erscheinen.

**Füge auf die gleiche Weise alle Timer/Zähler hinzu, die du für deinen Sportstream brauchst.**

---

## Scoreboard-Hintergrundbild in OBS hinzufügen {#how-to-add-a-scorebug-background-image-in-obs}

![Hinzufügen einer Bildquelle als Scoreboard-Hintergrund in OBS](/tutorial-img/how_add_scoreboard_background_to_obs.gif)

### 1. Bildquelle hinzufügen  
- Klicke im Bereich **Quellen** (*Sources*) auf die Schaltfläche **+**.  
- Wähle in der Liste **Bild** (*Image*).  
*Oder ziehe die gewünschte Bilddatei einfach aus dem Finder in das OBS-Fenster.*

### 2. Bildquelle benennen  
- Gib einen aussagekräftigen Namen für die Quelle ein (z. B. `Background`) und klicke auf **OK**.  

### 3. Bilddatei auswählen  
- Klicke neben dem Feld für den Dateipfad auf **Durchsuchen** (*Browse*).  
- Navigiere zu deiner lokalen Bilddatei, wähle sie aus und klicke auf **Öffnen** (*Open*).
- Klicke dann auf **OK**, um die Quelle zu speichern.

### 4. Bild unter den Textebenen platzieren  
- Ziehe das Bild im Vorschaubereich an die gewünschte Stelle in deiner Szene.  
- Passe die Größe bei Bedarf an.
- Verschiebe den Hintergrund in der Quellenliste ganz nach unten.

*Beispiel für einen Scoreboard-Hintergrund:*
![Beispielvorlage für den Hintergrund eines Sportscoreboards](/tutorial-img/DefaultScoreBoard.png)

---

## Zehntelsekunden in OBS anzeigen {#how-to-display-tenths-of-a-second-in-obs}

*OBS liest Textdateien standardmäßig etwa einmal pro Sekunde. Damit Zehntelsekunden korrekt angezeigt werden, muss diese Verzögerung verkürzt werden.*

![Timer mit Zehntelsekunden in OBS mithilfe von Advanced Scene Switcher](/tutorial-img/AdvancedSceneSwitcher/Show_tenths_timer.gif)

### 1. Plugin [Advanced Scene Switcher](https://obsproject.com/forum/resources/advanced-scene-switcher.395/) installieren
  
### 2. Plugin öffnen 
- Hauptmenü von OBS – **Werkzeuge** (*Tools*) – **Advanced Scene Switcher**  
- Setze im Tab **General** den Wert **Check conditions every** auf **100ms**

![Tab General in Advanced Scene Switcher mit Prüfintervall 100 ms](/tutorial-img/AdvancedSceneSwitcher/Advanced_Scene_Switcher_General.png)

### 3. Neues Makro hinzufügen  
- Klicke unten links auf die Schaltfläche **+** und benenne das Makro um (z. B. „Timer Delay“)  
- Deaktiviere **Perform actions only on condition change**  

### 4. Neue Bedingung hinzufügen  
- Klicke im Bereich der Bedingungen auf die Schaltfläche **+**  
- Wähle **If**  
- Wähle **File**  
- Klicke auf **Browse**  
- Wähle die Datei „Timer.txt“ (oder eine andere) aus dem Ausgabeordner von ScoreBoard  
- Setze die Bedingung auf **content changed**  

### 5. Neue Aktion hinzufügen  
- Klicke im Bereich der Aktionen auf die Schaltfläche **+**  
- Wähle **Source**  
- Wähle **Set Settings**  
- Wähle deine FreeType-2-Quelle (z. B. „Main Timer“)  
- Setze **Text(Text)**  
- Wähle **Set to macro property**  
- Wähle **File content**

![Bedingung und Aktion eines Advanced-Scene-Switcher-Makros zum Aktualisieren der OBS-Textquelle](/tutorial-img/AdvancedSceneSwitcher/Advanced_Scene_Switcher_Macro.png)

### 6. Texteingabemodus der Timer-Quelle ändern  
- Doppelklicke in OBS in der Quellenliste auf deine FreeType-2-Quelle (z. B. „Main Timer“)  
- Stelle den Texteingabemodus (*Text input mode*) auf manuell (*Manual*)  
- Gib einen beliebigen Platzhaltertext (z. B. ein Leerzeichen) in das Feld **Text** ein  
- Klicke auf **OK**

![Eigenschaften einer FreeType-2-Textquelle in OBS mit manuellem Texteingabemodus](/tutorial-img/AdvancedSceneSwitcher/OBS_Property_FreeType2_manual.png) 

### 7. Haupttimer in ScoreBoard starten und testen  
- Wähle in den Einstellungen von ScoreBoard einen Stil für den Haupttimer (z. B. [:5.3] oder [5.3])
- Stelle den Timer in ScoreBoard zum Testen auf 1 Minute (1:00)
- Starte den Timer und prüfe das Ergebnis in OBS

---

## Teamaufstellungen in einer OBS-Übertragung zeigen {#how-to-show-team-rosters-in-an-obs-broadcast}
![Teamaufstellung neben einem ScoreBoard-Scoreboard in OBS](/tutorial-img/RostersScoreBoard.png)

### Bildquelle {#image-source}
1. Erstelle mit einer beliebigen Software eine Grafikdatei (PDF oder Bild) mit der Teamaufstellung.

2. Füge die Grafikdatei über die Promo-Schaltfläche der Heim- (home promo) oder Gastmannschaft (away promo) in ScoreBoard hinzu und mache sie sichtbar.

3. Füge in OBS eine Bildquelle für die Datei Home_Promo.png oder Away_Promo.png hinzu.

### Textquelle {#text-source}
1. Füge in OBS eine Textquelle für die Dateien Home_Status.txt und Away_Status.txt hinzu.

2. Trage die Aufstellung in ScoreBoard in das Statusfeld (Status) jedes Teams ein. Zum Beispiel:
>#4   Erik Lindqvist  
>#7   Marco Bianchi  
>#9   Connor MacLeod  
>#11  Lukas Weber  
>#13  Tomas Novak  
>#16  Henrik Andersson  
>#19  Diego Fernandez  
>#21  Kai Nakamura  
>#23  Owen Fitzgerald  
>#27  Niklas Berg  
>#29  Marek Kowalski  
>#33  Jesse Virtanen  
>#44  Liam O'Brien  
>#61  Pavel Dvorak  
>#71  Anders Holm  
>#88  Zach Whitfield  
>#91  Miroslav Klimek  

3. Füge ein Hintergrundbild oder eine einfarbige Farbquelle (*Color Source*) hinzu.

4. Fasse Text- und Hintergrundebene in einer Gruppe zusammen, damit du ihre Sichtbarkeit mit einem Klick steuern kannst.

---

Zurück zur [Übersicht von ScoreBoard für Mac](/de/) oder [kostenlose Testversion herunterladen](/free-apps/ScoreBoard-free.zip).

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "inLanguage": "de",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Wie füge ich auf dem Mac ein Live-Sportscoreboard zu OBS hinzu?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Installiere ScoreBoard für Mac und füge dann die ausgegebenen TXT-Dateien in OBS als Quellen vom Typ Text (FreeType 2) und die Promo-/Logobilder als Quellen vom Typ Bild hinzu."
      }
    },
    {
      "@type": "Question",
      "name": "Warum aktualisiert sich meine Textquelle in OBS nicht sofort?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Standardmäßig liest OBS Textdateien etwa einmal pro Sekunde neu ein. Für schnellere Aktualisierungen, etwa Zehntelsekunden auf einem Timer, verwende das Plugin Advanced Scene Switcher: Es verkürzt das Prüfintervall und überträgt den Dateiinhalt in die Textquelle."
      }
    },
    {
      "@type": "Question",
      "name": "Kann ich Teamaufstellungen im Stream zeigen?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Ja. Trage die Aufstellung als Text in das Statusfeld eines Teams ein und/oder füge sie als Bild über die Promo-Schaltflächen in ScoreBoard hinzu, und zeige sie dann mit Text- und Bildquellen in OBS an."
      }
    },
    {
      "@type": "Question",
      "name": "Funktioniert das auch in Streamlabs, Wirecast oder Meld statt OBS?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Ja. ScoreBoard gibt einfache TXT- und Bilddateien aus, die jede Streaming-Software mit Text- oder Bilddateiquellen genauso lesen kann wie OBS."
      }
    },
    {
      "@type": "Question",
      "name": "Brauche ich ein Hintergrundbild für das Scoreboard oder reichen Textquellen?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Beides geht. Textquellen allein zeigen die Live-Werte; ein Hintergrundbild dahinter sorgt für ein gestaltetes Erscheinungsbild des Overlays."
      }
    }
  ]
}
</script>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "HowTo",
  "inLanguage": "de",
  "name": "Text-Timer oder -Zähler in OBS hinzufügen",
  "step": [
    { "@type": "HowToStep", "position": 1, "name": "OBS Studio öffnen", "text": "Starte OBS Studio auf deinem Computer." },
    { "@type": "HowToStep", "position": 2, "name": "Neue Szene erstellen (optional)", "text": "Klicke im Bereich Szenen auf die Schaltfläche +, gib der Szene einen Namen und speichere sie." },
    { "@type": "HowToStep", "position": 3, "name": "Textquelle hinzufügen", "text": "Klicke im Bereich Quellen auf die Schaltfläche + und wähle Text (FreeType 2), oder ziehe die gewünschte Textdatei aus dem Finder in das OBS-Fenster." },
    { "@type": "HowToStep", "position": 4, "name": "Textquelle benennen", "text": "Gib einen aussagekräftigen Namen für die Quelle ein und klicke auf OK, um sie zu erstellen." },
    { "@type": "HowToStep", "position": 5, "name": "Lesen aus Datei aktivieren", "text": "Aktiviere im Eigenschaftenfenster der Textquelle das Kontrollkästchen Aus Datei lesen." },
    { "@type": "HowToStep", "position": 6, "name": "TXT-Datei auswählen", "text": "Klicke neben dem Feld für den Dateipfad auf Durchsuchen, navigiere zu deiner lokalen TXT-Datei, wähle sie aus und klicke auf Öffnen." },
    { "@type": "HowToStep", "position": 7, "name": "Text auf der Arbeitsfläche platzieren", "text": "Ziehe das Textfeld im Vorschaubereich an die gewünschte Stelle in deiner Szene und passe die Größe bei Bedarf an." },
    { "@type": "HowToStep", "position": 8, "name": "Aussehen anpassen", "text": "Passe den Textstil über Schriftart, Größe und Farbe an." },
    { "@type": "HowToStep", "position": 9, "name": "Dateiaktualisierung testen", "text": "Ändere den Wert des Zählers in ScoreBoard und prüfe, ob die Änderungen sofort in OBS erscheinen." }
  ]
}
</script>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "HowTo",
  "inLanguage": "de",
  "name": "Scoreboard-Hintergrundbild in OBS hinzufügen",
  "step": [
    { "@type": "HowToStep", "position": 1, "name": "Bildquelle hinzufügen", "text": "Klicke im Bereich Quellen auf die Schaltfläche + und wähle Bild, oder ziehe die gewünschte Bilddatei aus dem Finder in das OBS-Fenster." },
    { "@type": "HowToStep", "position": 2, "name": "Bildquelle benennen", "text": "Gib einen aussagekräftigen Namen für die Quelle ein und klicke auf OK." },
    { "@type": "HowToStep", "position": 3, "name": "Bilddatei auswählen", "text": "Klicke neben dem Feld für den Dateipfad auf Durchsuchen, wähle deine lokale Bilddatei aus, klicke auf Öffnen und dann auf OK, um die Quelle zu speichern." },
    { "@type": "HowToStep", "position": 4, "name": "Bild unter den Textebenen platzieren", "text": "Ziehe das Bild im Vorschaubereich an die gewünschte Stelle, passe die Größe bei Bedarf an und verschiebe es in der Quellenliste ganz nach unten." }
  ]
}
</script>
