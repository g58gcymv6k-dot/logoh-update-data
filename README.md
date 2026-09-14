# log p-h Studio – Update-Spiegel

Dieses öffentliche Repository stellt die Referenz- und Update-Dateien für die lokale Offline-ZIP bereit.

- `reference-points.json`: feste Prüfpunkte für die manuell ausgelöste Aktualitätsprüfung
- `update-manifest.json`: Downloadpfade und SHA-256-Prüfsummen
- `fluid-data.js` und `secondary-data.js`: lokale Fallback-Tabellen
- `vendor/coolprop/`: gebündelte CoolProp-JavaScript-/WASM-Dateien

Die Offline-ZIP ruft die Dateien über `raw.githubusercontent.com` ab. Die Online-Site bleibt unverändert und nutzt Same-Origin-Dateien.

Nach jeder Änderung an einer angebotenen Datei müssen die SHA-256-Werte im Manifest aktualisiert werden.
