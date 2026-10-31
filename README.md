# Flirtly

Flirtly ist ein einfacher, responsiver KI-Chatpartner für natürliches Schreiben, Flirten, ernste Gespräche und erwachsene Dirty-Talk-Szenarien.

## Funktionen
- Automatische Erkennung der Sprache und Antworten in derselben Sprache
- Kurze, natürliche Antworten statt langer KI-Monologe
- Modi für natürliches Chatten, Flirten, freche, romantische oder ernste Gespräche, erwachsenen Dirty Talk, Rollenspiel und Coaching
- Mobilfreundlicher Chat mit lokalem Verlauf, Chat kopieren und neu starten
- OpenRouter-Anbindung ausschließlich serverseitig über eine Supabase Edge Function
- Der OpenRouter-Key liegt nicht im Frontend

## Backend
Supabase-Projekt: KDS AI (`eopvkwhcgznvubesaszv`).

Die Edge Function `flirt-ai` liest das vorhandene Supabase Secret `flirt_ai`. Als Alternativen werden `OPENROUTER_API_KEY` und `AI_API_KEY` unterstützt. Optional kann `FLIRT_AI_MODEL` oder `AI_MODEL` gesetzt werden; Standardmodell ist `openrouter/free`.

Das Secret darf niemals in HTML, JavaScript oder GitHub gespeichert werden. Sexuelle Gespräche sind auf eindeutig einvernehmliche Erwachsene beschränkt.

## Hosting
GitHub Pages veröffentlicht den `main`-Branch aus dem Root-Verzeichnis unter:
https://lordlolqdh.github.io/flirt-ai/
