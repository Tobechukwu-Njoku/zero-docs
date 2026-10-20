# Zero-Technologies Docs

Public docs, terms and privacy policies for Zero-Technologies Discord apps. Built with Jekyll and served by GitHub Pages at https://docs.zero-technologies.co.uk.

## Before publishing

1. Set `contact_email` in `_config.yml`.
2. Search for `TODO` and fill in the retention periods and data tables.
3. Check each privacy policy matches what the app actually stores.

## Deploy

1. Create a public repo (for example `zero-docs`) and push these files to `main`.
2. Repo **Settings > Pages**: Source = **Deploy from a branch**, Branch = `main`, folder `/ (root)`.
3. At your DNS provider, add:

   | Type | Name | Value |
   |---|---|---|
   | CNAME | `docs` | `<your-github-username>.github.io` |

4. Back in **Settings > Pages**, confirm the custom domain and tick **Enforce HTTPS** once the certificate is issued.
5. Optional: verify the domain under your GitHub account **Settings > Pages** to stop anyone else claiming it.

## Discord Developer Portal URLs

| App | Terms of Service URL | Privacy Policy URL |
|---|---|---|
| Mr. Freeze | `https://docs.zero-technologies.co.uk/mr-freeze/terms/` | `https://docs.zero-technologies.co.uk/mr-freeze/privacy/` |
| Authentik | `https://docs.zero-technologies.co.uk/authentik/terms/` | `https://docs.zero-technologies.co.uk/authentik/privacy/` |

Set these under each app's **General Information** page.

## Updating a policy

Edit the page, change `last_updated` in its front matter, and commit. Git history is the change record.

## Adding an app

1. Copy the `mr-freeze` folder and rename it.
2. Update the titles, links and content.
3. Add the app to the table in `index.md` and the nav in `_layouts/default.html`.

## Preview locally (optional)

```sh
gem install bundler jekyll
jekyll serve
```
