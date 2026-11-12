# MyChat

MyChat gehört zum MyDigital-System und verwendet dieselbe Supabase-Anmeldung.

## Version 1 – aktueller Funktionsumfang
- Anmeldung mit vorhandenem MyDigital-Konto
- Suche nach Benutzernamen
- Kontaktanfragen senden, annehmen und ablehnen
- Private Einzelchats zwischen bestätigten Kontakten
- Nachrichten in Echtzeit
- Dunkles, responsives Layout und installierbare PWA-Grundlage
- Datenbankzugriff über Row Level Security (RLS)

## Datenbank
Die Tabellen und Sicherheitsregeln wurden im gemeinsamen MyDigital-Supabase-Projekt über die Migrationen `mychat_v1_core`, `mychat_v1_access_hardening` und `mychat_v1_minimum_table_grants` eingerichtet. Die Datei `supabase/schema.sql` dokumentiert den Aufbau; sie ist keine zweite Migration zum erneuten Ausführen.

## Noch nicht enthalten
Gruppenchats, Bilder- und Dateianhänge, Online-Status, Schreibanzeige und Push-Benachrichtigungen folgen in späteren Versionen.

## Offline
Die PWA kann ihre App-Oberfläche zwischenspeichern. Anmeldung, Kontaktsuche und Nachrichten benötigen weiterhin eine Internetverbindung.
