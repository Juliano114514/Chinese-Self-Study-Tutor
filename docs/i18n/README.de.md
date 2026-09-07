# Chinese Self-Study Tutor

Ein anpassbares Codex-Skill für deutschsprachige Anfänger, die Hochchinesisch lernen. Der Tutor korrigiert Texte, erklärt Grammatik und Wortschatz, vermittelt Hanzi über nützliche Wörter, erstellt Übungen, fasst wiederkehrende Probleme zusammen und unterstützt Sprechübungen.

Sprachen: [Englisch](../../README.md) · [Chinesisch](README.zh-CN.md) · **Deutsch**

## Schnellstart

Installationsbereich: `user`

Codex kann das Skill bei Chinesisch-Lernaufgaben automatisch auswählen. Du kannst es auch ausdrücklich aufrufen:

```text
$chinese-self-study-tutor normal: Korrigiere diesen Tagebucheintrag und erkläre die wichtigsten Fehler.
```

Weitere sofort nutzbare Aufgaben findest du in der [deutschen Schnellstart-Anleitung](quickstart.de.txt).

## Antworttiefe wählen

- `quickest`: eine direkte Antwort oder Korrektur mit Pinyin und Tonzeichen.
- `simple`: die Antwort mit der wichtigsten Begründung, Abgrenzung oder einem Beispiel.
- `normal`: eine kompakte Lerneinheit mit chinesischer Wortfolge, Bedeutung, Hinweisen und kurzer Übung.
- `detailed`: ausführlichere Vergleiche, Gebrauchshinweise und gezielte Übungen.
- `full`: eine wiederverwendbare Lerneinheit mit Diagnose, Mustertext, umfangreicheren Übungen und nächsten Schritten.

Pinyin mit Tonzeichen begleitet das unterrichtete Chinesisch auf jeder Stufe, sofern du nicht ausdrücklich darum bittest, es wegzulassen. Der Tutor schätzt dein Niveau vorsichtig ein und unterrichtet zunächst auf der niedrigeren plausiblen Stufe. Erst wiederholte klare Belege oder dein ausdrücklicher Wunsch erhöhen das Niveau.

## So werden Korrekturen erklärt

Ab `normal` können Korrekturen Satz für Satz das verbesserte Chinesisch, passendes Pinyin, eine Zerlegung in chinesischer Wortfolge, eine wörtliche und eine natürliche Übersetzung, gezielte Hinweise und eine kurze Übung enthalten. Zum Beispiel:

```text
我 / 这两天 / 都 / 居家办公
Wǒ / zhè liǎng tiān / dōu / jūjiā bàngōng
Ich / diese zwei Tage / durchgehend / im Homeoffice arbeiten
Natürliches Deutsch: Ich arbeite seit zwei Tagen von zu Hause aus.
```

## Hanzi und Wortschatz

Bei einem unbekannten Hanzi beginnt der Tutor normalerweise mit einem kleinen Netz nützlicher Wörter statt mit einer isolierten Wörterbuchdefinition. **烛** (*zhú*) kann zum Beispiel über **蜡烛** (*làzhú*, Wachskerze), **烛火** (*zhúhuǒ*, Kerzenflamme), **烛光** (*zhúguāng*, Kerzenlicht) und **烛台** (*zhútái*, Kerzenständer) eingeführt werden. Das ist ein flexibler Unterrichtsansatz und keine feste Wortzahl.

## Standardeinstellungen und Archiv

- Erklärungen sind standardmäßig auf Englisch; Deutsch kann jederzeit verlangt werden.
- Der Tutor verwendet standardmäßig Hochchinesisch, vereinfachte Schriftzeichen und Pinyin mit Tonzeichen.
- Arbeit ab `normal` wird als eine eigenständige HTML-Datei im Ordner `archive` des aktiven Arbeitsbereichs gespeichert.
- Bei Korrekturen bleibt die Eingabedatei unverändert; Originaltext, Korrektur und Hinweise stehen gemeinsam in derselben Archivdatei.
- Dateinamen folgen `YYYYMMDD [Status] Titel.html`; bei Namenskonflikten verhindert ein Zahlenzusatz das Überschreiben.

Eine Eingabedatei oder ausdrücklich verlangte Dateiausgabe verwendet standardmäßig mindestens `normal`, sofern du nicht `quickest` oder `simple` wählst.
