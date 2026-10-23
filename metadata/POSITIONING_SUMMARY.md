# English positioning revision v7

The approved name is **Dearly: Invitation Studio**, exactly matching `APPROVED_POSITIONING.json` → `selected_names.en-US`. “Dearly” suggests a personal greeting; “Invitation Studio” identifies the creation task and supports the emphasis on editable wording and composition. The subtitle, “Bilingual cards for each guest,” connects the two leading workflows without implying translation.

The saved US Apple name query in `name-checks/en-US-0.json`, checked on 2026-10-23 at 03:40:26 UTC, returned no normalized exact match for the selected name. This is a limited search-result observation, not trademark clearance, a complete market search or a prediction of App Review acceptance.

## Research and owner direction

Read `APPROVED_POSITIONING.json`, `RESEARCH_BINDING.json`, the saved Apple competitor descriptions, and the owner's `COMPETITIVE_ANALYSIS.md` and `PRODUCT_DIRECTION.md`. The current bound Apple collection was fetched on 2026-10-23 at 03:33:54 UTC; the owner reports describe an earlier research snapshot and proposed product direction. Those reports provide context, while actual Swift behavior establishes claims used here.

In `MARKET_RESEARCH/competitors.json`, Greetings Island (1329922018) advertises templates, AI creation and RSVP management; Evite (431685286) emphasizes response tracking, messaging and distribution; 1Invites (1320828574) advertises fonts, photos, background removal, export and RSVP tools. These observations favor leading with the concrete combination of manually authored language versions, named PNG batches and reusable wording across visual changes. They do not establish that competitors lack these capabilities. No competitor slogans, template counts, prices or advertised features were transferred into this listing.

## Verified implementation evidence

All source references below are relative to `/Users/liguoliang/Documents/Codex/2026-10-22/invitation-workflows/listing-10languages/run-localized-v9/app`. The validator's research verification matched the bound source hashes and saved research hashes.

| Listing claim | Source evidence and limits |
| --- | --- |
| Manually authored bilingual versions and separate output | `Sources/CheckAndBilingual.swift`: `BilingualSettings`, `BilingualTextEditor` and `ExportLanguagePicker` expose editable second-language content and first/second/both selection. `Sources/InvitationToolPages.swift:440–478` renders each selected version separately. No automatic translation or semantic verification claim. |
| Guest-name PNG batches | `Sources/InvitationToolPages.swift:149–164,249–266,434–484`: retains the message, accepts one guest per line, supports pasting, limits batches to 100 guests, checks each guest/version and writes PNG files. No attendance tracking or automatic delivery claim. |
| Typography controls | `Sources/CanvasTextEditor.swift:1324–1408`: individual letter spacing, line spacing, rotation, size and alignment controls. Benefits concern readable hierarchy and arrangement, not an invented automatic layout algorithm. |
| Compatible themes preserve words | `Sources/EditorPages.swift:56–67,156–180`: changes palette or template on the existing design. Template switching is disabled with a photo background; the description states this limitation. |
| Photo cutout layouts | `Sources/PhotoElementsEditor.swift:524–539,945–969` and its positioning controls: separate subject elements, failure handling, scale, rotation and placement. Extraction success is not promised for every photo. |
| Local drafts and reuse | `Sources/AppStore.swift:114–140`: persistence, rename and duplication with a new identity and reset export state, retaining design content and assets. No cloud backup or synchronization claim. |
| Actual image export | `Sources/ExportPages.swift:240–310`: PNG encoding, file writes and Photos resource creation; output URLs support sharing. Revised images must be exported and shared again by the user. |
| Conditional subscription wording | `Resources/ProductConfiguration.json` has an empty `proProductID`; `Sources/PurchaseStore.swift` treats an empty ID as unavailable. Disclosure is conditional and covers confirmation charge, automatic renewal, cancellation at least 24 hours before period end, renewal charging within 24 hours before period end and account management. No price, trial, plan or paid-feature claim. |

## Delivery and validation

`store-metadata.json` starts from the approved v6 `PREVIOUS_DRAFT.json`. Only the six authorized en-US fields and top-level rationale changed. Nine non-English localizations, every screenshot caption, category, whats_new and all remaining keys are preserved exactly as JSON values. `ENGLISH_METADATA.txt` contains the name, subtitle, keywords and full description.

English field lengths: name 25; subtitle 30; keywords 99 ASCII characters and 99 bytes; description 2,979 total Unicode characters including footer; promotional text 163. The description has seven feature sections and 13 distinct feature bullets. Keywords are comma-separated, unique, relevant to the creation task and do not repeat words in the name or subtitle.

The exact final two description lines retain the owner-specified Privacy Policy and Terms of Use URLs from `LEGAL_LINKS.json`. The owner's known page identity issue is unchanged; no website was edited.

Validation passed using the existing validator and its supported listing catalog configuration:

```sh
BRAIDRUN_LOCALE_CATALOG=app_store_locales.json python3 validate_revision.py
```

The initial default-catalog invocation stopped because the default generation catalog does not accept every preserved listing locale. Selecting the supplied App Store listing catalog resolved that configuration mismatch without editing the validator, inputs, research or locale keys. Generated reports are `VALIDATION.json` and `STORE_METADATA.md`. No App Store upload was performed.

A final run of `python3 validate_revision.py` also passed. During this session, an external change added `os` and the listing-catalog environment setting to the validator; this agent did not edit that file. Its SHA-256 changed from `a431dcb8269c4c22080836dcebbedd99f584fcf0c38bf2d8307cd89c76b1a936` to `67409659d7c2741579bf03d5dd9af80c58de3afa32eeedd4e7dccb1c3a49a9be`. All other pre-existing files in the working directory matched the pre-write hash snapshot.
