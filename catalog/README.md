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

Nach dem Eintragen die lokale Website neu laden. Die Website übernimmt externe Datensätze automatisch und ergänzt Preisverlauf, Galerie und Markenlinks aus den vorhandenen Katalogdaten.
