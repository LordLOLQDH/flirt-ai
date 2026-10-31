# Flirt AI

Eine responsive, deutschsprachige Flirt-KI mit GitHub Pages als Frontend und KDS-AI-Supabase als Backend.

## Funktionen
- Flirt-Coach, Nachrichtenhilfe, Antwortideen, Date-Vorschläge und Rollenspiel
- Wählbare Persönlichkeit, Ziel und Gesprächsstil
- Mobilfreundlicher Chat, Vorschläge, Chat kopieren und lokal gespeicherter Verlauf
- OpenRouter-Anbindung ausschließlich serverseitig über eine Supabase Edge Function
- Kein API-Key im Frontend

## Backend einrichten
Supabase-Projekt: KDS AI (`eopvkwhcgznvubesaszv`).

In Supabase → Edge Functions → Secrets ein Secret hinzufügen:
- Name: `OPENROUTER_API_KEY`
- Wert: der selbst erstellte OpenRouter API-Key

Optional kann `FLIRT_AI_MODEL` als Secret gesetzt werden. Standard ist `openrouter/free`.

Die Edge Function `flirt-ai` verarbeitet die Anfrage und ruft OpenRouter serverseitig auf. Niemals den OpenRouter-Key in HTML, JavaScript oder GitHub speichern.

## Hosting
Aktiviere in GitHub unter Settings → Pages die Veröffentlichung aus dem `main`-Branch und dem Root-Verzeichnis. Die Website wird dann unter https://lordlolqdh.github.io/flirt-ai/ erreichbar sein.
