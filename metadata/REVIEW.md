# Independent metadata review

**Verdict: pass.** Local delivery only; this review is not approval, upload authorization or an Apple acceptance claim.

Metadata SHA256: `4724f87aae7d9a05a4187d9951021382a815fae36e655ecc0726ee5d7052b6a1`

Read both complete research reports (232 and 243 lines), RESEARCH_RECEIPT.json, ASO_RATIONALE.md, BASELINE.json, INPUT_RECEIPT.json, store-metadata.json, VALIDATION.json and the en-US SOURCE_AUDIT.json. Independently inspected active Swift implementation and target membership. Research hashes match their receipt; baseline and frozen source metadata match INPUT_RECEIPT.json.

Only authorized fields changed: 40 subtitle/promotional-text/description/keyword values, two Chinese names, and rationale (43 values total). JSON structure, locale set, all screenshot captions, eight other names, all whats_new strings, category, primary locale and schema remain equal to the baseline. Both Chinese names consist solely of Chinese characters.

The revision meaningfully applies the research: R02/N06 inform the explicit image-making outcome; W07/N01 inform sample-to-personal-information wording; R06/N10 inform manual rereading before sharing. These decisions appear in all ten descriptions, not only in the rationale. Offline, bilingual/Pro, automated validation, per-language versions and ten-language UI proposals were not promoted into marketing promises. Competitor brands/prices, invented demand, comparison claims and unsupported feature claims are absent from customer-facing fields. Internal rationale discusses exclusions as exclusions.

## Active code verification

- **Illustrated occasion templates, full sample preview, selection:** Active catalog, rendered sample card and Use Template action exist. Details is accessed by context menu; copy does not invent a tap sequence. Sources: [project.yml:18](../app/project.yml:18), [MainPages.swift:123](../app/Sources/MainPages.swift:123), [MainPages.swift:193](../app/Sources/MainPages.swift:193), [MainPages.swift:372](../app/Sources/MainPages.swift:372), [MainPages.swift:411](../app/Sources/MainPages.swift:411), [MainPages.swift:446](../app/Sources/MainPages.swift:446).
- **Event title, names, date/time, venue/address and personal message:** quickDetails binds title/hosts, date/time, venue, address and message to the edited invitation. Venue/address apply to in-person/hybrid events. Sources: [EditorPages.swift:618](../app/Sources/EditorPages.swift:618).
- **Individual text editing, font choice and on-card appearance:** Editor opens the selected text editor; changes update draft text and face settings used by rendering. Font selection and preview are implemented. Sources: [EditorPages.swift:504](../app/Sources/EditorPages.swift:504), [CanvasTextEditor.swift:830](../app/Sources/CanvasTextEditor.swift:830), [CanvasTextEditor.swift:1048](../app/Sources/CanvasTextEditor.swift:1048), [CanvasTextEditor.swift:1190](../app/Sources/CanvasTextEditor.swift:1190), [CanvasTextEditor.swift:339](../app/Sources/CanvasTextEditor.swift:339).
- **Complete preview, share image, save to Photos:** Reachable export page renders preview, generates image files, opens UIActivityViewController and writes photo resources after authorization. Copy does not promise delivery, receipt, format selection or automatic checking. Image wording accommodates implemented PNG/GIF paths. Sources: [Navigation.swift:313](../app/Sources/Navigation.swift:313), [ExportPages.swift:58](../app/Sources/ExportPages.swift:58), [ExportPages.swift:200](../app/Sources/ExportPages.swift:200), [ExportPages.swift:221](../app/Sources/ExportPages.swift:221), [ExportPages.swift:237](../app/Sources/ExportPages.swift:237), [ExportPages.swift:292](../app/Sources/ExportPages.swift:292), [ExportPages.swift:789](../app/Sources/ExportPages.swift:789).
- **English and Simplified Chinese UI; other listing languages are not extra UI languages:** store.t chooses English or Chinese; Chinese strings are Simplified Chinese. System zh languages select that Chinese branch; other system languages default to English unless explicitly overridden. No additional UI localization is claimed. Sources: [AppStore.swift:34](../app/Sources/AppStore.swift:34), [AppStore.swift:36](../app/Sources/AppStore.swift:36).

The target includes Sources and Resources in project.yml; the Xcode project also includes the inspected editor, catalog and export files. The source audit is a useful scope record, but the verdict above comes from checking reachable implementation, not assuming its feature list or product-direction proposals are proof.

## Locale observations

Counts include commas and spaces and are independently computed from actual decoded strings. All ten keyword strings are near the 100-character target (96–100). No empty terms, surrounding whitespace, exact or normalized duplicate terms, or full keyword terms repeated in name/subtitle were found. Editorial review found no obvious name/subtitle waste, competitor brands, unrelated padding or excessive synonym stuffing. Related font and occasion synonyms are relevant local phrases, not promises of extra features.

| Locale | Name | Subtitle | Promo | Description | Keywords | Terms |
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

- **en-US** — Birthday/party/card/design intent sits in the subtitle; keywords add templates, lettering, event details and image use. Stationery is relevant digital-card vocabulary and does not promise printing.
- **zh-Hans** — Natural Simplified Chinese name and terms. 活动通知 means invitation/notice content in this context, not push notifications. Family meals, banquets and anniversaries are editable-card uses, not promised dedicated templates. 字体/字形 and 聚会/亲友相聚 are related but distinct phrases; no excessive repetition.
- **zh-Hant** — Traditional Chinese name and vocabulary, including 範本, 個人化 and 照片儲存. 字體/字型 are conventional local search synonyms, not exact duplicates. Gathering/anniversary terms describe uses of editable cards. The description explicitly disclaims Traditional Chinese UI.
- **ja** — Natural invitation vocabulary; フォント/書体 and レタリング describe relevant lettering choices. 記念日 and 家族の集まり are plausible editable-card uses. Japanese UI is explicitly disclaimed.
- **ko** — Relevant Korean invitation, occasion, editing and image terms. 글꼴/서체 and 타이포그래피 are related local terms without exact duplication; no repeated inflection padding. English UI fallback is disclosed.
- **fr-FR** — French accents and natural fête/modèle/polices vocabulary retained. Birthday intent is in the subtitle; keywords cover editing and image output. English UI fallback is disclosed.
- **de-DE** — Relevant German birthday, party, template and font terms; common loanwords design/event are appropriate. Feier in the subtitle complements Geburtstag/Party. English UI fallback is disclosed.
- **es-ES** — Natural Spanish invitation/editing vocabulary, including diseño, fuentes and guardar. cumpleaños stays in the subtitle. The actual es-ES locale is preserved despite the roadmap mentioning es-MX; UI language is limited to English/Simplified Chinese.
- **pt-BR** — Brazilian Portuguese terms, including compartilhar, salvar and comemoração, are appropriate. Anniversary/birthday intent sits in the subtitle; no unsupported capability is added. UI language disclosure remains.
- **ru** — Natural Russian party/card/template/font and image-action terms. День рождения is in the subtitle and not repeated in keywords. English UI fallback is disclosed.

Names/subtitles are within 30 characters, promotional text within 170, descriptions within 4,000, and keywords within 100. All keyword counts agree with VALIDATION.json. REVIEW.json preserves the exact reviewed keyword strings, per-locale counts, input hashes and changed paths.

## Issues and limits

No revision issues found. Source review does not establish runtime success, actual sending or device Photos permissions. Keyword relevance is an editorial assessment, not evidence of demand or ranking. Supplied historical research was reviewed in full; its external competitor claims were not refreshed. Only REVIEW.json and REVIEW.md were written.
