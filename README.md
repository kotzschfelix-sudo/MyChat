# MyChat

MyChat gehört zum MyDigital-System und verwendet dieselbe Supabase-Anmeldung.

## Version 1
- Anmeldung mit vorhandenem MyDigital-Konto
- Suche nach Benutzernamen
- Kontaktanfragen senden, annehmen und ablehnen
- Private Einzelchats
- Nachrichten in Echtzeit
- Dunkles, responsives Layout und installierbare PWA-Grundlage

## Datenbank
Die Migration `supabase/schema.sql` erstellt Kontaktanfragen, Blockierungen, Chats, Chat-Mitgliedschaften und Nachrichten. Row Level Security schützt Chat-Inhalte. Die Funktion `create_direct_chat` erlaubt einen privaten Chat nur zwischen bestätigten Kontakten.

## Noch nicht enthalten
Gruppenchats, Anhänge, Online-Status, Schreibanzeige und Push-Benachrichtigungen werden in späteren Versionen ergänzt.

## Offline
Die PWA kann ihre App-Oberfläche zwischenspeichern. Anmeldung, Kontaktsuche und Nachrichten benötigen weiterhin eine Internetverbindung.
