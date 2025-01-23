### README: PV Machbarkeitsanalyse

#### Beschreibung
Dieses Programm berechnet wichtige Kennzahlen für die Realisierung einer Photovoltaikanlage (PV-Anlage) an einer Fassade. Die Anwendung dient als erste Entscheidungshilfe und liefert wirtschaftliche und energetische Analysen basierend auf Benutzer-Inputs und hochgeladenen 3D-Modelldaten.

---

### Funktionen
1. **Eingabe einer Fassadengeometrie und Umgebungsgeometrie:**
   - Unterstützt `.3dm`-Dateien (Rhino 3D-Format).
   - Verarbeitet und analysiert Geometrien mit korrekten Attributnamen / "Objektnamen" in Rhino.

2. **Berechnung wirtschaftlicher Kennzahlen:**
   - Berücksichtigt Parameter wie Investitionskosten, Instandhaltungskosten, Förderbeiträge und Strompreise.

3. **Generierung von Ergebnissen:**
   - Erstellt wirtschaftliche und energetische Kennzahlen, darunter Amortisationsdauer, Rendite und Stromproduktion.
   - Gibt eine Visualisierung der Verschattung auf der Fassade (3D-Geometrie) aus.

4. **Integration mit Grasshopper:**
   - Führt benutzerdefinierte Grasshopper-Definitionen aus, um die Geometrie und wirtschaftliche Daten zu berechnen.

---

### Eingabeparameter
Das Programm benötigt folgende Inputs:
1. **Fassadengeometrie (Auswahl)**  
   - Rhino `.3dm`-Datei, die die Fassadenfläche und Kontextgeometrien enthält.
   - Die Fassadengeometrie und die Kontextgeometrien müssen unterschliedliche Objektnamen haben.
   - Wenn alle Kontextgeometrien den selben Namen besitzen muss auf Viktor nur eine der Geometrien angewählt werden, der Rest wird automatisch übernommen.
   
2. **Parameter für die Berechnungen:**
   --> Standardwerte sind voreingestellt, können aber je nach Situation und Modultyp stark variieren! Entsprechende Links sind im Beschrieb bereitgestellt.
   - Modultyp (Optionen: L, Q, M, S) --> Standard Modultypen welche in Zukunft mit einer Datenbank hinterlegt werden.
   - Eigenverbrauch (Prozent)
   - Kostenangaben:
     - PV-Modul-Kosten (CHF/m²)
     - Installationskosten (CHF/m²)
     - Wechselrichter-Kosten (CHF)
   - Instandhaltungskosten (Prozent der Investitionskosten)
   - Förderbeiträge (Prozent oder CHF)
   - Strompreis (CHF/kWh)
   - Einspeisevergütung (CHF/kWh)
   - Zeitraum der Berechnung (Jahre)

---

### Ausgabe
Die Ergebnisse werden in zwei Formaten bereitgestellt: 

1. **3D-Visualisierung:**
   - Visualisierung der Verschattung auf der entsprechenden Fassade.
   
2. **Wirtschaftliche Kennzahlen:**
   --> wird in Zukunft als CSV verfügbar sein.
   - Einspeisevergütung: CHF
   - Einnahme pro Jahr: CHF
   - Stromkosteneinsparung: CHF
   - Gesamteinnahmen: CHF
   - Unterhaltskosten: CHF
   - Kosten pro Jahr: CHF
   - Gesamtkosten: CHF
   - Rendite: Prozent
   - Amortisationsdauer: Jahre
   - Stromproduktion der Fassade: kWh/a

---

### Anforderungen
- **Benötigte Software:**
  - Viktor-Plattform
- **Dateiformat:** `.3dm`
- **Internetverbindung:** Zum Abrufen von Rhino.Compute-Diensten.

---

### Haftungsausschluss
Die Berechnungen und Ergebnisse basieren auf den bereitgestellten Daten und sind nur als Informationsgrundlage gedacht. Eine Haftung für die Richtigkeit, Vollständigkeit oder Anwendbarkeit der Ergebnisse wird nicht übernommen. Entscheidungen basierend auf diesen Daten erfolgen auf eigenes Risiko.

---

### Lizenzierung
Die Berechnungen sind in einer ersten Testphase gratis zu nutzen. Um die Serverkosten auszugleichen wird in Zukunft eine kostenpflichtige Version ergänzt.

---

### Spenden
Spenden sind natürlich sehr erwünscht und können unter unserem PayPal-Account eingezahlt werden :) 
--->>>>> https://paypal.me/SamuelHenseler?country.x=CH&locale.x=de_DE

---

### Kosten-PV-Module
Monokristalline Module: Preisbereich: CHF 200 - CHF 300 pro m²

Polykristalline Module: Preisbereich: Ähnlich wie bei monokristallinen Modulen, tendenziell jedoch etwas günstiger. Sie könnten in einem Bereich von etwa CHF 150 - CHF 250 pro m² liegen.

Dünnschichtmodule: Preisbereich: CHF 100 - CHF 150 pro m². Diese Module sind im Vergleich zu kristallinen Modulen preisgünstiger, was sie für großflächige Installationen attraktiv macht.

Farbige monokristalline Module (Glas-Glas): Preisbereich: CHF 350 - CHF 450 pro m². Diese sind teurer aufgrund der ästhetischen Beschichtung und der Doppelglas-Konstruktion, die zusätzlichen Schutz und eine längere Lebensdauer bietet.

---

#### Kontakt
Bei Problemen oder Fragen:  
E-Mail: [pvplanningsyst@gmail.com](mailto:pvplanningsyst@gmail.com)  
Website: [ParametricZone](https://www.parametriczone.ch)  
