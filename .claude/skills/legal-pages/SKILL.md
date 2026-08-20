---
name: legal-pages
description: Edit the static legal pages (privacy policy, terms of service) for Naru while keeping their URLs stable. Use when updating legal text, privacy/terms content, or the legal site — guards the stable paths referenced by App Store Connect and ad reviews.
---

# Legal-Pages (naruhodo-legal)

Reines statisches HTML, kein Build. Dateien direkt editieren:

```
/privacy-policy/index.html
/terms-of-service/index.html
/index.html
/CNAME
```

## Harte Regeln

- **Pfade nicht ändern:** `/privacy-policy` und `/terms-of-service` sind in App Store Connect und in TikTok/Meta-Ad-Reviews verlinkt. Umbenennen/Verschieben bricht externe Referenzen.
- Beim Texten: nur Inhalt der `<body>`-Sektion ändern, Struktur/Slugs lassen.
- **Hosting-Vorsicht:** `CNAME` = `naru-app.com` — dieselbe Domain wie `naru-web`. Vor CNAME-/DNS-Änderungen klären, welches Repo die Domain bedient. Nicht blind ändern.

## Nach Änderung

Live-URLs prüfen (200 + korrekter Inhalt) bevor als erledigt gemeldet wird.
