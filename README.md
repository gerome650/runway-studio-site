# Runway Studio site

Static site for Runway Studio. No build step: `index.html`, self-hosted fonts in `fonts/`, and a favicon. All paths are relative, so it works both at a `github.io/<repo>/` address and at a custom domain.

## Deploy (GitHub Pages)

1. Repo Settings > Pages > Build and deployment: deploy from branch `main`, folder `/ (root)`.
2. Until a domain is attached the site is served at `https://<github-user>.github.io/<repo>/`.
3. When the domain is chosen: add a `CNAME` file containing `www.<domain>`, set the same value as the custom domain in Pages (before changing DNS), then at the registrar:
   - `A` record for `@`: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - `CNAME` for `www`: `<github-user>.github.io`
4. Once the certificate is issued, tick Enforce HTTPS.

## Open items

- Contact address on the page is a stand-in until the new domain has a mailbox.
- Image slots (Films, Key visuals, Series, Scene generation) show placeholders until stills are supplied.

## Fonts

Inter, Inter Tight and Geist Mono, all under the SIL Open Font License.
