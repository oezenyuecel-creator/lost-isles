# LOST ISLES 🏝️

### *Survive · Explore · Escape*

Ein **stilisiertes 3D Survival-/Erkundungs-Abenteuer** fürs Handy — im Geiste von *Raft × Oceanhorn × Animal Crossing*, aber mit eigener Identität und einem Geheimnis hinter dem Archipel.

Eigenständiger **One-File-Prototyp** (`index.html`) auf Basis von [three.js](https://threejs.org). Keine Build-Tools, keine Installation, keine Assets — die komplette Welt (Inseln, Wasser-Shader, Charakter, Tiere, Sound) wird **prozedural** erzeugt & vertont. Läuft direkt im Handy-Browser.

> **Status: v0.1 – spielbarer Vertical-Slice.** Der Kern steht: stranden, sammeln, craften, ein Floß bauen, zur nächsten Insel segeln, tauchen, Haien entkommen — und den ersten Faden des Archipel-Geheimnisses ziehen. Die große Vision (Basenbau, Zähmen, Bosse, Koop, hunderte Sammelobjekte, persistente Jahreszeiten-Welt) ist bewusst **noch nicht** enthalten — siehe [Roadmap](#roadmap-zur-vollen-vision).

---

## 📖 Story

Dein Flugzeug gerät über dem Ozean in Turbulenzen und stürzt ab. Du überlebst, treibst tagelang auf einem Stück Holz und wirst schließlich an eine einsame tropische Insel gespült.

Dein Ziel: **von der Insel entkommen.** Sammle Ressourcen, stelle Werkzeuge her, baue ein Floß, entdecke weitere Inseln — und baue schließlich ein seetüchtiges Boot zur Flucht.

Doch je weiter du kommst, desto klarer wird: Der Absturz war **kein Zufall**. Ein Funkspruch. Ein Wrack. Eine alte Ruine mit leuchtendem Stein. Ein seltsames Licht am nächtlichen Horizont…

---

## 🎮 Steuerung (Mobile-first)

| Aktion | Handy | Desktop |
|---|---|---|
| Bewegen | linker Joystick | `WASD` / Pfeiltasten |
| Kamera | rechts über den Screen ziehen | Maus ziehen |
| Springen | Knopf **⤒** | `Leertaste` |
| Sprinten | Knopf **»** (halten) | `Shift` |
| Tauchen / Auftauchen | Knopf **⤓** (im Wasser) | Knopf |
| **Sammeln / Interagieren** | großer Knopf **✋ AKTION** | `E` |

Oben rechts: 🎒 Inventar · 🔨 Werkbank · 📜 Questbuch · 🗺️ Seekarte · 📖 Sammlung.

---

## ✨ Was schon drin ist (v0.1)

- **Stilisierte 3D-Welt** — prozedurale Inseln mit Strand/Gras/Fels, wehende Palmen, driftende Wolken, low-poly Look.
- **Animierter Wasser-Shader** — echte Wellen, Fresnel, Sonnen-Glitzern, Schaumkämme; das Meer bewegt sich mit dir (endloser Ozean).
- **Dynamischer Tag/Nacht-Zyklus** — Sonnenauf-/untergang, wandernde Sonne, warme Sunset-Farben, Sternennacht.
- **Wettersystem** — Klar, Brise, Bewölkt, Regen, Sturm mit Blitzen; beeinflusst Wellen, Sicht (Nebel) und Stimmung.
- **Sammeln per Antippen** — Kokosnüsse, Holz, Steine, Palmblätter, Bananen, Muscheln, Krabben, Trinkwasser, Bambus, Lianen.
- **Crafting** — Seil, Steinbeil, Speer, Angel, Fackel, Lagerfeuer, Wasserfilter, Schlafplatz, **Floß**, Segel, Harpune, **Segelboot**. Bessere Werkzeuge = mehr Ertrag.
- **Überlebens-Bedürfnisse** — Vitalität, Hunger, Durst, Energie (+ Sauerstoff beim Tauchen). Entspannt, nicht bestrafend.
- **See-Reise** — Floß bauen → antippen → auf der Karte ein Ziel wählen und zu neuen Inseln **segeln**.
- **Tauchen** — Unterwasserwelt mit Perlen, Korallen, Seesternen und versunkenen Schatztruhen.
- **Lebendiges Meer** — Fischschwärme, Möwen, Papageien, ein springender **Delfin**, ein **Wal** am Horizont.
- **Haie** 🦈 — schwimmst du zu weit raus, kreist ein Hai, jagt dich schließlich — schnell zurück an Land! (Speer/Harpune wehren ab.)
- **Quest-Kette** — führt Schritt für Schritt von „Sammle 5 Kokosnüsse" bis „Entkomme dem Archipel".
- **Sammlungsbuch** 📖 — entdeckte Arten & Objekte werden geloggt (100 %-Sammler-Motivation).
- **Geheimnis-Hooks** — Flugzeugwrack, abhörbarer Funkspruch, alte Ruine, geheimnisvolles Licht am Nacht-Horizont.
- **Prozeduraler Sound** — Wellenrauschen, Musik-Pad, Sammel-Blips, Hai-Spannungs-Drone, Gewitter.
- **Auto-Save** (localStorage) — dein Fortschritt bleibt erhalten; „Fortsetzen" auf dem Startscreen.
- **Intro-Cinematic** — Flugzeugabsturz → Treiben → Anspülung (überspringbar).

---

## 🚀 Spielen

**Einfach [`index.html`](index.html) im Browser öffnen** — fertig. Am besten auf dem Handy im Querformat.

Lokal mit Server (empfohlen, wegen ES-Modules):
```bash
npx serve .
# dann http://localhost:3000 im Browser öffnen
```

> Benötigt einen modernen Browser (WebGL2 + Import-Maps): iOS Safari 16.4+, aktuelles Chrome/Android.

---

## 🗺️ Roadmap zur vollen Vision

Bewusst **nicht** in v0.1 — die Bausteine für ein Spiel, das man über Monate täglich öffnet:

- **Persistente Welt** — Jahreszeiten, tägliche Schatzkisten, wandernde Fischschwärme, Insel-Events (Meteoriten, Piratenschiffe, gestrandete Container).
- **Basenbau** — Haus, Küche, Werkstatt, Lager, Hafen, Farm, Fischteich, Obstgarten — die Insel zum Paradies ausbauen.
- **Tiere zähmen** — Papageien, Schildkröten reiten, Affen sammeln Kokosnüsse, Hunde finden Schätze, Delfine zeigen Wracks.
- **Meeresleben & Bosse** — Wale, Orcas, Mantas, Kraken; Setpiece-Bosse (Weißer Hai, Riesen-Kraken, Seeschlange).
- **Riesige Sammlung** — 100+ Fischarten, 60+ Muschelarten, Fossilien, Münzen, Artefakte, Flaschenpost — alles im Sammlungsbuch.
- **Story-Mystery** — andere Überlebende, verlassene Lager, Forschungsstationen, alte Tempel, eine vergessene Zivilisation.
- **Koop** — bis zu 4 Freunde: gemeinsam bauen, tauchen, Bosse bestreiten.
- **Native App** — Portierung nach Unity/Godot für 60 FPS 3D & App-Store-Release.

---

*Prototyp gebaut mit [Claude Code](https://claude.com/claude-code). Ein Spiel-Konzept — kein kommerzielles Produkt.*
