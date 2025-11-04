# Die wichtigsten Watchtower Parameter im Überblick

| Variable                             | Beschreibung                                               |
| ------------------------------------ | ---------------------------------------------------------- |
| `WATCHTOWER_CLEANUP=true`            | Alte Images werden gelöscht                                |
| `WATCHTOWER_LABEL_ENABLE=true`       | Nur Container mit Label werden überwacht                   |
| `WATCHTOWER_INCLUDE_RESTARTING=true` | Auch Container im Neustart-Prozess werden berücksichtigt   |
| `WATCHTOWER_SCHEDULE=0 0 4 * * *`    | Tägliches Update um 4:00 Uhr (Go-Cron!)                    |
| `WATCHTOWER_LIFECYCLE_HOOKS=true`    | Aktiviert pre- & post-update Hooks                         |
| `WATCHTOWER_MONITOR_ONLY=false`      | Wenn auf `true`, wird nichts aktualisiert – nur beobachtet |
| `WATCHTOWER_NOTIFICATIONS=shoutrrr`  | Aktiviert Benachrichtigungen                               |
| `WATCHTOWER_NOTIFICATION_URL=...`    | Ziel-URL für Shoutrrr-Dienste                              |

# Watchtower Schedule Beispiele

| Ausdruck         | Bedeutung                 |
| ---------------- | ------------------------- |
| `0 0 4 * * *`    | Täglich um 4:00 Uhr früh  |
| `0 0 3 * * 0`    | Jeden Sonntag um 3:00 Uhr |
| `0 */15 * * * *` | Alle 15 Minuten           |
| `0 0 */6 * * *`  | Alle 6 Stunden            |
| `0 30 2 * * 1-5` | Mo–Fr um 2:30 Uhr nachts  |
