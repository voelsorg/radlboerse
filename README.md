# Völser Radl-Börse

Website für die Völser Radl-Börse – ein Fahrrad-Tauschmarkt organisiert von der [Pfadfinder*innengruppe Völs](https://pfadivoels.at/).

**Live**: https://radlboerse.voels.org

## Über das Event

Die Völser Radl-Börse findet jährlich am CYTA-Gelände in Völs (Tirol) statt. Besucher können gebrauchte Fahrräder kaufen oder ihre eigenen Räder zum Verkauf anbieten. Der Reinerlös kommt der ehrenamtlichen Jugendarbeit der Pfadfinder*innen zugute.

## Technologie

- **Bootstrap 5.3.x** – CSS Framework
- **PPOE Theme** – Custom CSS nach [PPOE Brand Guidelines](https://ppoe.at/service/ressourcen/design/)
- **GitHub Pages** – Hosting

## Lokale Entwicklung

```bash
# Repository klonen
git clone https://github.com/voelsorg/radlboerse.git
cd radlboerse

# Lokalen Server starten (optional)
python3 -m http.server 8000
```

Dann http://localhost:8000 im Browser öffnen.

## Jährliche Aktualisierung

Vor jedem Event müssen folgende Stellen in `index.html` aktualisiert werden:

1. **Event-Datum** im Hero-Bereich (h1, h2)
2. **JSON-LD Structured Data** (startDate, endDate)
3. **Meta Description**
4. **Spendenabgabe-Frist** im Spenden-Bereich
5. **Copyright-Jahr** im Footer
6. **Telefonnummer** falls geändert

## Lizenz

Basierend auf [One Page Wonder](https://startbootstrap.com/template/one-page-wonder) von Start Bootstrap.

Code unter [MIT Lizenz](LICENSE).

## Kontakt

- E-Mail: radlboerse@gmail.com
- Website: https://pfadivoels.at
