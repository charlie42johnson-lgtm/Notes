# 10 - Syntax 2: Hierarchische Satzstruktur

## Grenzen der traditionellen Syntax

### Problem: Mehrdeutigkeit
Die traditionelle Konzeption betrachtet Sätze als **linear**.
Doch Sätze haben eine **innere Hierarchie**.

### Beispiel 1: Deutsch

**Satz**: Im Wald leben viele böse Wiesel und Hermeline.

#### Mögliche Lesarten:

**Lesart 1**: [viele böse Wiesel] und Hermeline
- viele böse Wiesel und (außerdem) Hermeline
- Hermeline sind **nicht böse**

**Lesart 2**: viele [böse Wiesel und Hermeline]
- viele böse Wiesel und viele Hermeline
- Hermeline sind **vielleicht böse**

**Lesart 3**: viele böse [Wiesel und Hermeline]
- viele böse Wiesel und viele böse Hermeline
- **Alle** sind böse

### Beispiel 2: Russisch

**Satz**: Мы будем жить плохо, но не долго.
(My budem žit' plocho, no ne dolgo.)

#### Mögliche Lesarten:

**Lesart 1**: Мы будем [плохо жить], [но не долго]
- 'Wir werden schlecht leben, aber nicht lange leben'

**Lesart 2**: Мы будем [плохо жить], [но не долго]
- 'Wir werden schlecht leben, aber nicht lange schlecht leben'

### Erkenntnis
Der **Sinn hängt davon ab**, wie die Satzteile **hierarchisch zueinander stehen**.

## Phrasenstrukturgrammatik

### Grundidee
- **Hierarchische** Betrachtung der Syntax
- Sätze werden in **Phrasen** zerlegt
- Phrasen werden von einem **Einzelwort dominiert** (Kopf)
- Der **Typ der Phrase** ergibt sich aus der **Wortart des Kopfes**

### Phrasentypen

| Phrasentyp | Kopf | Satzgliedfunktion | Beispiel |
|------------|------|-------------------|----------|
| **Nominalphrase (NP)** | Nomen | Subjekt, Objekt, Prädikativ | das kleine Kind |
| **Verbalphrase (VP)** | Verb | Prädikat | in die Schule gehen |
| **Adjektivphrase (AP)** | Adjektiv | Prädikativ, Attribut | sehr groß |
| **Adverbphrase (AvP)** | Adverb | Umstandsergänzung | sehr oft |
| **Präpositionalphrase (PP)** | Präposition | Umstandsergänzung | auf dem Tisch |

### Baumstruktur

```
S (Satz)
├── NP1 (Subjekt)
│   └── Ich
└── VP (Prädikat)
    ├── V
    │   └── lege nieder
    ├── NP2 (Objekt)
    │   ├── Prn
    │   │   └── mein
    │   └── N
    │       └── Amt
    └── PP3 (Umstandsergänzung)
        ├── Prp
        │   └── mit
        └── NP3
            ├── N3
            │   └── Sorge
            ├── Knj
            │   └── und
            └── N3
                └── Zuversicht
```

### Integration traditioneller Satzglieder

```
S
├── NP1 (Subjekt)
├── VP (Prädikat)
│   ├── V
│   ├── NP2 (Objekt)
│   └── PP3 (Umstandsergänzung)
└── (weitere Konstituenten)
```

## Dependenzgrammatik

### Grundidee
Das **Verb beherrscht das gesamte Satzgerüst** über seine lexikalischen Eigenschaften.

### Stemma (hierarchische Darstellung)
- **Verb steht an oberster Stelle**
- Nach Tesnière (1959): Atommodell

### Atommodell
```
        Verb (Kern)
       /    |    \
      /     |     \
  Subj.   Obj.  Umstandsergänzung
```

### Argumente

#### Obligatorische Argumente (Aktanten)
- Das Verb fordert sie **zwingend**
- **Typischerweise**: Subjekt und Objekte

#### Fakultative Argumente (Zirkumstanten)
- Können **ergänzt oder weggelassen** werden
- **Typischerweise**: Umstandsergänzungen

### Beispielstemma

```
lege nieder (Verb, Kern)
├── ich (Subjekt, Aktant)
├── Amt (Objekt, Aktant)
└── mit Sorge und Zuversicht (Umstandsergänzung, Zirkumstant)
    └── und
        ├── Sorge
        └── Zuversicht
```

### Integration klassischer Syntax
Auch in diese Darstellung lässt sich jene der klassischen Grammatik integrieren.

## Valenz (Dependenzgrammatik)

### Definition
Verben werden nach der **Anzahl der geforderten Aktanten** eingeteilt.

### Valenztypen

#### 1. Avalente Verben (Nullstellig)
- **Benötigen**: weder Subjekt noch Objekte
- **Typ**: unpersönliche Verben (Wetterverben)

| Sprache | Beispiel | Bedeutung |
|---------|----------|-----------|
| **Deutsch** | (es) regnet | |
| **Finnisch** | sataa | 'es regnet' |
| **Tschechisch** | prší | 'es regnet' |
| **Russisch** | темнеет (temneet) | 'es wird dunkel' |

**Hinweis**: In germanischen Sprachen wird "Nullsubjekt" gefordert.

#### 2. Univalente Verben (Einstellig)
- **Benötigen**: ein Subjekt, aber kein Objekt
- **Typ**: intransitive Verben

| Sprache | Beispiel | Bedeutung |
|---------|----------|-----------|
| **Deutsch** | ich lache | |
| **Bulgarisch** | тя спи (tja spi) | 'sie schläft' |

#### 3. Bivalente Verben (Zweistellig)
- **Benötigen**: ein Subjekt und ein direktes Objekt
- **Typ**: einfach transitive Verben

| Sprache | Beispiel | Bedeutung |
|---------|----------|-----------|
| **Deutsch** | ich lese ein Buch | |
| **Polnisch** | ja czytam książkę | 'ich lese ein Buch' |

#### 4. Trivalente Verben (Dreistellig)
- **Benötigen**: ein Subjekt, ein direktes und ein indirektes Objekt
- **Typ**: ditransitive Verben

| Sprache | Beispiel | Bedeutung |
|---------|----------|-----------|
| **Deutsch** | ich gebe dir ein Buch | |
| **Neuštokavisch** | ja ti dajem knjigu | 'ich gebe dir ein Buch' |

## Semantische Rollen (Theta-Rollen)

### Problem der Kasus
- Kasus übernehmen **mehr als eine Funktion**
- Ein Kasus kann **verschiedene Rollen** ausdrücken

### Beispiel: Nominativ

| Satz | Rolle des Nominativs |
|------|---------------------|
| Tante Moni wirft den Ziegelstein durchs Fenster. | **Agens** (handelnde Person) |
| Tante Moni bekommt ein Geschenk. | **Rezipient** (Empfänger) |
| Tante Moni erleidet einen Nervenzusammenbruch. | **Patiens** (Opfer) |

### Beispiel: Agens-Ausdruck

| Sprache | Satz | Kasus des Agens |
|---------|------|-----------------|
| **Polnisch** | Student kupuje książkę. | Nominativ |
| **Deutsch** | Der Student kauft ein Buch. | Nominativ |
| **Polnisch** | Książka jest kupowana przez studenta. | Genitiv |
| **Deutsch** | Das Buch wurde von einem Studenten gekauft. | Genitiv/Dativ |

**Erkenntnis**: Die **semantische Rolle** bleibt dieselbe, unabhängig vom Kasus.

### Zentrale semantische Rollen (Auswahl)

| Rolle | Definition | Beispiel |
|-------|------------|----------|
| **Agens** | Handelnde Person | Tante Moni wirft... |
| **Patiens** | Opfer einer Handlung | Tante Moni erleidet... |
| **Thema** | Gegenstand einer Handlung, "unbelebtes Opfer" | Ich gebe **dir ein Buch** |
| **Rezipient** | Empfänger eines Themas | Ich gebe **dir** ein Buch |
| **Instrument** | Mittel zum Zweck, "unbelebter Agens" | Ich schneide **mit dem Messer** |
| **Experiens** | "Empfindende" Person | Tante Moni **hasst** Kinder |

### Valenzdarstellung im mentalen Lexikon

#### Beispiel: geben
```
geben
├── [Agens]
├── [Thema/Rezipient]
└── [Rezipient]
```

#### Beispiel: hassen
```
hassen
├── [Experiens]
└── [Thema/Patiens]
```

## Generative Grammatik (Wiederholung und Vertiefung)

### Entwicklung
- Kern aus Phrasenstrukturgrammatik entwickelt
- **Schlüsselwerk**: Chomsky, *Syntactic Structures* (1957)
- **Minimalist Program** (1995): Radikale Reform

### Zentrale Konzepte

#### 1. Generativ
- "die Erzeugung betreffend"
- Wie Sätze erzeugt werden

#### 2. Tiefen- und Oberflächenstruktur (Frühe Version)

| Aspekt | Tiefenstruktur | Oberflächenstruktur |
|--------|----------------|---------------------|
| **Ebene** | Abstrakt | Real geäußert |
| **Sprachen** | Allen gemein | Sprachspezifisch |
| **Verbindung** | Transformationsregeln |

#### 3. Universalgrammatik (UG)
- **Angeboren** im menschlichen Gehirn
- Grundprinzipien der Syntax

#### 4. Prinzipien- und Parametermodell

##### Prinzipien
- **Universal**, in allen Sprachen gleich

##### Parameter
- **Sprachspezifisch**
- Werden beim Spracherwerb gelernt

### Spracherwerb

#### Das "Armut des Reizes"-Problem
- Sprachlicher Input ist **spärlich und defektiv**
- Kinder lernen trotzdem perfekt

#### Erklärung
- Kinder konkretisieren **angeborene kognitive Strukturen**
- Aus Input werden **spezifische Parameter** abgeleitet
- Produzieren **nie gehörte** Sätze korrekt

### Module der GG (Auswahl)

#### X'-Schema (X-bar)
- **Allgemeines Bauprinzip** von Phrasen
- **Regel**: XP → X
- Jede Phrase hat einen **Kopf**
- **Verzweigung**: Nur in zwei Richtungen
- **Zwischenstufen**: Mit Strich (') markiert

#### Kasusfilter
- **Jede NP erhält genau einen Kasus**
- Zuweisung vom Verb (Kopf der VP) aus
- **Beispiele**:
  - das Amt niederlegen → Amt: Akkusativ
  - jemandem treu sein → jemandem: Dativ

#### Move-α
- **Phrasenbestandteile können verschoben werden**
- Regeln sind **sprachspezifisch** (Parameter)
- **Beispiel**: Wh-Bewegung

| Typ | Beispiel |
|-----|----------|
| **Aussagesatz** | Ich habe das Buch gelesen. |
| **mit Wh-Element** | Ich habe **[welches Buch]** gelesen. |
| **Fragesatz** | **[Welches Buch]** habe ich gelesen? |

## Satzverbindungen

### Übersicht

```
Sätze
├── einfache Sätze
│   └── Ich hasse dich.
│
└── zusammengesetzte Sätze
    ├── Satzverbindung (Parataxe)
    │   ├── asyndetisch (ohne Bindewort)
    │   │   └── Heute hasse ich dich, morgen liebe ich dich.
    │   │
    │   └── syndetisch (mit Bindewort)
    │       └── Heute hasse ich dich, und morgen liebe ich dich.
    │
    └── Satzgefüge (Hypotaxe)
        └── Ich hasse dich, weil du blöd bist.
```

### Satzverbindung (Parataxe)

#### Definition
Verbindung **zweier selbstständiger Sätze**.

#### Arten

##### a) Asyndetische Satzverbindung
- **Ohne Bindewort**
- **Beispiel**: Heute hasse ich dich, morgen liebe ich dich.

##### b) Syndetische Satzverbindung
- **Mit Bindewort**
- **Beispiel**: Heute hasse ich dich, und morgen liebe ich dich.

### Satzgefüge (Hypotaxe)

#### Definition
Verbindung eines **selbstständigen** mit einem **unselbstständigen** Satz.

#### Terminologie
- **Hauptsatz**: Selbstständiger Satz
- **Nebensatz**: Unselbstständiger Satz

#### Beispiele

| Typ | Beispiel |
|-----|----------|
| **Standard** | Ich hasse dich, weil du blöd bist. |
| **Infinitivsatz** | Er versprach mir, morgen zu kommen. |
| **Subjektsatz** | Mich überrascht, wie intelligent du bist. |

#### Grenzfälle

##### Nebensätze mit Satzfähigkeit
- **Beispiel 1**: Dass du mir ja nicht wieder besoffen Rad fährst!
- **Beispiel 2**: Bis einer heult.

**Kriterium**: Nebensätze hängen von Hauptsätzen ab, sind diesen also untergeordnet.

### Nebensatztypen

Nebensätze lassen sich wie Satzglieder typologisieren:

| Typ | Beispiel | Frageprobe |
|-----|----------|------------|
| **Objektsatz** | Ich weiß, wer du bist. | Was weiß ich? |
| | Er versprach, heute zu kommen. | Was versprach er? |
| **Subjektsatz** | Wer nicht hören will, muss fühlen. | Wer muss fühlen? |
| | Mir ist bewusst, dass ich übertreibe. | Was ist bewusst? |
| **Attributsatz** | Das Kind, das ich meine, fehlt heute. | vgl. Das nervige Kind... |
| **Adverbialsatz** | Siehe unten | |

### Adverbialsätze

#### Definition
Nebensätze, die eine Umstandsergänzung ersetzen.

#### Erkennbar an
Der **Konjunktion**, von der sie eingeleitet werden.

#### Wichtige Typen

| Typ | Konjunktion (dt.) | Beispiel |
|-----|-------------------|----------|
| **Temporal** | als, während, seit, bevor | Als er antanzte, war es schon zu spät. |
| **Kausal** | weil, da | Der Zug fällt aus, weil der Schaffner verschwunden ist. |
| **Final** | damit | Gib Uwe bitte die Schaufel, damit endlich Ruhe am Spielplatz ist. |
| **Konzessiv** | obwohl | Obwohl sie schlechte Laune hatte, ging sie zur Arbeit. |
| **Konditional** | wenn, falls | Wenn du kommst, freue ich mich. |

#### Konjunktionen in verschiedenen Sprachen

| Typ | Deutsch | Russisch | Neuštokavisch |
|-----|---------|----------|---------------|
| **Temporal** | als, während | (в то время как) | dok, otkad |
| **Kausal** | weil, da | (потому что) | jer |
| **Final** | damit | что́бы | da |
| **Konditional** | wenn, falls | когда́, е́сли | kad, ako |

## Verknüpfungen zu anderen Vorlesungen

- [[01 - Einführung in die Linguistik]]: Strukturebenen, GG
- [[02 - Geschichte und Zeichen]]: Strukturalismus
- [[05 - Morphologie 1]]: Flexion
- [[06 - Morphologie 2]]: Morphosyntax, grammatische Kategorien
- [[07 - Wörter]]: Wortarten
- [[08 - Semantik]]: Satzsemantik
- [[09 - Syntax 1]]: Satzglieder, Valenz
- [[X - Besonderheiten]]: Slavische Satzstrukturen

## Zusammenfassung

### Wichtige Erkenntnisse

1. **Sätze sind hierarchisch strukturiert**, nicht linear
2. **Phrasenstrukturgrammatik** zeigt diese Hierarchie
3. **Dependenzgrammatik** betont die zentrale Rolle des Verbs
4. **Semantische Rollen** sind unabhängig von Kasus
5. **Valenz** bestimmt die Satzstruktur
6. **Generative Grammatik** sucht universale Prinzipien
7. **Satzverbindungen** können parataktisch oder hypotaktisch sein
