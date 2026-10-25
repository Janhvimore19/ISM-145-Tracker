# ISM 145 Tracker Launcher

This is a static GitHub Pages launcher. It contains no employee records, passwords, leave requests, or database.

## First-time configuration

Edit `config.js` and replace:

- `PRIMARY-HOST-IP` with the Primary TL laptop's office IPv4 address
- `SECONDARY-HOST-IP` with the Secondary TL laptop's office IPv4 address
- `EMERGENCY-HOST-IP` with Janhvi's office IPv4 address

Set the active host:

```js
activeHost: "primary"
```

Allowed values are `primary`, `secondary`, or `emergency`.

Update the audit text:

```js
updatedBy: "Kirtan Shetty",
updatedAt: "25 Oct 2026, 9:00 AM"
```

## When changing hosts

1. Stop the old host.
2. Move the latest `ism145.db` to the new host.
3. Start the new host.
4. Edit only `config.js` on GitHub.
5. Change `activeHost` to the new host.
6. Update `updatedBy` and `updatedAt`.
7. Commit the change.

The public GitHub Pages URL remains the same.

## Important

- Only one tracker host may be active at a time.
- GitHub Pages is only the launcher, not the database or Python host.
- Do not upload `ism145.db`, employee files, passwords, or leave data to this repository.
- The tracker remains reachable only from networks allowed to reach the active host laptop.
