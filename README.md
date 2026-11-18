# justtapapps.com

Website for Just Tap Apps LLC. Plain HTML and CSS, no build step. Whatever is on `main` is live at https://justtapapps.com.

## Pages

| File | Page |
|---|---|
| `index.html` | Home |
| `apps.html` | Our Apps (Snooze Bully featured; Atlas Noches and Travel Shakeup shown as "In development") |
| `about.html` | About |
| `contact.html` | Contact and support |
| `privacy.html` | Privacy Policy |
| `terms.html` | Terms of Service |
| `delete-account.html` | Account deletion (required by Google Play) |
| `disclaimer.html` | Disclaimer |
| `style.css` | Shared styles for every page |

Images: `logo-icon.png`, `hero.jpg`, `snooze-bully.png`, `atlas-noches.png`, `travel-shakeup.png`.

Every page has a strict Content-Security-Policy meta tag: only same-site styles and images, no scripts, no outside fonts, no forms.

## Hosting

- **GitHub Pages:** deploys from `main`, `/ (root)`. Settings: https://github.com/travel-shakeup/justtapapps-site/settings/pages
- **Deploy status:** https://github.com/travel-shakeup/justtapapps-site/actions (green check = live)
- **Custom domain:** the `CNAME` file holds `justtapapps.com`. Do not delete it.
- **`.nojekyll`:** tells GitHub to serve files as they are.
- **HTTPS:** certificate issued by GitHub Pages; "Enforce HTTPS" on.

## Domain and DNS (Squarespace)

Domain registered at Squarespace (via Google Workspace). Private Registration and Domain Lock are on.

Records pointing the site at GitHub:

| Type | Name | Data |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | travel-shakeup.github.io |

Leave the email records alone: MX (Google Workspace), SPF, DKIM, DMARC and the Resend records.

## Links for store listings

- Privacy policy: https://justtapapps.com/privacy.html
- Account deletion: https://justtapapps.com/delete-account.html
- Support: support@justtapapps.com

## To do

- [ ] When Snooze Bully is on Google Play, replace "Coming soon to Google Play" in `apps.html` with a real store link.
- [ ] When Atlas Noches or Travel Shakeup launches: restore its full card in `apps.html`, add its sections back to `disclaimer.html` and `privacy.html`, and mention it in the meta descriptions in `index.html` and `apps.html`.
- [ ] Before any iPhone launch, update the Google Play-specific wording (subscriptions, refunds, cancellation) in `terms.html`, `privacy.html` and `delete-account.html`.
