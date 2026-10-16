# Privora Platform (legacy cloud services)

Account, billing, hosted-model and update-feed implementation extracted with history from [privora-desktop](https://github.com/MohammedSafwan10/privora-desktop). Privora Desktop is BYOK-only and no longer needs these account or credit services. This extraction does not deploy code or delete existing cloud resources.

- `apps/web/`: previous account/billing website.
- `appwrite/functions/`: model gateway and desktop update feed.
- `appwrite/scripts/`: credit administration.
- `appwrite.config.json`: previous site configuration.
- `docs/desktop-auto-updates.md`: update-feed operations.

Run `npm --prefix apps/web ci`, then `npm run web:dev`, `npm run web:lint`, or `npm run web:build`. Keep all private credentials outside Git. Existing live deployments remain unchanged until deliberately migrated.
