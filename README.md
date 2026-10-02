# Runway Studio site

Static site for Runway Studio, served at https://www.runwaystudio.ph. No build step: `index.html`, self-hosted fonts in `fonts/`, a favicon and a share-preview image (`og.png`).

## Hosting (GitHub Pages)

- Repo Settings > Pages: deploy from branch `main`, folder `/ (root)`.
- Custom domain: `www.runwaystudio.ph` (the `CNAME` file declares it). The bare domain redirects to `www`.
- DNS at Namecheap (Advanced DNS > Host Records), web records only:
  - `A` record, host `@`: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153 (four records)
  - `CNAME` record, host `www`: `gerome650.github.io`
- Mail records live under Mail Settings on the same page and are separate from the web records.
- Enforce HTTPS is switched on once GitHub has issued the certificate.

## Open items

- Image slots (Films, Key visuals, Series, Scene generation) show placeholders until stills are supplied.

## Fonts

Inter, Inter Tight and Geist Mono, all under the SIL Open Font License.
