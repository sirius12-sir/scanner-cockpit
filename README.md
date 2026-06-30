# Scanner-Cockpit

**Ein Steuerstand für Menschen, die mehrere unverwandte Domänen gleichzeitig betreiben.**

Kein Produktivitäts-Tool im üblichen Sinn. Eher das Gegenteil: ein Werkzeug für die, denen die üblichen Tools nicht passen, weil sie für *ein* Leben mit *einer* Richtung gebaut sind.

## Das Problem

Wer mehrere unverwandte Felder ernsthaft betreibt — nicht nebenher, sondern mit echter Tiefe in jedem —, scheitert selten am Können. Er scheitert an den **Umschaltkosten**.

Jeder Wechsel von einer Domäne in die nächste kostet: Wo war ich? Welcher Stand? Welches Werkzeug, welche offene Frage, welcher halbfertige Gedanke? Bei zwei Feldern ist das Reibung. Bei fünf oder acht frisst diese Reibung die Breite auf, für die man sich die Felder überhaupt erst zugelegt hat. Das ist der Punkt, an dem die meisten Vielseitigen aufgeben und sich doch auf eines verengen — nicht aus Einsicht, sondern aus Erschöpfung.

## Das Prinzip

Die Lösung ist nicht mehr Disziplin. Disziplin skaliert nicht über acht Domänen. Die Lösung ist, die **Wiedereinstiegskosten gegen null zu drücken**.

Das ist dieselbe Logik wie 5S in einer Werkstatt, nur angewandt auf den Kopf statt auf die Wand: Jede Domäne hat ihren eigenen, abgegrenzten Bereich. Der Zustand bleibt stehen wie eine angehaltene Maschine — man muss den Kontext nicht neu laden, wenn man zurückkommt. Man kann eine Sache mitten im Satz liegen lassen und Wochen später dort weitermachen, ohne Anlauf.

Infrastruktur statt Willenskraft. Zustand erhalten statt Gedächtnis belasten. Wer so arbeitet, hält nicht acht Felder im Kopf — er hält acht Felder in einer Struktur, die ihm das Im-Kopf-Halten abnimmt.

Das Scanner-Cockpit ist eine Umsetzung dieses Prinzips für die digitale Seite. Die physische Seite — getrennte Werkstätten, Werkzeug griffbereit, gängige Teile auf Lager — löst man anders, aber nach demselben Gesetz.

## Was es tut

- Domänen als getrennte Bereiche, nicht als eine flache Liste. Was zum einen Feld gehört, taucht nicht zwischen zwei anderen auf.
- Pro Bereich bleibt der Zustand erhalten: offene Punkte, Notizen, der Faden, an dem man zuletzt war.
- Schneller Wiedereinstieg: aufmachen, sehen wo man war, weitermachen. Kein Sortieren, kein Suchen.

Bewusst schlicht. Das Tool ist kein Ziel, es ist ein Wiedereinstiegspunkt.

## Die bewussten Entscheidungen

Hier steht, *warum* es so gebaut ist. Wer nur die Features will, kann das überspringen. Wer die Begründung liest und nickt, ist vermutlich der Grund, warum dieses Repo öffentlich ist.

**Kein Backend, kein Account, kein SaaS.** Die Daten liegen über die File System Access API als ganz normale Datei auf der eigenen Platte. Sie gehören dir, sie bleiben bei dir, sie gehen durch keine fremde Cloud. Das ist kein fehlendes Feature, das ist die Hauptentscheidung. Wer mehrere Lebensbereiche an einem Ort bündelt, darf diesen Ort nicht jemand anderem geben.

**localStorage als Fallback**, wenn die File-API nicht verfügbar ist. Kein Datenverlust — aber die eigene Datei ist der erste Weg.

**Eine einzige HTML-Datei.** Kein Build-Schritt, keine Abhängigkeiten, kein Framework, das in drei Jahren nicht mehr sauber installiert. Doppelklick, läuft. Das ist Absicht: Ein Werkzeug, das man jahrelang benutzen will, muss auch in zehn Jahren noch starten und reparierbar sein — von einem selbst, ohne Toolchain-Archäologie.

## Was es bewusst nicht tut

- Keine Cloud-Sync, keine Multi-Device-Magie. Wer das braucht, synct die Datei selbst, mit Mitteln, denen er traut.
- Keine Gamification, keine Streaks, keine Benachrichtigungen. Es soll nichts von dir wollen.
- Kein KI-Schnickschnack. Das Tool denkt nicht für dich — es vergisst nur nicht für dich.
- Keine Kollaboration. Das hier ist ein Einzel-Steuerstand. Mit Absicht.

Wenn dir die Hälfte davon fehlt, ist das nicht dein Tool — und das ist in Ordnung. Es ist für eine schmale Sorte Mensch gebaut.

## Für wen das ist

Für jemanden, der mehrere unverwandte Welten gleichzeitig betreibt — mit Tiefe in jeder, nicht nur Interesse — und sie nicht durch Willenskraft zusammenhält, sondern durch Struktur. Der lieber eine Stunde investiert, ein System zu bauen, das ihm hundert Stunden Suchen erspart. Dem Autonomie kein Schlagwort ist, sondern Funktionsprinzip.

## Wenn das nach dir klingt

Dann interessiert dich an diesem Repo vermutlich nicht das Tool, sondern die Betriebsart dahinter.

Davon gibt es wenige. Ich kenne kaum jemanden, der so arbeitet, und hätte gern jemanden zum Reden — nicht über das Fachthema (Tiefe kann jeder selbst), sondern über das *Wie*: wie man mehrere Domänen auf Niveau hält, ohne sich zu zerlegen. Wenn du das auch tust, mach ein Issue auf oder schreib mir: **[KONTAKT EINTRAGEN]**

Kein Verein, keine Community, kein Newsletter. Nur die Möglichkeit, dass sich zwei Leute finden, die dieselbe seltene Sache machen.

---

*Lizenz: MIT — nimm es, bau es um, mach es zu deinem. Genau dafür liegt es hier.*
