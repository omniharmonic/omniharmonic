# Import report: omniharmonic

Imported from https://www.omniharmonic.com (Squarespace 7.1) on 2026-10-28 with `openspace import squarespace`.
Sources: page HTML and the sitemap, Squarespace's `?format=json` data (owner mode). 37 requests.

## Summary

- **4** pages, **0** collection items in 0 collection(s)
- **21** media files (4.2 MB) downloaded into `media/`
- **1** redirects so old addresses keep working
- **9** item(s) need your attention (below)

## Pages

| Squarespace | OpenSpace | Title | Sections | Blocks |
| --- | --- | --- | ---: | ---: |
| `/` | `/` | Home | 11 | 27 |
| `/about` | `/about` | about | 5 | 10 |
| `/research` | `/research` | research | 1 | 9 |
| `/art` | `/art` | art | 2 | 5 |

## Design

The look was recreated with OpenSpace's own design system (Site Styles tokens, section color themes, layouts and section presets), not by copying Squarespace's template CSS or code.

- Brand color #0f3a48 (Squarespace "accent" color).
- Fonts on Squarespace: Instrument Serif / Public Sans → pairing "Instrument Serif & Instrument Sans" (Instrument Serif / Instrument Sans), same family for Instrument Serif. Licensed fonts can be uploaded in Site Styles → Fonts.
- Type scale on Squarespace: Heading 1 is 8.6× body text (very large; OpenSpace's display preset is the nearest). Density "comfortable" from the section heights.
- Fonts on Squarespace kept as they are (Instrument Serif, Public Sans): free on Google Fonts, self-hosted with the site.
- Type scale on Squarespace (the live site, measured in a browser) kept: display 137px/91.6px, heading 1 137px/91.6px, heading 2 19.5px/18.2px, body 16px/16px.
- Page rhythm on Squarespace (the live site, measured in a browser): sections padded 55px (55px on phones) — kept in Site Styles.
- Page background #ffffff on Squarespace → #fafafa (text contrast 15.6:1).

Design check: 9 error(s), 16 warning(s).

- **error** (/): Two text blocks (text and text) overlap on desktop, so neither can be read properly.
- **error** (/): Two text blocks (text and text) overlap on desktop, so neither can be read properly.
- **error** (/): Two text blocks (text and text) overlap on desktop, so neither can be read properly.
- **error** (/): Two text blocks (text and text) overlap on desktop, so neither can be read properly.
- **error** (/): Two text blocks (text and text) overlap on desktop, so neither can be read properly.
- **error** (/): Two text blocks (text and text) overlap on desktop, so neither can be read properly.
- **error** (/): Two text blocks (text and text) overlap on mobile, so neither can be read properly.
- **error** (/): A text block is completely covered by a image on mobile, so visitors can't see it.
- **error** (/): A text block is completely covered by a image on mobile, so visitors can't see it.
- warning (/): A text block sits directly on a photo on desktop, where busy areas make it hard to read.
- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): “Together, we can” jumps from Heading 1 to Heading 4, skipping a level.
- … and 13 more: run Design check in Studio or `design_check` with Claude.

## Needs attention

### Blocks that need a look

- Squarespace "scrolling" block has no direct OpenSpace equivalent; its text was kept as a text block. _(/)_

### Links

- Link to /cdn-cgi/l/email-protection led to a page that wasn't imported; it now points at the home page. Point it at the right page. _(/)_
- Text link to /digital-products-2-1 led to a page that wasn't imported; the link was removed. _(footer)_
- Text link to /portfolio-3 led to a page that wasn't imported; the link was removed. _(footer)_

### Design

- A photo section's overlay was darkened from 15% to 70% so its text stays readable. _(/)_
- A photo section's overlay was darkened from 15% to 60% so its text stays readable. _(/)_
- A photo section's overlay was darkened from 15% to 45% so its text stays readable. _(/art)_

### Other

- The page had no Heading 1; its first heading was made the Heading 1 (search engines and screen readers use it). _(/, /research, /art)_

## Redirects

Saved in `content/site.json` (`redirects`), published with the site:

| From | To |
| --- | --- |
| `/home` | `/` |

## Not moved by the importer

- Orders, customers, inventory, discounts, gift cards, shipping and tax settings (commerce stays in Squarespace until you switch).
- Newsletter subscribers, form submissions, member accounts and blog comments.
- Scheduling (Acuity), donations, digital-download files and anything behind a login.
- Squarespace analytics and SEO history (search engines follow the redirects).

## Next steps

1. `npm install`, then `npx openspace check` (it should report no errors) and `npx openspace dev` to look around.
2. Bring it to visual parity with Claude: in this folder run `claude`, then `/openspace:import-squarespace` (or ask Claude to compare each page with the original). It screenshots both sites at desktop and mobile and adjusts presets, Site Styles and sections — never raw HTML.
3. Fix the items under **Needs attention**, then publish (push to GitHub, or `publish` with Claude).
4. Move the domain only after the new site is live and checked:
   - add the custom domain in OpenSpace (`deploy.customDomain` in `openspace.json`, or the Hub);
   - at your DNS provider (Squarespace Domains or elsewhere), point the records at the new host as the domain guide says (GitHub Pages: `A`/`CNAME` records; Cloudflare: the Pages project's records);
   - keep the Squarespace subscription until the new site serves your domain over HTTPS and the redirects work; then cancel it (and transfer the domain away from Squarespace if you like).

