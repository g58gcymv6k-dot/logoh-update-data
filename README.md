# log p-h Studio – Update-Spiegel

Dieses öffentliche Repository stellt die Referenz- und Update-Dateien für die lokale Offline-ZIP bereit.

- `reference-points.json`: feste Prüfpunkte für die manuell ausgelöste Aktualitätsprüfung
- `update-manifest.json`: Downloadpfade und SHA-256-Prüfsummen
- `fluid-data.js`: lokale Kältemittel-Fallback-Tabelle
- `secondary-data.js.gz.b64`: komprimierte Sekundärmedium-Tabelle
- `vendor/coolprop/coolprop.js`: CoolProp-JavaScript-Datei
- `vendor/coolprop/coolprop.wasm.gz.b64.part00` bis `part06`: komprimierte WASM-Datei in Teilstücken

Die Offline-ZIP ruft die Dateien über `raw.githubusercontent.com` ab. Große Dateien werden im Browser zusammengesetzt, entpackt und danach gegen die SHA-256-Prüfsumme der Originaldatei geprüft. Die Online-Site bleibt unverändert und nutzt Same-Origin-Dateien.

Nach jeder Änderung an einer angebotenen Datei müssen die SHA-256-Werte im Manifest aktualisiert werden.
