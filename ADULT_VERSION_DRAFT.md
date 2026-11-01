# Flirtly 18+ — Entwicklungsentwurf

**NICHT ÖFFENTLICH FREIGEBEN.** Diese Arbeit liegt auf dem Branch `adult-v1-draft`; die bestehende Teen-Version auf `main` bleibt unverändert.

## Dateien
- `index.html`: 18+-Selbstauskunfts-Prototyp. Kein Altersnachweis; nach Bestätigung bleibt der Chat absichtlich gesperrt.
- `agb.html`, `datenschutz.html`, `impressum.html`, `cookies.html`, `jugendschutz.html`: Rechtsseiten als Entwürfe mit Platzhaltern.

## Startblocker
1. Tatsächlichen rechtlichen Betreiber und zustellfähige Anschrift festlegen.
2. Fachlich/juristisch klären, ob und welche Altersverifikation erforderlich ist.
3. Eigenes Backend und separate Supabase-Umgebung einrichten. Teen-Endpunkt nicht für Erwachsenen-Inhalte wiederverwenden.
4. Serverseitige Zugriffskontrolle und Inhaltsmoderation umsetzen; eine Checkbox ist leicht umgehbar.
5. KI-Anbieter, Hosting, Logs, Speicherfristen, Drittlandtransfers und alle weiteren Datenflüsse erfassen.
6. Cookies und Local Storage auditieren; Consent-Manager nur passend zum tatsächlichen Einsatz integrieren.
7. Rechtsseiten qualifiziert prüfen lassen.
8. Meldeweg, Löschkonzept und Sicherheits-/Missbrauchsreaktion einrichten.
9. Sicherstellen, dass die bestehende Teen-Version unverändert und altersgerecht bleibt.

Keine API-Geheimnisse ins Frontend. Ein Git-Branch ist kein Sicherheitsmechanismus und die Alterscheckbox ist keine Altersverifikation.
