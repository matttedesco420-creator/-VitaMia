# Ausgaben – Einrichtung

Diese App läuft **vollständig auf deinem Gerät**. Kein Konto, kein Server,
keine Cloud. Alle Einträge und Belegbilder liegen im Speicher deines Handys.

---

## 1. API-Key

Die Texterkennung läuft über die Anthropic-API – derselbe Key wie bei der
Belegverwaltung funktioniert auch hier.

1. **console.anthropic.com** öffnen und anmelden
2. Unter **API Keys** → **Create Key** (oder den bestehenden verwenden)
3. Der Key beginnt mit `sk-ant-...`

Kosten: rund 0,3–1,5 Cent pro Beleg.

Läuft die Belegverwaltung unter derselben github.io-Adresse, übernimmt die
App den dort gespeicherten Key automatisch.

## 2. App veröffentlichen

**Neues** GitHub-Repository anlegen (z. B. `ausgaben`), alle Dateien
hochladen – `index.html` direkt im Hauptordner, die Icons im Ordner `icons/`, die Bibliotheken im Ordner `lib/`.
Dann **Settings → Pages** → *Deploy from a branch*, Branch `main`, Ordner `/ (root)`.

## 3. Auf dem Handy installieren

- **iPhone (Safari):** Teilen-Symbol → „Zum Home-Bildschirm"
- **Android (Chrome):** Menü → „App installieren"

---

## So funktioniert's

**Erfassen:** Großer Knopf öffnet die Kamera. Der Beleg wird ausgelesen,
einer Kategorie zugeordnet und dir zum Prüfen gezeigt. Nach „Speichern"
liegt er automatisch im richtigen Monat (nach Belegdatum). Ohne Beleg:
„Eintrag erstellen".

Wird derselbe Beleg ein zweites Mal hochgeladen (oder gleicher Betrag am
gleichen Tag), erscheint ein Hinweis.

**Übersicht:** Alle Monate mit Summe und farbigem Anteilsbalken je
Kategorie. Monat antippen → Aufteilung und alle Einträge. Kategorie
antippen filtert die Liste.

**Monats-PDF:** Im Monat „Monats-PDF speichern" – enthält Übersicht,
Einzelposten und alle Belegbilder (zwei pro Seite). Das PDF wird immer
frisch aus den aktuellen Daten erzeugt.

**Kategorien:** ⚙ → Kategorien. Anlegen, umbenennen, Farbe ändern,
löschen (Einträge werden vorher verschoben). Neue Kategorien lassen sich
auch direkt beim Prüfen eines Belegs anlegen.

## Speicher

Ein Belegbild braucht rund 80–150 KB. Bei 100 Belegen im Monat sind das
etwa 10–15 MB pro Monat – für ein Handy unproblematisch. Die Bilder bleiben
daher standardmäßig gespeichert.

Wer Platz sparen will: Monat öffnen → **Monats-PDF speichern** → PDF in
Dateien/iCloud ablegen → **Bilder entfernen**. Einträge und Summen bleiben,
nur die Bilder verschwinden vom Gerät.

## Sicherung

⚙ → Sicherung. „Mit Bildern" sichert alles, „Nur Einträge" ist deutlich
kleiner. Über „Sicherung einlesen" kommen die Daten auf ein neues Gerät;
vorhandene Einträge werden nicht doppelt angelegt.

Ohne Sicherung gibt es keine zweite Kopie: Löschst du die App vom
Startbildschirm oder verlierst das Handy, sind die Daten weg.
