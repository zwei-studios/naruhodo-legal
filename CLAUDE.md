# naruhodo-legal

Statische **Legal-Pages** (Privacy Policy, Terms of Service) für Naru. Reines HTML, kein Build.

```
/index.html                  Übersicht / Redirect
/privacy-policy/index.html
/terms-of-service/index.html
/CNAME                        Custom Domain (aktuell: naru-app.com)
```

## Harte Regeln

- Diese URLs sind in **App Store Connect** und **TikTok/Meta-Ad-Reviews** verlinkt → Pfade `/privacy-policy` und `/terms-of-service` **stabil halten**, nicht umbenennen.
- ⚠️ `CNAME` zeigt auf `naru-app.com` — dieselbe Domain wie `naru-web`. Vor Hosting-/DNS-Änderungen klären, welches Repo `naru-app.com` tatsächlich bedient (Konflikt-Potenzial). Nicht blind die CNAME ändern.

## Skills (scoped)

- `legal-pages` — Legal-Texte bearbeiten unter Wahrung stabiler URLs + Hosting-Hinweis.
