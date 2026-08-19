# flechaamarilla.org

Static one-page site for **Flecha Amarilla, Inc.**, a Texas nonprofit corporation
(501(c)(3), EIN 42-3820188).

Its jobs, in order of importance:

1. Establish publicly that flechaamarilla.org and crghouston.org both belong to
   Flecha Amarilla, Inc. — required for Google for Nonprofits domain verification,
   and matched by the "Legal information for donors" section of crghouston.org/support-us.
2. Give the domain a legitimate destination, since all CRG outbound mail sends from
   `crg@flechaamarilla.org`.

## Structure

Plain static HTML. No framework, no build step.

- `index.html` — the whole site, styles inline in a `<style>` block
- `crg-logo.png` — 128px copy of the CRG logo (the source is a 1 MB 1024px PNG)

## Deploy

Cloudflare Pages. Build command: none. Output directory: `/` (repo root).

DNS lives at **Namecheap**, not Cloudflare — deliberately. The domain carries live
Google Workspace mail (MX, SPF, DKIM, and a google-site-verification TXT), so the
nameservers are left alone and the domain points at Pages via a single DNS record.

## Editing

The EIN, mailing address, and 501(c)(3) language are legal facts reproduced from
crghouston.org/support-us. If one changes, change it in **both** places.
