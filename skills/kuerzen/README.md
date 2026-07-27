# Kürzen: ein Skill zum Redigieren deutschsprachiger Geschäftstexte im Informationsstil

![Chaotische graue Textzeilen fallen in einen orangefarbenen Trichter und kommen als ordentliche, gleichmäßige orange Rechtecke wieder heraus — Unordnung wird zu strukturiertem Text](/.github/images/cover.webp)

Inspiriert von **[«Пиши, сокращай 2025»](https://sokratil.ru/)** („Schreib und Kürze 2025") von Maxim Iljachow und Ljudmila Sarytschewa.

> Dies ist die deutsche Version. Versionen für andere Sprachen finden Sie im [Haupt-README](../../README.md).

## Was es macht

Geben Sie Claude, ChatGPT oder Codex einen deutschsprachigen Geschäftstext, zum Beispiel eine E-Mail, Landingpage, Pressemitteilung, einen Lebenslauf, Bericht, eine Präsentation oder Kaltakquise-Mail. Das Skill redigiert ihn auf fünf Ebenen:

1. **Aufräumen auf Wortebene** — entfernt Füllphrasen, Unschärfen, aufgeblasenes Vokabular, leere Bewertungen und Floskeln
2. **Klarheit auf Satzebene** — wandelt Nominalstil in Verben um, bricht überladene Sätze auf, bringt Ordnung in Absätze, behebt Schachtelsätze und Verbalklammern
3. **Kampf dem Behördendeutsch** — sechs Werkzeuge gegen Beamtendeutsch, Nominalstil, Genitivketten und Funktionsverbgefüge
4. **Struktur und Zweck** — prüft die nützliche Wirkung, die Zielgruppe, die Textstruktur, Einleitung und Schluss
5. **Genre-Regeln** — Vorlagen und Prüfungen für „Über uns"-Seiten, Lebensläufe, Anschreiben, Kaltakquise-Mails, Pressemitteilungen, Arbeitsdokumente, Folien und Landingpages

Das Skill liefert eine redigierte Fassung mit Änderungsprotokoll und Empfehlungen, was die Autorin ergänzen sollte (Fakten, Beispiele, Recherche).

## Installation

### Über `npx skills` (empfohlen)

```bash
npx skills add iamursky/sokrati/tree/main/skills/kuerzen
```

### ChatGPT

1. Laden Sie den gesamten Ordner `skills/kuerzen` einschließlich `SKILL.md` und `references/` herunter
2. Öffnen Sie in der ChatGPT-Seitenleiste **Plugins → Skills**
3. Wählen Sie **Create → Upload from your computer** und laden Sie den Skill-Ordner hoch
4. Warten Sie, bis ChatGPT die Prüfung abgeschlossen hat. Wählen Sie das Skill anschließend mit `@` aus oder bitten Sie ChatGPT, einen Geschäftstext zu verbessern

### Claude Desktop / Web

1. Laden Sie den gesamten Ordner `skills/kuerzen` einschließlich [SKILL.md](SKILL.md) und `references/` herunter
2. Gehen Sie zu **Customize → Skills → + → Upload a skill**
3. Laden Sie den Skill-Ordner hoch
4. Das Skill aktiviert sich automatisch — bitten Sie Claude, das „Wasser" aus dem Text zu schneiden oder ihn „knackiger" zu machen

### Manuelle Installation für Claude Code

```bash
# Persönlich (in allen Projekten verfügbar)
git clone https://github.com/iamursky/sokrati ~/sokrati
ln -s ~/sokrati/skills/kuerzen ~/.claude/skills/kuerzen

# Projektbezogen (für das Team über Git verfügbar)
git clone https://github.com/iamursky/sokrati .sokrati
ln -s .sokrati/skills/kuerzen .claude/skills/kuerzen
```

## Verwendung

Das Skill wird automatisch aktiviert, wenn Sie:

- Claude, ChatGPT oder Codex bitten, einen Geschäftstext auf Deutsch zu bearbeiten, zu prüfen, zu entrümpeln oder zu verbessern
- Stichworte wie „Informationsstil", „Infostil", „Iljachow", „Glavred", „Füllwörter", „Floskeln", „Behördendeutsch", „Beamtendeutsch", „Nominalstil" oder „Substantivitis" erwähnen
- Bitten, das „Wasser" aus einem Text zu schneiden, ihn „knackiger" oder „verständlicher" zu machen
- Bitten, etwas in „einfache Sprache" oder „auf den Punkt" zu übersetzen
- „Marketing-Sprech", „Bullshit-Bingo" oder „Denglisch" entfernen lassen wollen

### Beispiele

**Vollständige Redaktion:**

> Redigier diesen Landingpage-Text im Informationsstil: [Text]

**Review ohne Umschreiben:**

> Gib mir Feedback zu dieser Mail. Was kann besser werden? [Text]

**Frage zur Technik:**

> Wie schreibe ich eine „Über uns"-Seite, die wirklich überzeugt?

## Urheberschaft

Das Skill ist inspiriert von **«Пиши, сокращай 2025»** von Maxim Iljachow und Ljudmila Sarytschewa. Es ist kein offizielles Produkt der Buchautoren und gibt den Originaltext nicht wieder. Die Ideen und Techniken gehören den Autoren des Buchs; dieses Skill interpretiert sie als Arbeitsablauf für einen KI-Assistenten. Wenn Sie Russisch lesen und das Buch mögen, unterstützen Sie die Autoren, indem Sie es über den oben verlinkten Verlag kaufen.
