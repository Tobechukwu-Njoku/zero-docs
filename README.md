# Zero-Technologies Docs

Public docs, terms and privacy policies for Zero-Technologies Sign-in and Discord apps. Built with Jekyll and served by GitHub Pages at https://docs.zero-technologies.co.uk.

## Before publishing

Check each privacy policy still matches what the service stores, and bump `last_updated`.

## Deploy

1. Create a public repo (for example `zero-docs`) and push these files to `main`.
2. Repo **Settings > Pages**: Source = **Deploy from a branch**, Branch = `main`, folder `/ (root)`.
3. At your DNS provider, add:

   | Type | Name | Value |
   |---|---|---|
   | CNAME | `docs` | `tobechukwu-njoku.github.io` (Cloudflare: DNS only, grey cloud) |

4. Back in **Settings > Pages**, confirm the custom domain and tick **Enforce HTTPS** once the certificate is issued.
5. Optional: verify the domain under your GitHub account **Settings > Pages** to stop anyone else claiming it.

## URLs for provider settings

| Where | Terms of Service URL | Privacy Policy URL |
|---|---|---|
| Discord app Victor Fries | `https://docs.zero-technologies.co.uk/victor-fries/terms/` | `https://docs.zero-technologies.co.uk/victor-fries/privacy/` |
| Discord sign-in app, Google consent screen, Microsoft branding | `https://docs.zero-technologies.co.uk/sign-in/terms/` | `https://docs.zero-technologies.co.uk/sign-in/privacy/` |
| Zero-Technologies Cloud (Nextcloud): link from the login page and footer | `https://docs.zero-technologies.co.uk/cloud/terms/` | `https://docs.zero-technologies.co.uk/cloud/privacy/` |
| Databasus Google OAuth app (Drive storage, Google sign-in) | `https://docs.zero-technologies.co.uk/databasus/terms/` | `https://docs.zero-technologies.co.uk/databasus/privacy/` |

Google also needs a home page (`https://docs.zero-technologies.co.uk/sign-in/`, or `/databasus/` for the Databasus app) and the authorised domain `zero-technologies.co.uk`.

## Updating a policy

Edit the page, change `last_updated` in its front matter, and commit. Git history is the change record.

## Adding an app

1. Copy the `victor-fries` folder and rename it.
2. Update the titles, links and content.
3. Add the app to the table in `index.md` and the nav in `_layouts/default.html`.

## Preview locally (optional)

```sh
gem install bundler jekyll
jekyll serve
```
