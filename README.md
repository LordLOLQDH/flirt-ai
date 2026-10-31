# Flirt AI

Eine responsive, deutschsprachige Flirt-KI mit GitHub Pages als Frontend und KDS-AI-Supabase als Backend.

## Funktionen
- Flirt-Coach, Nachrichtenhilfe, Antwortideen, Date-Vorschläge und Rollenspiel
- Wählbare Persönlichkeit, Ziel und Gesprächsstil
- Mobilfreundlicher Chat, Vorschläge, Chat kopieren und lokal gespeicherter Verlauf
- OpenRouter-Anbindung ausschließlich serverseitig über eine Supabase Edge Function
- Kein API-Key im Frontend

## Backend
Supabase-Projekt: KDS AI (`eopvkwhcgznvubesaszv`).

Die Edge Function `flirt-ai` liest das vorhandene Supabase Secret `flirt_ai`. Als kompatible Alternativen werden `OPENROUTER_API_KEY` und `AI_API_KEY` unterstützt. Optional kann `FLIRT_AI_MODEL` oder `AI_MODEL` gesetzt werden; Standardmodell ist `openrouter/free`.

Der OpenRouter-Key bleibt serverseitig und darf niemals in HTML, JavaScript oder GitHub gespeichert werden.

## Hosting
Aktiviere in GitHub unter Settings → Pages die Veröffentlichung aus dem `main`-Branch und dem Root-Verzeichnis. Die Website ist dann unter https://lordlolqdh.github.io/flirt-ai/ erreichbar.
