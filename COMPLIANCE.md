# Landing compliance handoff — issue #2

This is an implementation record and review checklist, not legal certification.
The current public GPL-3.0 repository and GitHub Pages research site are retained.
The proposal does not modify hosting, licensing grants, or provider accounts.

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
- Inline SVGs: icon provenance not established; confirm original icon sources
  and permission notices. Logo: confirm ownership and any third-party elements.
  Do not infer copyright ownership from repository location.
- Screenshots: PRODUCT.md identifies the Whiskerfield sample project as the
  source. Files below remain unchanged; specific capture revision, permissions
  for visible underlying media and icon credits remain to be confirmed using
  [prototype #429](https://github.com/geneograph-team/geneograph-prototype/issues/429). Unreferenced files remain shipped
  by the current copy-all deployment; no binary removed.

- `src/prototype-albums-expanded.png` — referenced in HTML; provenance/rights pending.
- `src/prototype-albums.webp` — not found in HTML src/srcset references; provenance/rights pending.
- `src/prototype-archive-expanded.png` — referenced in HTML; provenance/rights pending.
- `src/prototype-archive.webp` — not found in HTML src/srcset references; provenance/rights pending.
- `src/prototype-family-tree-hero.png` — referenced in HTML; provenance/rights pending.
- `src/prototype-family-tree.webp` — referenced in HTML; provenance/rights pending.
- `src/prototype-geneograph-household.png` — referenced in HTML; provenance/rights pending.
- `src/prototype-geneograph.webp` — not found in HTML src/srcset references; provenance/rights pending.
- `src/prototype-notes-daisy.png` — referenced in HTML; provenance/rights pending.
- `src/prototype-notes.webp` — not found in HTML src/srcset references; provenance/rights pending.
- `src/prototype-people-profile-updated.png` — referenced in HTML; provenance/rights pending.
- `src/prototype-people-profile.webp` — not found in HTML src/srcset references; provenance/rights pending.

## Privacy and service evidence (reviewed 26 Nov 2026)

- [GDPR Articles 6, 13 and 15–22](https://eur-lex.europa.eu/eli/reg/2016/679/oj):
  controller identity, legal basis, retention, recipients/transfers, rights and
  complaint route must be established for actual processing.
- [Web3Forms terms](https://web3forms.com/terms), [privacy](https://web3forms.com/privacy)
  and [DPA](https://web3forms.com/dpa), updated 13 Jul 2026: the published DPA
  applies to customer form submissions; operator Web3Creative processes for
  the customer, operates from India and describes SCCs and a three-year
  physical retention window, with plan-dependent visibility. Annex 3 names
  infrastructure/anti-spam subprocessors and optional integrations require
  separate review. The actual account, acceptance, transfers, deletion,
  optional integrations and mailbox operation are not verified.
- [GitHub Pages documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages)
  explains IP logging. [Hosting limits](https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits)
  restrict online-business/e-commerce/SaaS use. Review suitability before
  commercial launch; no hosting migration in this issue.
- Prototype data flows reviewed from pushed default
  `db987a97e323a69043d2314a7314fe9272e4d998`: local in-memory research,
  persisted preferences, Quill/jsDelivr, MapLibre/unpkg, OpenFreeMap map tiles,
  Geoapify → LocationIQ place queries and user-triggered MyHeritage photo fetches
  from supported GEDCOM links. See prototype #430 and draft PR #433.
- [Geoapify privacy](https://www.geoapify.com/privacy-policy/),
  [LocationIQ privacy](https://locationiq.com/privacy),
  [OpenFreeMap privacy](https://openfreemap.org/privacy/) reviewed as public
  provider references, not account-specific agreements.
- Landing source contains no analytics or tracking cookie/storage code. Actual
  browser and hosting behavior still needs verification. No cookie banner added
  absent a demonstrated requirement.

## Founder confirmations — required before privacy approval

- Confirm exact legal name and contact details of the data controller (natural
  person or legal entity), and any required representative/DPO. The draft uses
  only the existing project name and published contact email, not an invented
  legal identity.
- Confirm the proposed legal bases: affirmative Research Group consent,
  legitimate interest for handling inquiries (record balancing assessment),
  and basis for hosting/security and optional demo data processing.
  Confirm applicable direct-marketing/electronic communications requirements.
  The signup notice describes withdrawal and includes notice version/language
  in the existing submission. Ensure consent records and unsubscribe requests
  are handled in practice; do not treat a form field as sufficient proof.
- Confirm retention/deletion policy for inbox, backups, signup list and provider
  records; account plan, DPA applicability, actual subprocessors, international
  transfer assessment and safeguards, anti-spam and optional integrations.
  Confirm the mailbox provider/arrangements and who can access submissions.
- Confirm icon, logo and screenshot/underlying media rights. Document required
  credits and approval for any replacements; no blanket claim of ownership.
- Review source correspondence for the exact deployed revision. Root GPL text
  is copied byte-identically into src/ because the existing workflow copies
  only src/. Keep both copies synchronized; if deployment-revision binding
  requires a workflow change, request specific authorization first.

## QA pending

Test both languages, all six existing pages and both license pages in real
browser at mobile/desktop widths; check keyboard, font loading, network/storage,
local license/source paths and form validation/success/error using controlled
test data. Do not send unsolicited submissions. Verify exact deployed artifact
and links after authorized publication. No deploy/merge performed by this work.
