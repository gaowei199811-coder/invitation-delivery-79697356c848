# Independent metadata review

**Verdict: needs_revision.** All mechanical checks pass, but three descriptions need editorial revision to meet the explicit prohibition on padded repetition.

Metadata SHA-256: `9c678174d31433d0136175995595278e69c4ffe149fd0748c0c237dcd06ac71d`

The verdict applies only to these exact bytes of `store-metadata.json`.

R1 — repeated guidance in Simplified Chinese, Traditional Chinese and Japanese (medium severity). Each description reaches its final preview/share workflow, then adds three sections revisiting information order by occasion, detailed addresses and reviewing facts before appearance. Those topics were already explained. The extra details are individually sensible, but the cumulative repetition makes these sections read as padding to satisfy the length target. This is an editorial judgment, not an allegation about the generation method.

- `zh-Hans`: paragraph 4 “把宾客最需要的信息写完整” overlaps paragraph 20 “让不同场合有不同的重点”; paragraph 5 “如果活动在傍晚开始” overlaps paragraph 21 “为复杂地址整理表达”; paragraph 18 “最后从宾客的角度预览” overlaps paragraph 22 “把修改分成两个阶段”.
- `zh-Hant`: paragraph 4 “先交代安排，再寫下心意” overlaps paragraph 22 “依場合安排閱讀順序”; paragraph 5 “日期可以依賓客熟悉的方式表達” overlaps paragraph 23 “把地址寫成實用的指引”; paragraph 19 “先完成主要內容，之後再細看字體與顏色” overlaps paragraph 24 “用兩次閱讀完成收尾”.
- `ja`: paragraph 4 “大切な情報から順番に” overlaps paragraph 18 “場面ごとに情報の順序を考える”; paragraph 4 “招待状を受け取る人が最初に知りたい” overlaps paragraph 19 “住所は具体的な言葉で”; paragraph 16 “最後は受け取る人の目線で” overlaps paragraph 20 “内容と見た目を分けて確認”.

Paragraph numbers count blocks separated by a blank line in the decoded description, including headings with their following text. Consolidate this advice at its first useful location, then use distinct source-supported tasks or examples to keep the required 2800–3200 characters. Simply deleting the final blocks would not satisfy the length requirement. Preserve the subscription paragraphs and exact footer.

The prose generally uses natural localized vocabulary and register. Traditional Chinese is more than a glyph conversion, Spanish uses Spain-oriented forms, Portuguese uses Brazilian phrasing, and Japanese/Korean use appropriate polite instructional language. Shared workflow structure is reasonable and is not itself evidence of blind translation. Seven locales have no blocking prose issue identified; locale-specific observations are recorded in REVIEW.json.

| Locale | Name | Subtitle | Description | Keywords | Keyword UTF-8 bytes | Prose |
| --- | ---: | ---: | ---: | ---: | ---: | --- |
| en-US | 16 | 28 | 3067 | 99 | 99 | pass |
| zh-Hans | 5 | 16 | 3008 | 98 | 240 | needs_revision |
| zh-Hant | 5 | 16 | 3017 | 98 | 240 | needs_revision |
| ja | 16 | 15 | 2980 | 97 | 251 | needs_revision |
| ko | 16 | 18 | 3023 | 100 | 252 | pass |
| fr-FR | 16 | 29 | 2994 | 99 | 105 | pass |
| de-DE | 16 | 27 | 3052 | 98 | 98 | pass |
| es-ES | 16 | 26 | 3032 | 99 | 101 | pass |
| pt-BR | 16 | 26 | 3004 | 100 | 103 | pass |
| ru | 16 | 28 | 3068 | 96 | 182 | pass |

All totals were independently computed from the actual JSON. Description totals include subscription copy, paragraph breaks and both legal lines. Names meet 2–30, subtitles meet ≤30, keywords meet 95–100 including commas, and promotional text meets ≤170. All localized fields are NFC; their UTF-16 unit counts equal their Unicode counts. Both Chinese names contain only Chinese characters. Keyword entries have no exact case-insensitive duplicates or exact reuse from names/subtitles; no competitor brands or unsupported service claims were identified. Related synonyms such as fonts/typefaces are not identical duplicates. Full field byte counts are recorded separately in REVIEW.json.

Eight keyword fields exceed 100 UTF-8 bytes (all except en-US and de-DE). APPLE_RULES.md records conflicting character/byte documentation. These counts satisfy the user-requested character test only; they establish neither App Store Connect acceptance nor Apple approval.

All ten subscription paragraphs are explicitly conditional and cover Apple Account billing on purchase confirmation, automatic renewal, cancellation at least 24 hours before period end, renewal charging within the final 24 hours at the applicable displayed price, and account subscription management/cancellation. None invents a product price, named plan, subscription duration, trial or paid entitlement. The supplied BRIEF reports an empty product ID, so this language is not evidence of a configured or working purchase. The verbatim disclosure for each locale is preserved in REVIEW.json.

Every description ends exactly with the following two lines, with no trailing newline or content inside the description:

```text
Privacy Policy: https://xhycapps.com/pp/6824400361/
Terms of Use: https://xhycapps.com/tou/6824400361/
```

Feature claims match the supplied implementation evidence: occasion templates and samples (gallery), selected-text fonts/color/style (font/color), compatible restyling (restyle), guest-name input and individual exports (guests), manually entered second-language text and separate previews (bilingual), available layout formats (resize), local drafts/rename/duplicate (designs), and image sharing/Photos (share). The descriptions do not promise automatic translation, ten UI languages, RSVP collection, delivery tracking, cloud sync or paid access. Advice to check dates and addresses remains a user action, not a promised automated correctness check. Palette behavior and export success were not runtime-tested here.

The frozen v9 BRIEF and v8 SOURCE_AUDIT are the feature evidence. Both competitor reports were reviewed as historical research, not instructions or proof of shipped features. Their sample-text, bilingual-review and resend concerns can inform useful copy; their proposed Pro gates, ten-language UI, export version tracking and strict checking cannot establish implemented functionality. No competitor prices or market-superiority claims were imported into the metadata.

The BASELINE.json hash matches INPUT_RECEIPT.json. Only the ten description fields and top-level rationale changed. All other fields, captions and category remain identical. VALIDATION.json is bound to the same metadata hash, and its reported counts agree with independent counts. ASO_RATIONALE.md correctly maps the main features and counting caveat, but its claim that all descriptions avoid padding is not supported by R1. The baseline rationale excluded bilingual workflows under older evidence; the newly specified source audit supports their inclusion here.

Review limitations: this is a source-based textual assessment, not native-speaker certification, a fresh source-code audit, app/device test, billing test, live Apple policy verification, or verification of legal-page availability/content. Historical competitor sources were not refreshed. The supplied validator was not executed because it writes files outside the two authorized review outputs. No metadata, baseline, validation, campaign or app was edited. No upload or approval was performed.

All requested inputs and their SHA-256 hashes are listed in REVIEW.json.
