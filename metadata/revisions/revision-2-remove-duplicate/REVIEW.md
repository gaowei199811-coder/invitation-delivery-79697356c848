**Verdict: needs_revision.** One English editorial defect prevents a pass. This is a fresh review of the actual metadata bytes, previous draft, validation, approved positioning, bound raw Apple results, and the original app source. No previous verdict was reused.

The first bullet under “Write for both audiences” says: “Write the second language version yourself, then switch previews to review each card. Write and edit a second language version yourself, then preview each card.” The second sentence repeats the first without adding useful information. Delete that second sentence and its preceding space. This would leave **2,909 characters**, including the conditional subscription disclosure and exact legal footer; no replacement padding is needed. This correction is proposed only and has not been applied.

Fresh byte hashes:

- `store-metadata.json`: `9696dee1c62f0d790943903bcf0246766eb4eb2b31477a32f85bbde841c51797`
- `RESEARCH_BINDING.json`: `523dce3b55525b0cc755962ae72869a4d3e9900f39f68a221f0d58e5731bce3e`

Both match VALIDATION.json. Every file digest listed in RESEARCH_BINDING.json matches the actual referenced file, and all five bound Swift source digests match the original source under `/Users/liguoliang/Documents/Codex/2026-10-22/invitation-workflows/listing-10languages/run-localized-v9/app`. The validation pass correctly reports numerical compliance but does not resolve the repeated English sentence.

Independent counts use Unicode characters, including spaces, line breaks, subscription text and footer. Keyword bytes use UTF-8. Feature counts exclude subscription and legal material.

| Locale | Name | Subtitle | Description | Keywords chars / bytes | Feature sections / bullets | Repetition |
| --- | ---: | ---: | ---: | ---: | ---: | --- |
| en-US | 25 | 30 | 2984 | 99 / 99 | 7 / 13 | Fail: repeated sentence |
| zh-Hans | 5 | 16 | 2935 | 98 / 240 | 8 / 23 | Pass |
| zh-Hant | 5 | 16 | 2893 | 98 / 240 | 8 / 23 | Pass |
| ja | 16 | 15 | 2920 | 97 / 251 | 8 / 22 | Pass |
| ko | 16 | 18 | 2831 | 100 / 252 | 8 / 18 | Pass |
| fr-FR | 16 | 29 | 3141 | 99 / 105 | 8 / 16 | Pass |
| de-DE | 16 | 27 | 3084 | 98 / 98 | 8 / 16 | Pass |
| es-ES | 16 | 26 | 3092 | 99 / 101 | 8 / 16 | Pass |
| pt-BR | 16 | 26 | 3068 | 100 / 103 | 8 / 16 | Pass |
| ru | 16 | 28 | 3099 | 96 / 182 | 8 / 16 | Pass |

All names and subtitles meet the 30-character ceilings. English keywords meet both the 95–100-character and 95–100-byte requirements, are relevant to occasions and supported editing features, contain no repeated keyword entries, and do not duplicate words in the English name/subtitle. English has seven clear feature sections and 13 distinct useful bullets despite the redundant sentence within the first bullet. Its structure passes; repetition and professional editorial quality fail. The remaining English language is clear and concrete, without pseudo-technical embellishment.

All nine non-English descriptions remain within their retained 2,800–3,200-character bounds and have eight feature sections. Their repetition checks pass: introductory summaries are developed into distinct actions, controls or examples rather than duplicated instructions. Their existing non-ASCII keyword byte counts are reported transparently; the special 95–100-byte requirement here applies to English.

A recursive comparison with PREVIOUS_DRAFT.json finds changes only in `en-US.name`, `en-US.subtitle`, `en-US.promotional_text`, `en-US.description`, `en-US.keywords`, and the explanatory top-level `rationale`. All nine non-English localization objects are exactly equal as parsed JSON values. Every screenshot caption, every locale’s `whats_new`, schema version, primary locale, category, and every other protected field is unchanged. This verifies field values, not identical whole-file serialization.

The English name is exactly the selected name in APPROVED_POSITIONING.json: **Dearly: Invitation Studio**. The saved US Apple search receipt `name-checks/en-US-0.json`, checked at 2026-10-23T03:40:26.571067+00:00, contains 48 results and no normalized exact match. This supports only that bounded search observation, not universal uniqueness, trademark clearance, name reservation, or review acceptance. The metadata makes none of those claims.

The opening leads with two language versions and named guest cards, a concrete combination supported by the source. The saved raw Apple descriptions establish that Greetings Island (1329922018) emphasizes templates, AI creation and RSVP management; Evite (431685286) promotes RSVP/view tracking and guest messaging; and 1Invites (1320828574) already advertises fonts, photos, background removal and export. The revision appropriately uses cutouts and typography as supporting benefits. It does not assert those competitors lack bilingual editing or named image batches, claim exclusivity, or promise to avoid review. No distinctive copied rival language was found; an additional normalized eight-word overlap check of English feature copy against all three saved search-result sets found no matches. That check supports, but cannot prove, originality beyond these materials. Saved raw review feeds were parsed and hash-checked; user reviews are not treated as proof of competitor feature absence. These are the saved live-search captures, not a new live search or an exhaustive market audit.

Source checks were made against implementation, not just the positioning references:

- `Sources/CheckAndBilingual.swift:140–151, 509–590, 793–839`: first/second/both export selection, preview controls and directly editable second-language text. The app also contains optional translation machinery; the listing describes the supported manual workflow without claiming translation is impossible.
- `Sources/InvitationToolPages.swift:148–170, 249–310, 434–480`: keeps the original message, accepts one pasted guest per line, uses the name placeholder, limits batches to 100 guests, and renders PNG files separately for each guest and selected language.
- `Sources/EditorPages.swift:56–67, 156–180`: palette changes and template replacement preserve wording; template switching is disabled for photo backgrounds, as disclosed.
- `Sources/CanvasTextEditor.swift:1323–1408`: individual text spacing, rotation, size and alignment controls substantiate the typography claims.
- `Sources/PhotoElementsEditor.swift:146–155, 524–539, 945–959`: extracted subjects become separate elements, extraction can fail, and cutouts can be scaled and rotated. The listing includes a practical failure qualification.
- `Sources/AppStore.swift:99–137`: local persistence, renaming and duplication retain design content and active photo references in a new draft.
- `Sources/ExportPages.swift:253–307`: PNG rendering, output URLs and Photos saving substantiate image export. Exported static images must be regenerated and shared after edits.
- `Sources/PurchaseStore.swift`: product loading handles an empty product ID as unavailable. The metadata makes subscription availability conditional and promises neither a current price nor a trial.

Every description ends with the exact required footer:

```text
Privacy Policy: https://xhycapps.com/pp/6824400361/
Terms of Use: https://xhycapps.com/tou/6824400361/
```

**Non-blocking owner-retained limitation:** the legal webpages’ wrong product name remains unresolved, as stated by the owner. The owner explicitly retained these URLs. This review does not fail the metadata for that decision or claim the webpage mismatch was fixed; the pages were not re-fetched in this review. Conditional subscription information and the literal footer are present.

Only REVIEW.json and REVIEW.md were written. No metadata, baseline, validation, campaign or app edits, approval, or upload were performed. This is a static source and copy review, not a device execution test.
