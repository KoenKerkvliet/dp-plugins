# DP Plugins — update-kanaal

Distributie van de Design Pixels-plugins (DP Toolbox, DP Analytics, DP Cookie Consent,
DP Webshop). Dit is geen broncode-repo: hier staan alleen de release-ZIP's en de
ondertekende versielijst.

- `manifest.json` — versielijst. Het veld `data` is ondertekend met Ed25519
  (`signature`, sleutel-id in `key`). DP Toolbox accepteert de lijst alleen met een
  geldige handtekening, en een ZIP alleen als zijn sha256 in die lijst staat.
- `zips/<slug>/<slug>-<versie>.zip` — de laatste vijf versies per plugin.

Wordt bijgewerkt door `publish.py` (lokaal, niet in deze repo). Handmatig wijzigen
heeft geen zin: zonder geldige handtekening negeren de sites de lijst.
