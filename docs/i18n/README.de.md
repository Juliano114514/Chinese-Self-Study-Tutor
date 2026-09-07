# Chinese Self-Study Tutor

Ein anpassbares Codex-Skill für englisch- oder deutschsprachige Anfänger, die Hochchinesisch lernen. Der Tutor kann Hausaufgaben korrigieren, Mustertexte schreiben, Grammatik und Wortschatz erklären, Hanzi-Lektionen erstellen, Tests durchführen, wiederkehrende Probleme zusammenfassen und mündliche Übungen per Sprachfunktion leiten.

## Installation und Aufruf

Dieses Quellpaket wird nach `C:\Users\liangjiayin\.codex\skills\chinese-self-study-tutor` gespiegelt. Codex kann das Skill bei Chinesisch-Lernaufgaben automatisch auswählen. Du kannst es auch ausdrücklich mit `$chinese-self-study-tutor` aufrufen.

Beispiele:

- `$chinese-self-study-tutor Korrigiere diesen Tagebucheintrag auf normal.`
- `$chinese-self-study-tutor Erkläre mir 把 auf Deutsch, detailed.`
- `$chinese-self-study-tutor full: Erstelle aus 天、地、人 eine Lektion mit Test.`
- `$chinese-self-study-tutor Übe mit mir per Sprachfunktion eine Bestellung im Restaurant.`

## Antworttiefe

Wähle `quickest`, `simple`, `normal`, `detailed` oder `full`, oder überlasse die Wahl dem Tutor. Die Stufen sind flexible Empfehlungen und keine starren Vorlagen. Ab `normal` wird automatisch archiviert; Eingabedateien und ausdrücklich verlangte Dateiausgaben beginnen standardmäßig mindestens bei `normal`.

Pinyin mit Tonzeichen begleitet das unterrichtete Chinesisch auf jeder Stufe, sofern du nicht ausdrücklich darum bittest, Pinyin wegzulassen. Der Tutor schätzt dein aktuelles Niveau vorsichtig ein und unterrichtet zunächst auf der niedrigeren plausiblen Stufe. Erst wiederholte klare Belege oder dein ausdrücklicher Wunsch erhöhen das Niveau.

Bei Korrekturen auf `normal` enthält jeder sinnvolle Satz das korrigierte Chinesisch, das zugehörige Pinyin, eine Zerlegung in chinesischer Wortfolge, eine wörtliche und eine natürliche Übersetzung, gezielte Hinweise und eine kurze Übung. Zum Beispiel:

```text
我 / 这两天 / 都 / 居家办公
Wǒ / zhè liǎng tiān / dōu / jūjiā bàngōng
Ich / diese zwei Tage / alle / im Homeoffice arbeiten
Natürliches Deutsch: Ich arbeite seit zwei Tagen von zu Hause aus.
```

## Archiv

Umfangreichere Arbeit wird als eigenständiges HTML im Ordner `archive` des aktiven Arbeitsbereichs gespeichert und in `homework`, `tests`, `knowledge`, `speaking` und `reviews` eingeordnet. Quelldateien werden nie verändert. Dateinamen folgen `YYYYMMDD Titel.html` und `YYYYMMDD [Status] Titel.html`; bei Namenskonflikten wird eine Nummer angehängt, statt Dateien zu überschreiben.

Englisch ist die Standardsprache für Erklärungen. Auf Wunsch oder bei klarer Präferenz wird Deutsch verwendet. Standardmäßig nutzt der Tutor vereinfachte Schriftzeichen, kann sich aber an andere Wünsche anpassen.
