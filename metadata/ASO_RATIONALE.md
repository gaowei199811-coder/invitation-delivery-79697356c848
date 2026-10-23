# ASO rationale — targeted v6

Only `localizations.ko.description` and the top-level `rationale` differ from the supplied v5 PREVIOUS_DRAFT.json. All nine other locale objects, all short fields, whats_new, screenshot captions, category and schema are preserved exactly. BASELINE.json matches the INPUT_RECEIPT.json SHA-256. All outputs are in the literal working directory. No app, campaign, frozen source, credentials, review or previous evidence was edited; no network publication or paid API call was used.

## R1-ko resolution and copy review

Deleted the complete third bullet under “모임에 맞는 첫 디자인”, beginning “예시를 디자인 참고로 삼아 자신의 카드를 시작하세요.” There is no replacement template-start recap. The section now contains only occasion browsing and full-sample composition comparison.

Replaced generic photo expression/pose advice with distinct practical controls: size/rotation and mirroring, opacity and overlapping element order, followed by centering and optional center snapping. Typography now explains letter/line spacing, paragraph alignment and restoring default alignment. Removed the trailing general recap from the draft-duplication bullet as well. These details describe user actions, not implementation mechanics. The complete Korean description was read for flow after editing: occasion selection, event content, typography, style/format, photos, guest/language variants, drafts and final export each own a separate topic. No additional address, proofreading or template-start section was added to reach the character target.

The short two-sentence introduction and eight feature sections are retained, with 18 feature bullets, followed by a separate subscription heading and four billing bullets. Korean copy is 2,831 Unicode code points including spaces, actual newlines, subscription disclosure and the final two legal lines. Existing language limits remain explicit: English and Simplified Chinese UI; English on a Korean-configured device. The nine preserved descriptions were read for context, without expanding the authorized revision scope.

## Feature evidence

Primary scope sources:
- Frozen BRIEF: `/Users/liguoliang/Documents/Codex/2026-10-22/invitation-workflows/listing-10languages/run-localized-v9/app/BRIEF.md`.
- Active v8 audit: `/Users/liguoliang/Documents/Codex/2026-10-22/invitation-workflows/listing-10languages/run-distinctive-v8/store-assets/campaign/en-US/SOURCE_AUDIT.json`.

The audit's gallery, fonts, colour, restyle, cutout, bilingual, resize, guests, designs and share entries support occasion templates, editable lettering, compatible styles and palettes, photo cutouts, manually entered second-language content, available layouts, guest-specific images, local draft reuse and image sharing/saving. Its exclusions and the BRIEF rule out inferred AI service success, RSVP collection, online delivery, commercial printing, template counts, cloud sync, paid entitlements and ten-language UI claims. Source inspection is evidence of controls, not a new runtime test.

Added-control evidence under the frozen app directory:
- `Sources/CanvasTextEditor.swift:1322–1345`: letter and line spacing, default alignment restoration; `:1382–1407`: left/center/right and vertical alignment controls.
- `Sources/PhotoElementsEditor.swift:1020–1105`: size/rotation/opacity, horizontal/vertical flips, center snapping toggle, center X/Y and layer ordering. `:839–866` implements the center guides and snapping while dragging. The copy makes no new claim about cutout accuracy or service success.

Both Swift files were read and compared byte-for-byte with `/Users/liguoliang/Downloads/app 开发/邀请函/InvitationMakerV2/Sources/`; the corresponding files are identical. The original app was read-only.

COMPETITIVE_ANALYSIS.md and PRODUCT_DIRECTION.md supplied historical task/positioning context only. Their recommendations, proposed Pro scope, roadmap and approval language were not treated as instructions or implemented features. No competitor wording, endorsements or market superiority claims were introduced.

## Subscription and legal scope

Frozen `Resources/ProductConfiguration.json` has an empty `proProductID`, consistent with the BRIEF. The preserved Korean subscription block is conditional on choosing an auto-renewing subscription. Its four bullets cover Apple Account charging on purchase confirmation, cancellation at least 24 hours before the period ends, renewal charging within the preceding 24 hours at the displayed applicable renewal price, and management/cancellation in Apple Account subscription settings. It advertises no available plan, integrated purchase flow, paid entitlement, price, trial or duration. Configuration limitations belong here, not in consumer copy.

LEGAL_LINKS.json and the owner confirm the retained URLs with ID 6824400361. The final two English-label legal lines are exact, with nothing following them in each description. The owner has acknowledged the webpages' current product-name mismatch and will correct the pages separately; no URL substitutions or page edits were made.

## Counting and keyword policy

Counts below use decoded NFC Unicode code points, including commas and spaces. Description counts include subscription text and legal footer. UTF-8 keyword bytes are recorded separately. All short fields are inherited unchanged from v5; no keyword expansion or new terms were introduced.

APPLE_RULES.md records the discrepancy between Apple's product-page guidance (100 keyword characters) and the App Store Connect platform-version reference (100 bytes). This revision follows the owner-requested product-page character rule, records bytes transparently and makes no claim of App Store acceptance or Apple approval. No App Store submission was performed.

| Locale | Name | Subtitle | Promo | Description | Keywords | Keyword UTF-8 bytes |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| en-US | 16 | 28 | 153 | 3047 | 99 | 99 |
| zh-Hans | 5 | 16 | 69 | 2935 | 98 | 240 |
| zh-Hant | 5 | 16 | 69 | 2893 | 98 | 240 |
| ja | 16 | 15 | 78 | 2920 | 97 | 251 |
| ko | 16 | 18 | 88 | 2831 | 100 | 252 |
| fr-FR | 16 | 29 | 160 | 3141 | 99 | 105 |
| de-DE | 16 | 27 | 152 | 3084 | 98 | 98 |
| es-ES | 16 | 26 | 138 | 3092 | 99 | 101 |
| pt-BR | 16 | 26 | 146 | 3068 | 100 | 103 |
| ru | 16 | 28 | 150 | 3099 | 96 | 182 |

## Validation

`BRAIDRUN_LOCALE_CATALOG=app_store_locales.json python3 validate_revision.py` passed and generated STORE_METADATA.md and VALIDATION.json. Separate exact-value comparison confirmed that the only differences from v5 are `localizations.ko.description` and `rationale`. Section checks confirm eight feature sections, 18 feature bullets and four subscription bullets. Frozen baseline receipt hash also matches. The validator and previous evidence were not edited.
