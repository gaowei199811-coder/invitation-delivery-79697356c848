# Independent metadata review

Verdict: **needs_revision**. One English source-accuracy correction is required. This is a fresh review of the actual files, not a reused prior verdict or approval for upload.

The English description says “Bilingual content is manually authored, not automatically translated.” The app supports manual editing, but also exposes Translate and Fill / Translate Again on iOS 18+. `CheckAndBilingual.swift:601–622` implements that action; lines 1006–1008 and 1147–1189 execute Apple system translation, and lines 481–494 and 569–573 apply the translated result. This is a functioning source path, not merely a label or placeholder. Runtime translation still depends on device, OS and supported language availability; no device execution was performed in this review.

Remove the categorical denial and present manual writing as an available workflow. Suggested replacement for that bullet: “Write and edit the second language version yourself, then switch previews to review each card.” Preserve the total length requirement, conditional subscription information and exact footer. The approved positioning document's manual-only interpretation does not override the actual source.

## Independent measurements

Counts use Unicode characters and actual UTF-8 encoding. Description counts include the subscription disclosure and legal footer. Feature sections and bullets exclude subscription and legal text.

| Locale | Name | Subtitle | Description | Keywords characters / bytes | Feature sections / bullets |
| --- | ---: | ---: | ---: | ---: | ---: |
| en-US | 25 | 30 | 2979 | 99 / 99 | 7 / 13 |
| zh-Hans | 5 | 16 | 2935 | 98 / 240 | 8 / 23 |
| zh-Hant | 5 | 16 | 2893 | 98 / 240 | 8 / 23 |
| ja | 16 | 15 | 2920 | 97 / 251 | 8 / 22 |
| ko | 16 | 18 | 2831 | 100 / 252 | 8 / 18 |
| fr-FR | 16 | 29 | 3141 | 99 / 105 | 8 / 16 |
| de-DE | 16 | 27 | 3084 | 98 / 98 | 8 / 16 |
| es-ES | 16 | 26 | 3092 | 99 / 101 | 8 / 16 |
| pt-BR | 16 | 26 | 3068 | 100 / 103 | 8 / 16 |
| ru | 16 | 28 | 3099 | 96 / 182 | 8 / 16 |

All names and subtitles meet the 30-character limit. English keywords are 99 characters and 99 UTF-8 bytes, relevant to supported invitation creation, with no duplicated keyword tokens or name/subtitle word overlap. English description has seven clear feature sections and thirteen distinct useful bullets; its 2,979 characters meet the 2,800–3,000 requirement. All nine other descriptions retain their approved 2,800–3,200 bounds. Their byte counts are recorded, not subjected to the English-only 95–100-byte requirement. All locales retain the exact requested legal footer. No duplicate feature bullets or material within-locale repetition was found. English wording is professional and understandable, without pseudo-technical decoration or material padding; the translation denial is an accuracy defect, not a prose-style failure.

## Preservation and evidence

A recursive comparison with PREVIOUS_DRAFT.json found changes only to English name, subtitle, promotional_text, description and keywords, plus the explanatory top-level rationale. All nine non-English localization objects are exactly equal as parsed JSON. All screenshot captions, every whats_new field, primary locale, category, schema version and other keys are unchanged. The rationale change is explicitly recorded here rather than treating the entire file as unchanged.

The name exactly equals APPROVED_POSITIONING.json's selected “Dearly: Invitation Studio.” Independently normalizing the 48 returned names in name-checks/en-US-0.json found no exact match. The receipt records a US Apple software search at 2026-10-23T03:40:26.571067+00:00. This supports only the saved query's result set, not universal uniqueness, trademark clearance, name reservation or review acceptance. No such broader claims appear in the revised customer copy.

Raw Apple search responses were read directly, including the descriptions for track IDs 1329922018, 431685286 and 1320828574. They support the research's observation that templates, typography, photo tools and RSVP-oriented messaging already appear in this market. The English opening instead presents a concrete two-language and guest-name image workflow. This is useful differentiation in emphasis, not proof of competitor feature absence. No copied rival slogans or unsupported absence claims were found; an additional normalized eight-word overlap check of English feature copy against all three saved search-response description sets found no matches. The saved live Apple receipts were reviewed as evidence at their recorded time; no new market-wide search or legal clearance is implied.

Actual source was read under `/Users/liguoliang/Documents/Codex/2026-10-22/invitation-workflows/listing-10languages/run-localized-v9/app`. Beyond the translation exception, the English claims are supported by:

- `InvitationToolPages.swift:148–170,249–308,434–484`: retained message, guest names, greeting substitution, 100-guest limit, and separate guest/language PNG exports.
- `CheckAndBilingual.swift:140–151,793–839`: export language selection and manual second-language editing.
- `EditorPages.swift:56–67,156–180`: palette changes and template switching without replacing wording; photo-background switching restriction.
- `CanvasTextEditor.swift:1324–1408`: text spacing, rotation, size and alignment.
- `PhotoElementsEditor.swift:524–539,945–969`: extracted photo subjects, failure handling, scaling and rotation.
- `AppStore.swift:114–137`: local persistence, renaming and copying content with retained photo assets.
- `ExportPages.swift:231–292`: image export and Photos saving. The copy correctly asks users to export and share a revised image themselves.

The subscription paragraph remains conditional rather than asserting an available paid plan. PurchaseStore.swift checks for an empty product identifier before loading or purchasing. No current price or trial benefit is invented.

All hashes in RESEARCH_BINDING.json were independently checked against the referenced research bytes and the five actual source files; they match. Matching hashes establish binding, not the correctness of the positioning interpretation. VALIDATION.json's counts and metadata/research hashes agree with this independent computation, but its pass status does not resolve the source-accuracy defect.

## Retained webpage limitation

The owner explicitly retained `https://xhycapps.com/pp/6824400361/` and `https://xhycapps.com/tou/6824400361/` despite their current wrong product name. That unresolved webpage/product-identity limitation remains recorded and is not a metadata failure under the owner's decision. The exact footer is preserved. This review does not certify the external pages' legal adequacy or silently correct their URLs.

## Actual-byte hashes

- metadata_sha256: `60dac127d450e64355dc3d4db0e7b735badf9d571a63c018cf72716e0e4a60c2`
- research_sha256: `523dce3b55525b0cc755962ae72869a4d3e9900f39f68a221f0d58e5731bce3e`

Only REVIEW.json and REVIEW.md were written. No metadata, baseline, validation, campaigns or app files were edited; no approval or upload was performed.
