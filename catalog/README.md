# Handbag catalog

Neue Taschen werden in `handbags.json` als Objekte innerhalb des Arrays ergänzt.
`bag-template.json` enthält die erwartete Struktur.

Pflichtfelder:

- `brand`
- `model`
- `year`
- `category`
- `size.height_cm`, `size.width_cm`, `size.depth_cm`
- `material`
- `color`
- `description`
- `price_eur`
- `image_url`

Optionale Felder:

- `price_history_eur`: erfasste Preise als Zahlenreihe, ältester Wert zuerst
- `price_change_percent`: prozentuale Preisbewegung zum letzten Vergleich
- `product_url`: offizielle Produktseite

Im offenen Admin-Panel „IT Cover“ lassen sich Produkte und Preisverläufe bearbeiten.
Die Eingaben werden zunächst nur im lokalen Browser gespeichert. Über „Katalog-JSON
exportieren“ kannst du die Änderungen herunterladen und in `handbags.json` übernehmen.
Für die produktive Nutzung ist zusätzlich eine geschützte serverseitige Speicherung nötig.

Nach dem Eintragen die lokale Website neu laden. Die Website übernimmt externe Datensätze automatisch und ergänzt Preisverlauf, Galerie und Markenlinks aus den vorhandenen Katalogdaten.
