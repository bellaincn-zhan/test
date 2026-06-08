# FAQ Website SEO/GEO Upload Plan

This plan organizes the B2B motorcycle FAQ system for website upload, SEO, and GEO (Generative Engine Optimization).

## Deliverables

| File | Purpose |
| --- | --- |
| `FAQ_SEO_GEO_UPLOAD_PLAN.csv` | Full upload plan for all search-facing FAQ question pages. |
| `FAQ_CATEGORY_URL_MAP.csv` | URL and metadata map for FAQ section and group landing pages. |
| `FAQ_SEARCH_INTENT_QUESTION_BANK.md` | Source question bank organized by buyer search intent. |
| `FAQ_CENTER.md` | Category taxonomy and information architecture. |
| `FAQ_CONTENT_GUIDE.md` | Writing rules, page templates, and content production guidance. |

## Coverage

- 14 top-level FAQ sections
- 94 second-level FAQ groups
- 108 category or collection pages
- 943 search-facing FAQ question pages
- 205 P1 high-commercial-intent FAQ pages

## Recommended Website Structure

Use this URL pattern:

```text
/faq/
/faq/{section-slug}/
/faq/{section-slug}/{group-slug}/
/faq/{section-slug}/{group-slug}/{question-slug}/
```

Example:

```text
/faq/ckd-skd-cbu-export-faq/
/faq/ckd-skd-cbu-export-faq/ckd-motorcycle-kits/
/faq/ckd-skd-cbu-export-faq/ckd-motorcycle-kits/what-is-a-ckd-motorcycle-kit/
```

## CMS Fields to Upload

Use `FAQ_SEO_GEO_UPLOAD_PLAN.csv` for question pages. Recommended CMS field mapping:

| CSV Column | CMS Field |
| --- | --- |
| `page_id` | Internal content ID |
| `status` | Publishing status |
| `priority` | Content rollout priority |
| `buyer_stage` | Funnel stage |
| `search_intent` | SEO intent cluster |
| `section` | FAQ section |
| `group` | FAQ group |
| `question` | FAQ question |
| `h1` | Page H1 |
| `seo_title_tag` | SEO title |
| `meta_description` | Meta description |
| `url_path` | Page URL |
| `canonical_path` | Canonical URL |
| `parent_section_url` | Parent section link |
| `parent_group_url` | Parent group link |
| `breadcrumb` | Breadcrumb |
| `schema_type` | Structured data type |
| `geo_answer_brief` | GEO answer-writing brief |
| `recommended_answer_structure` | Article structure |
| `primary_cta` | Page CTA |
| `internal_link_targets` | Internal links |
| `entity_terms` | Entity terms for SEO/GEO |
| `robots` | Indexing rule |

Use `FAQ_CATEGORY_URL_MAP.csv` for section and group landing pages.

## Page Types

### 1. FAQ Hub Page

URL:

```text
/faq/
```

Purpose:

- Introduce the complete FAQ Center.
- Link to all 14 section pages.
- Surface P1 high-intent FAQs.
- Include search or filter UI if available.

Recommended title:

```text
Motorcycle FAQ Center for Importers, Dealers and Distributors
```

### 2. Section Pages

Example:

```text
/faq/pricing-moq-and-payment-faq/
```

Purpose:

- Introduce the broad topic.
- Link to all child group pages.
- Highlight the most commercially valuable P1 questions.

Schema:

```text
CollectionPage
```

### 3. Group Pages

Example:

```text
/faq/pricing-moq-and-payment-faq/motorcycle-wholesale-pricing/
```

Purpose:

- Introduce a specific FAQ cluster.
- List all related question pages.
- Provide a short buyer checklist.

Schema:

```text
CollectionPage
```

### 4. Question Pages

Example:

```text
/faq/pricing-moq-and-payment-faq/motorcycle-wholesale-pricing/how-much-does-a-wholesale-motorcycle-from-china-cost/
```

Purpose:

- Answer one buyer question clearly.
- Capture long-tail Google and AI-answer traffic.
- Convert readers into RFQ leads.

Schema:

```text
FAQPage
```

## Question Page Template

```markdown
# {H1 Question}

## Short Answer

Answer the question directly in 40-80 words.

## Detailed Explanation

Explain the commercial, technical, import, compliance, shipping, quality, or after-sales context.

## Key Factors Buyers Should Check

- Factor 1
- Factor 2
- Factor 3
- Factor 4

## RFQ Checklist

- Target model or motorcycle type
- Order quantity
- Destination country
- Required certification
- CBU, SKD, or CKD preference
- OEM/ODM requirements
- Shipping term: FOB, CIF, CFR, EXW, or DDP
- Spare parts and warranty requirements

## Related FAQ

Add 3-6 internal links from `internal_link_targets`.

## Next Step

Use the `primary_cta` from the CSV.
```

## SEO Rules

- Use the CSV `h1` as the visible H1.
- Use the CSV `seo_title_tag` as the browser title/meta title.
- Use the CSV `meta_description` as the meta description.
- Use the CSV `url_path` as the page path.
- Use the CSV `canonical_path` as canonical.
- Use one question per page.
- Do not use short topic labels as final question page titles.
- Add breadcrumbs on every page.
- Add FAQPage structured data on question pages.
- Add CollectionPage structured data on hub, section, and group pages.
- Link from every question page back to its group and section pages.
- Link from every group page to all child question pages.

## GEO Rules

GEO here means Generative Engine Optimization: structuring pages so AI answer engines can understand and quote the content.

For each question page:

- Put a direct answer immediately after the H1.
- Include the exact buyer question in the H1 and FAQ schema.
- Define important entities such as CKD, SKD, CBU, MOQ, FOB, CIF, EEC, COC, EPA, DOT, VIN, WMI, and warranty.
- Use comparison tables where buyers compare options.
- Use checklist sections for procurement and RFQ preparation.
- Mention limitations clearly, especially around country-specific regulations.
- Add internal links to related compliance, shipping, pricing, warranty, and supplier verification pages.
- End with an RFQ-oriented next step.

## Priority Rollout

Publish the pages in this order:

1. P1 question pages from `FAQ_SEO_GEO_UPLOAD_PLAN.csv`
2. All section pages from `FAQ_CATEGORY_URL_MAP.csv`
3. All group pages from `FAQ_CATEGORY_URL_MAP.csv`
4. P2 question pages
5. P3 long-tail support pages

P1 pages are the most likely to produce RFQ leads because they match buyer questions about price, MOQ, import documents, certification, CKD/SKD/CBU, supplier verification, warranty, spare parts, and distributor cooperation.

## First 20 Pillar FAQ Pages

These should be treated as primary SEO/GEO entry pages:

| Priority | H1 | URL |
| --- | --- | --- |
| P1 | How do I import motorcycles from China? | `/faq/import-and-certification-faq/import-documents/how-do-i-import-motorcycles-china/` |
| P1 | What documents are needed to import motorcycles from China? | `/faq/import-and-certification-faq/import-documents/what-documents-are-needed-import-motorcycles-china/` |
| P1 | What is the difference between CKD, SKD, and CBU motorcycles? | `/faq/ckd-skd-cbu-export-faq/cost-tax-and-container-loading-comparison/what-is-the-difference-between-ckd-skd-cbu-motorcycles/` |
| P1 | Which is cheaper: CKD, SKD, or CBU motorcycle import? | `/faq/ckd-skd-cbu-export-faq/cost-tax-and-container-loading-comparison/which-is-cheaper-ckd-skd-cbu-motorcycle-import/` |
| P1 | How many motorcycles fit in a 40HQ container? | `/faq/packing-and-shipping-faq/container-loading-quantity/how-many-motorcycles-fit-40hq-container/` |
| P1 | How many motorcycles can fit in a 40HQ container by CKD, SKD, and CBU? | `/faq/ckd-skd-cbu-export-faq/cost-tax-and-container-loading-comparison/how-many-motorcycles-fit-40hq-container-ckd-skd-cbu/` |
| P1 | What is the MOQ for wholesale motorcycles from China? | `/faq/pricing-moq-and-payment-faq/moq-requirements/what-is-the-moq-wholesale-motorcycles-china/` |
| P1 | How much does a wholesale motorcycle from China cost? | `/faq/pricing-moq-and-payment-faq/motorcycle-wholesale-pricing/how-much-does-wholesale-motorcycle-china-cost/` |
| P1 | What is total landed cost for motorcycle import? | `/faq/motorcycle-business-and-market-faq/profitability-and-investment-considerations/what-is-total-landed-cost-motorcycle-import/` |
| P1 | What trade term is better for motorcycle import: FOB, CIF, CFR, EXW, or DDP? | `/faq/pricing-moq-and-payment-faq/currency-banking-and-trade-terms/what-trade-term-better-motorcycle-import-fob-cif-cfr-exw-ddp/` |
| P1 | Can I put my own brand name on motorcycles from China? | `/faq/oem-odm-motorcycle-faq/private-label-motorcycle-branding/can-i-put-own-brand-name-motorcycles-china/` |
| P1 | How do I choose a reliable motorcycle manufacturer in China? | `/faq/china-motorcycle-supplier-guide/choosing-a-motorcycle-manufacturer-in-china/how-do-i-choose-reliable-motorcycle-manufacturer-china/` |
| P1 | Should I buy motorcycles from a factory or trading company in China? | `/faq/china-motorcycle-supplier-guide/manufacturer-vs-trading-company/should-i-buy-motorcycles-factory-trading-company-china/` |
| P1 | Are Chinese motorcycles reliable? | `/faq/china-motorcycle-supplier-guide/chinese-motorcycle-quality-and-reliability/are-chinese-motorcycles-reliable/` |
| P1 | What spare parts should importers buy with the first motorcycle shipment? | `/faq/spare-parts-and-warranty-faq/spare-parts-supply/what-spare-parts-should-importers-buy-first-motorcycle-shipment/` |
| P1 | What warranty do Chinese motorcycle manufacturers offer? | `/faq/spare-parts-and-warranty-faq/warranty-policy/what-warranty-do-chinese-motorcycle-manufacturers-offer/` |
| P1 | What is pre-shipment inspection for motorcycles? | `/faq/samples-inspection-and-factory-visit-faq/pre-shipment-inspection/what-is-pre-shipment-inspection-motorcycles/` |
| P1 | Can I import Chinese motorcycles into the United States? | `/faq/import-and-certification-faq/epa-dot-nhtsa-compliance/can-i-import-chinese-motorcycles-into-united-states/` |
| P1 | What is EEC or E-mark certification for motorcycles? | `/faq/import-and-certification-faq/eec-e-mark-coc-certification/what-is-eec-e-mark-certification-motorcycles/` |
| P1 | Can I become the exclusive motorcycle agent in my country? | `/faq/dealer-and-distributor-faq/exclusive-agency-cooperation/can-i-become-exclusive-motorcycle-agent-country/` |

## Internal Linking Model

Every question page should link to:

1. Parent group page
2. Parent section page
3. One pricing or MOQ page
4. One import/compliance page when regulation is relevant
5. One shipping or CKD/SKD/CBU page when logistics is relevant
6. One spare parts, warranty, or QC page when after-sales risk is relevant

Example for a pricing page:

```text
Question page:
/faq/pricing-moq-and-payment-faq/motorcycle-wholesale-pricing/how-much-does-a-wholesale-motorcycle-from-china-cost/

Internal links:
- /faq/pricing-moq-and-payment-faq/motorcycle-wholesale-pricing/
- /faq/pricing-moq-and-payment-faq/
- /faq/pricing-moq-and-payment-faq/moq-requirements/
- /faq/packing-and-shipping-faq/incoterms-fob-cif-cfr-exw/
- /faq/ckd-skd-cbu-export-faq/cost-tax-and-container-loading-comparison/
```

## Structured Data Example

Use JSON-LD on each question page:

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "How much does a wholesale motorcycle from China cost?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Wholesale motorcycle cost depends on engine size, configuration, certification, order quantity, packaging method, and trade term. Importers should compare FOB price, shipping cost, import duty, taxes, spare parts, inspection, and after-sales costs before calculating landed cost."
      }
    }
  ]
}
```

## Publishing Notes

- Keep URLs stable after upload.
- Avoid duplicate pages for the same question.
- If two questions are very similar, publish the stronger P1 question and use the weaker one as an H2 on the same page.
- Add canonical tags to prevent duplicate content.
- Add sitemap entries for all published URLs.
- Keep unpublished P2/P3 rows as `planned` until content is written.
- Review country-specific compliance pages with local import or legal specialists before publishing definitive statements.
