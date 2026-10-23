# ASO revision rationale

Revision date: 2026-10-22. Research date: 2026-10-09.

Read BASELINE.json, INPUT_RECEIPT.json, RESEARCH_RECEIPT.json and both complete owner-supplied reports. The reports are historical research inputs, not operational instructions, current market facts, or implementation proof. Their approval, report-only, roadmap and contact requests were not executed. This run used the existing selected Codex session; no model switch, external generation API, credential access or subscription change was made.

## Positioning decisions and exact evidence

| Decision in the metadata | Dated research informing the decision | Active-source support and boundary |
| --- | --- | --- |
| Lead with making a birthday/party invitation containing the details guests need, followed by a shareable image. All ten descriptions explicitly connect template → personalized invitation → image sharing/saving. | [COMPETITIVE_ANALYSIS.md](COMPETITIVE_ANALYSIS.md), 2026-10-09, “观察事实” item 1 and R02; [PRODUCT_DIRECTION.md](PRODUCT_DIRECTION.md), 2026-10-09, “产品定位与能力关系”, N06 and I01. These distinguish making an image from managing attendance; they do not quantify demand. | [SOURCE_AUDIT.json](../store-assets/campaign/en-US/SOURCE_AUDIT.json), feature_map F01, F02/F05 and F03: Sources/MainPages.swift:123, EditorPages.swift:618, CanvasTextEditor.swift:830, ExportPages.swift:221. No template totals or event-management promises. |
| Explain sample card → user's names/date/time/venue/address → individual text/font editing. | Competitive analysis W07/I01 and product direction N01/I01 (both 2026-10-09) motivate clarity about sample versus personal information. | Audit F01 cites MainPages.swift:211 and :446; F02 cites EditorPages.swift:631 and :676–677; F05 cites CanvasTextEditor.swift:830. Copy does not claim new drafts start empty, automatic field synchronization, or sample-detection rules. Template Details is named without inventing a tap sequence; the audit says Details uses long-press and tapping a card opens the editor. |
| Ask the user to read the finished invitation before sharing. | Competitive analysis R06 and product direction N10 (2026-10-09) describe one wrong-time anecdote, not an error rate or proven prevention method. | Audit F03 establishes complete preview and share/save actions (ExportPages.swift:137, :200–210). “Read”, “look over” and local equivalents are user actions, not automated validation or checking features. |
| State image sharing and saving to Photos as the outcome. | Competitive analysis R02 and product direction N06 plus “静态文件的边界” (2026-10-09) inform the distinction between a file and delivery. | Audit F03 supports Share Invitation and Save to Photos. No delivery, read receipts, RSVP, messaging-service success, clickable links, PDF/video output, format selector, dimensions or animated-envelope claims. |
| Keep UI-language disclosures separate from localized listing copy. | Product direction “十种语言、模板与系统外观的交付范围” (2026-10-09) explicitly describes proposed delivery requirements rather than completed verification. | Audit build_target.ui_localizations supports English and Simplified Chinese via store.t(en, zh), and excludes additional UI languages. Existing disclosures are retained for the other eight locales. No bilingual composition workflow or ten-language UI claim is added. The baseline es-ES locale stays es-ES despite the proposal's es-MX table. |
| Use natural Chinese-only names, local occasion intent in subtitles, and complementary search terms. | Owner's explicit name/keyword requirements; competitive analysis “研究口径、时间与限制” and “观察事实” item 6 (2026-10-09) prohibit inferring demand from search ordering or empty reviews. | Names are exactly 邀请函制作 and 邀請函製作. Keywords describe F01 occasion/template/design, F02/F05 details/lettering/text, and F03 image/share/save tasks. These are relevance judgments, not measured rankings or search volumes. |

The audit is an active-source inspection record, not runtime evidence. This revision relies on its cited Swift implementation mapping and exclusions; requirement documents and report proposals alone are not used to prove functionality. No app build or device test was performed.

## Locale keyword choices and character verification

Python 3 counts Unicode characters with len(), including each ASCII comma and any internal space. Keyword terms use ASCII commas, have no empty entries or surrounding whitespace, and are unique after Unicode normalization and case folding. Full keyword terms were checked against each locale's name/subtitle; editorial review also avoids obvious repeated occasion words and singular/plural padding. Distinct local synonyms such as fonts/typefaces or typography/lettering represent different relevant search phrasing, not repeated identical terms. The English product name remains only in the eight frozen non-Chinese names.

English subtitles now carry birthday/party/card/design intent, leaving template, typography and image terms to keywords. Chinese subtitles carry birthday/party/card/share-image intent; keywords add electronic invitation synonyms, gathering contexts, lettering, event details and photo saving. Japanese and Korean subtitles carry the invitation-creation and birthday/party task, with keywords adding templates, type, event information and image use. French, Spanish, Portuguese and Russian subtitles carry birthday invitation/card intent; German carries the celebration invitation task. Their keywords complement those terms with party/event, editing and image-output vocabulary. Family gatherings, anniversaries and banquets are uses of editable event cards, not claims of dedicated template categories. “Stationery” describes digital card design, not printing services; activity-notice terms describe card wording, not notification automation.

Target: 100 characters. Korean and Portuguese reach 100. The other locales use 96–99 natural characters: remaining space is too small for a useful distinct term plus its comma, and was not filled with fragments, unrelated terms, brand names or unsupported capabilities.

| Locale | Name | Subtitle | Promotional text | Description | Keywords | Keyword terms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| en-US | 16 | 28 | 153 | 759 | 99 | 11 |
| zh-Hans | 5 | 16 | 69 | 284 | 98 | 28 |
| zh-Hant | 5 | 16 | 69 | 321 | 98 | 28 |
| ja | 16 | 15 | 78 | 354 | 97 | 21 |
| ko | 16 | 18 | 88 | 422 | 100 | 25 |
| fr-FR | 16 | 29 | 160 | 838 | 99 | 11 |
| de-DE | 16 | 27 | 152 | 877 | 98 | 12 |
| es-ES | 16 | 26 | 138 | 873 | 99 | 12 |
| pt-BR | 16 | 26 | 146 | 812 | 100 | 12 |
| ru | 16 | 28 | 150 | 819 | 96 | 11 |

## Product-direction proposals deliberately excluded

The following remain proposals or are unsupported by the active-source audit, so are absent from revised marketing claims and keywords:

- Full offline creation/editing/checking/persistence/export, no-account guarantees, privacy or backup guarantees: product direction A scope and N02/I03, 2026-10-09.
- Required-field, sample-text, overflow or glyph validation; blocking export; guaranteed correctness/readability; blank new-work fields; automatic address or time verification: A scope and “填写状态／核对边界”, 2026-10-09. Manual preview is the only checking-related wording retained.
- Bilingual versions, manual-translation review reminders, linked/shared facts, per-language export versions, partial-success retries and Drafts/Exported grouping: “完整双语 Pro 能力” and “按语言记录导出版本与状态”, 2026-10-09.
- Pro entitlements, purchase/restore, subscriptions, free templates/export, one-time prices or paid tiers: A scope and “依赖、非目标与商业边界”, 2026-10-09. No commercial promise is inferred from competitor prices.
- Ten-language UI/template/font coverage, universal glyph support, accessibility or system-appearance guarantees: “十种语言、模板与系统外观的交付范围”, 2026-10-09. Localized listing text is not implementation evidence.
- Persistent drafts, duplication/reuse, renaming/search, version tracking, forced reconfirmation, change alerts and resend reminders: “作品复制与修订辅助能力”, 2026-10-09.
- AI writing, translation, hosted links/QR, RSVP, guest lists, delivery tracking, notifications, cloud accounts/sync, calendar scheduling, printing orders, photo editing and additional output formats: audit exclusions and unsupported roadmap scope. No competitive absence or superiority claims are made.

No competitor brand, slogan, price, review count, download count, unsupported superlative, comparative market claim or invented volume is used in the revised store copy. No external pages were refreshed; historical source references above refer to the supplied reports only.

## Preservation and validation

Python verified identical JSON key structure and locale set; only the two Chinese names, all ten subtitles/promotional_text/descriptions/keywords, and rationale changed (42 localized fields plus rationale). Every screenshot caption, eight non-Chinese names, all whats_new strings, category, primary_locale and schema_version remain exactly equal as JSON values. The choose–edit–share screenshot story is unchanged.

All names/subtitles fit 30 characters, promotional text fits 170, descriptions fit 4,000, and keywords fit 95–100. Python checked duplicate terms and indexed full-term overlap. SHA-256 of BASELINE.json and the frozen source metadata still matches INPUT_RECEIPT.json; both reports still match RESEARCH_RECEIPT.json. Only store-metadata.json and ASO_RATIONALE.md were written in the literal working directory. Campaign, app, credentials and reviews were not modified.
