# Landing compliance handoff — issue #2

This is a technical implementation record, not legal certification.
The public repository retains GPL-3.0 and the existing static hosting workflow.
Ongoing requirements are tracked in [landing issue #4](https://github.com/geneograph-team/geneograph-landing/issues/4).
Keep personal information, account-specific evidence, contracts, internal
decisions and confidential legal assessments in restricted records.

## Verified technical inventory

- Manrope variable TTF and OFL 1.1 are copied byte-identically from
  [Google Fonts pinned revision](https://github.com/google/fonts/tree/b31870aff700ab7a1d74fa0c6887d95beb9e0037/ofl/manrope).
  Font blob: `75274da58537d6123b14f2cd0c355ad4681fc2b3`.
  License blob: `e271172a9ed0cddc895aabb6509f1c7d880b492d`.
  The upstream metadata declares weights 200–800, Latin, Latin Extended,
  Cyrillic and Cyrillic Extended (also Greek and Vietnamese). No font modification.
  No Google Fonts stylesheet or preconnect is needed.
- No bundled JS dependencies. ResearchGroup.js uses native browser form/fetch APIs
  with Web3Forms. Existing form endpoint and access key unchanged.
- The project logo is project-created. Icons are project-created or sourced
  from [SVG Repo](https://www.svgrepo.com/); see its
  [licensing page](https://www.svgrepo.com/page/licensing/).
  Free availability does not establish permission or waive attribution.
  Verify individual terms where applicable. The EN/RU Legal pages include
  an attribution and rights reporting route; review reports and correct
  credits, replace or remove affected material as appropriate.
- PRODUCT.md identifies the Whiskerfield sample project as the screenshot
  source. Captures and sample content are project-created; third-party
  materials remain subject to applicable terms. Coordinate provenance and
  permissions with [prototype #429](https://github.com/geneograph-team/geneograph-prototype/issues/429).
  Files remain unchanged; unreferenced files are included by the current
  copy-all deployment.

- `src/prototype-albums-expanded.png` — referenced in HTML; project-created capture/content; verify applicable third-party rights.
- `src/prototype-albums.webp` — not found in HTML src/srcset references; project-created capture/content; verify applicable third-party rights.
- `src/prototype-archive-expanded.png` — referenced in HTML; project-created capture/content; verify applicable third-party rights.
- `src/prototype-archive.webp` — not found in HTML src/srcset references; project-created capture/content; verify applicable third-party rights.
- `src/prototype-family-tree-hero.png` — referenced in HTML; project-created capture/content; verify applicable third-party rights.
- `src/prototype-family-tree.webp` — referenced in HTML; project-created capture/content; verify applicable third-party rights.
- `src/prototype-geneograph-household.png` — referenced in HTML; project-created capture/content; verify applicable third-party rights.
- `src/prototype-geneograph.webp` — not found in HTML src/srcset references; project-created capture/content; verify applicable third-party rights.
- `src/prototype-notes-daisy.png` — referenced in HTML; project-created capture/content; verify applicable third-party rights.
- `src/prototype-notes.webp` — not found in HTML src/srcset references; project-created capture/content; verify applicable third-party rights.
- `src/prototype-people-profile-updated.png` — referenced in HTML; project-created capture/content; verify applicable third-party rights.
- `src/prototype-people-profile.webp` — not found in HTML src/srcset references; project-created capture/content; verify applicable third-party rights.

## Shared website and demo notices

The EN/RU Legal pages cover the website and interactive demo. The
`src/third-party-licenses/` directory contains byte-identical copies of the
prototype's nine primary library license files and map-style license notice.
The prototype retains its original distributed license files. When updating a
prototype vendor version, reconcile the published component index and copied
license text with the corresponding original. Keep upstream notices intact.
The landing owns user-facing privacy and license content; the demo links to
its localized sections. Publish landing changes before dependent demo updates.

## Privacy and service evidence (reviewed 26 Nov 2026)

- [GDPR Articles 6, 13 and 15–22](https://eur-lex.europa.eu/eli/reg/2016/679/oj):
  controller identity, legal basis, retention, recipients/transfers, rights and
  complaint route must be established for actual processing.
- [Web3Forms terms](https://web3forms.com/terms), [privacy](https://web3forms.com/privacy)
  and [DPA](https://web3forms.com/dpa) describe service processing, retention,
  subprocessors and applicable international transfer terms. Verify the actual
  processing arrangements and retain supporting account evidence privately.
  Public privacy notices describe the service's role and current data flows.
- [GitHub Pages documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages)
  explains IP logging. [Hosting limits](https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits)
  restrict online-business/e-commerce/SaaS use. Review suitability before
  commercial launch; no hosting migration in this issue.
- Prototype data flows reviewed from pushed default
  `db987a97e323a69043d2314a7314fe9272e4d998`: local in-memory research,
  persisted preferences, Quill/jsDelivr, MapLibre/unpkg, OpenFreeMap map tiles,
  Geoapify → LocationIQ place queries and user-triggered MyHeritage photo fetches
  from supported GEDCOM links. See prototype #430 and PR #433.
- [Geoapify privacy](https://www.geoapify.com/privacy-policy/),
  [LocationIQ privacy](https://locationiq.com/privacy),
  [OpenFreeMap privacy](https://openfreemap.org/privacy/) reviewed as public
  provider references, not account-specific agreements.
- Landing source contains no analytics or tracking cookie/storage code. Actual
  browser and hosting behavior still needs verification. No cookie banner added
  absent a demonstrated requirement.

## Ongoing requirements

Track the following in landing issue #4 and applicable prototype issues.

- Verify legally required controller identity and contact disclosures, lawful
  bases, rights and complaint mechanisms, recipients, retention and transfer
  safeguards in both Legal page privacy sections.
- Verify processor/service terms, security, retention/deletion and consent
  and withdrawal processes for hosting, forms, email and optional demo
  services. Retain private agreements and verification evidence separately.
- Maintain asset provenance, required credits and rights-report handling.
  Resolve applicable licensing questions without publishing private evidence.
- Keep the distributed GPL text byte-identical to the root license and verify
  corresponding source access for each deployed revision. Obtain specific
  approval for any required deployment-workflow change.
- Reassess applicable privacy, distribution and hosting requirements when
  services, product features or release scope change. Obtain appropriate legal
  review where necessary.

## QA pending

Test all six primary pages in both languages and the legacy legal URL redirects
in a real browser at mobile/desktop widths; check keyboard, font loading, network/storage,
local license/source paths and form validation/success/error using controlled
test data. Do not send unsolicited submissions. Verify exact deployed artifact
and links after publication. Record results in the technical tracker.
