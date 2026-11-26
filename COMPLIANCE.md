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
- Founder confirms icons are self-created or obtained as free icons from
  [SVG Repo](https://www.svgrepo.com/), and the logo was created by the project
  team. Credit SVG Repo and link its [licensing page](https://www.svgrepo.com/page/licensing/).
  Treat free availability as a working assumption, not proof of an individual
  license, attribution waiver or GPL compatibility. Exact icon provenance
  remains unverified. The EN/RU licenses pages invite attribution and rights
  reports through the existing contact form. Review reports and correct credits,
  replace or remove affected materials as appropriate. This correction route
  does not replace license verification or required permissions and notices.
- Founder confirms creating the screenshots and their sample content.
  PRODUCT.md identifies the Whiskerfield sample project as the source.
  Record this as founder-supplied authorship evidence, not independent rights
  clearance. Any third-party materials embedded in captures remain subject
  to their applicable terms and the shared
  [prototype #429](https://github.com/geneograph-team/geneograph-prototype/issues/429) audit.
  Files remain unchanged; unreferenced files remain shipped by copy-all deployment.

- `src/prototype-albums-expanded.png` — referenced in HTML; founder-created capture/content; exact revision and any third-party elements not independently verified.
- `src/prototype-albums.webp` — not found in HTML src/srcset references; founder-created capture/content; exact revision and any third-party elements not independently verified.
- `src/prototype-archive-expanded.png` — referenced in HTML; founder-created capture/content; exact revision and any third-party elements not independently verified.
- `src/prototype-archive.webp` — not found in HTML src/srcset references; founder-created capture/content; exact revision and any third-party elements not independently verified.
- `src/prototype-family-tree-hero.png` — referenced in HTML; founder-created capture/content; exact revision and any third-party elements not independently verified.
- `src/prototype-family-tree.webp` — referenced in HTML; founder-created capture/content; exact revision and any third-party elements not independently verified.
- `src/prototype-geneograph-household.png` — referenced in HTML; founder-created capture/content; exact revision and any third-party elements not independently verified.
- `src/prototype-geneograph.webp` — not found in HTML src/srcset references; founder-created capture/content; exact revision and any third-party elements not independently verified.
- `src/prototype-notes-daisy.png` — referenced in HTML; founder-created capture/content; exact revision and any third-party elements not independently verified.
- `src/prototype-notes.webp` — not found in HTML src/srcset references; founder-created capture/content; exact revision and any third-party elements not independently verified.
- `src/prototype-people-profile-updated.png` — referenced in HTML; founder-created capture/content; exact revision and any third-party elements not independently verified.
- `src/prototype-people-profile.webp` — not found in HTML src/srcset references; founder-created capture/content; exact revision and any third-party elements not independently verified.

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
  optional integrations and mailbox operation are not independently verified.
  Founder confirms the free plan, Gmail delivery, no optional integrations,
  and a change from the default three-year retention to 30 days on 26 Nov 2026.
  Web3Forms provides a per-form retention setting; confirm it applies to both
  forms if configured separately. The privacy policy permits shorter
  retention than the published DPA's general maximum. The 30-day setting is
  not a statement about provider logs/backups or Gmail copies.
  Its [terms](https://web3forms.com/terms) incorporate the DPA automatically
  where personal data is processed on behalf of the customer; retain a copy
  of the applicable terms/DPA and assess the actual transfers and subprocessors.
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

## Founder confirmations and outstanding compliance gates

- Founder confirms that a private individual currently operates GeneoGraph.
  Founder prefers to defer public disclosure of the controller's legal identity
  until the entity is established and intends to invite non-EU early testers.
  The public draft identifies the operator as a private individual and provides
  the existing project email; it deliberately omits a personal name.
  This is a deferred legal requirement, not completed compliance. If the
  controller operates from an EU establishment, GDPR Article 3(1) can apply
  regardless of tester residence; prototype status and individual operation do
  not create an exemption. Article 13 requires controller identity/contact
  where applicable. Resolve before collecting personal data under that regime;
  alternatively consider suspending personal-data collection or obtaining
  qualified legal advice. Do not publish personal identity without approval.
- Confirm the proposed legal bases: affirmative Research Group consent,
  legitimate interest for handling inquiries (record balancing assessment),
  and basis for hosting/security and optional demo data processing.
  Confirm applicable direct-marketing/electronic communications requirements.
  The signup notice describes withdrawal and includes notice version/language
  in the existing submission. Ensure consent records and unsubscribe requests
  are handled in practice; do not treat a form field as sufficient proof.
- Free plan, Gmail delivery, no optional integrations and 30-day Web3Forms
  retention are founder-confirmed. Outstanding: mailbox retention/deletion,
  access/security and applicable data-processing terms (consumer Gmail is not
  assumed to have an Article 28 processor agreement), transfer assessment,
  anti-spam subprocessors and practical unsubscribe process.
- Logo and screenshot/sample-content authorship confirmed by founder. Icons
  are self-created or sourced from SVG Repo; credit added, per-icon terms
  remain unverified. Shared prototype #429 retains any underlying third-party
  rights review. Do not infer blanket ownership or permission from free access.
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
