# FAQ Center Content Guide

This guide explains how to turn the FAQ Center taxonomy into publishable FAQ articles, category pages, and CMS records.

## Content Goals

The FAQ Center should help international motorcycle buyers answer practical pre-sales, import, compliance, customization, shipping, quality, and after-sales questions. Each article should be written for B2B buyers such as importers, distributors, fleet operators, dealers, and OEM/ODM partners.

## Recommended URL Structure

Use short, descriptive, lowercase slugs. Keep one stable URL per final FAQ topic.

```text
/faq/
/faq/{section-slug}/
/faq/{section-slug}/{group-slug}/
/faq/{section-slug}/{group-slug}/{topic-slug}/
```

Example:

```text
/faq/motorcycle-buying-guide/
/faq/motorcycle-buying-guide/motorcycle-types/
/faq/motorcycle-buying-guide/motorcycle-types/street-motorcycles/
```

## Content Model

Each FAQ topic should include these fields:

| Field | Purpose |
| --- | --- |
| `title` | Human-readable page title. |
| `slug` | Stable URL slug. |
| `section` | Top-level FAQ section. |
| `group` | Parent FAQ group. |
| `question` | Buyer-focused question. |
| `short_answer` | 40-80 word direct answer. |
| `full_answer` | Detailed explanation with buying/import context. |
| `recommended_for` | Buyer type, market, or use case. |
| `key_considerations` | Practical decision factors. |
| `related_topics` | Internal links to adjacent FAQ pages. |
| `cta` | Suggested next action, such as requesting a quotation or confirming compliance requirements. |

## Article Template

Use this structure for each FAQ topic page:

```markdown
# {Question}

## Short Answer

{Direct answer in plain language.}

## Details

{Explain the topic from the buyer's perspective. Include commercial, technical, import, or operating context when relevant.}

## Key Considerations

- {Decision factor 1}
- {Decision factor 2}
- {Decision factor 3}

## Recommended For

{Buyer profile, market, road condition, or business scenario.}

## Related FAQ

- [{Related Topic 1}]({url})
- [{Related Topic 2}]({url})
- [{Related Topic 3}]({url})

## Next Step

{Call to action.}
```

## Writing Guidelines

- Write for importers and distributors, not retail consumers only.
- Mention regional regulations carefully; advise buyers to confirm local rules before import.
- Prefer practical trade language: MOQ, FOB, CIF, CKD, SKD, CBU, homologation, spare parts, warranty, and after-sales support.
- Keep the short answer concise and make the detailed answer actionable.
- Avoid unsupported legal guarantees. Use phrases such as "usually", "commonly", and "depends on local requirements" when regulation varies by country.
- Cross-link topics that affect the same buying decision, such as engine displacement, road conditions, payload, spare parts, and certification.

## Category Page Template

Each top-level section and group page should introduce the topic and link to child FAQ pages.

```markdown
# {Section or Group Title}

{One-paragraph overview of what buyers can learn in this section.}

## Popular Questions

- [{Topic 1}]({url})
- [{Topic 2}]({url})
- [{Topic 3}]({url})

## All Topics

{Full list of child pages.}

## Need Help?

Contact the sales or export team with your market, order quantity, required model, and target import country.
```

## Priority Rollout

Prioritize articles that answer high-intent buyer questions and reduce sales friction.

### Priority 1: High Commercial Intent

- Motorcycle Wholesale Pricing
- MOQ Requirements
- Payment Terms
- CKD Motorcycle Kits
- SKD Motorcycle Export
- CBU Motorcycle Export
- Shipping Documents
- Container Loading Quantity
- Spare Parts Supply
- Warranty Policy
- Choosing a Motorcycle Manufacturer in China
- Avoiding Motorcycle Import Risks

### Priority 2: Import and Compliance

- Import Documents
- Customs Clearance Requirements
- EEC / E-mark / COC Certification
- EPA / DOT / NHTSA Compliance
- Homologation & Type Approval
- VIN / WMI / Registration Documents
- CKD / SKD / CBU Compliance
- Country Import Guides

### Priority 3: Product Selection and Technical Fit

- Motorcycle Types
- Engine Displacement Selection
- Motorcycle Use Cases
- Road Condition Selection
- Brake System
- Suspension & Tires
- Payload, Durability & Road Adaptability
- Fuel Consumption & Performance

### Priority 4: Partnership and Operations

- OEM / ODM Motorcycle FAQ
- Samples, Inspection & Factory Visit FAQ
- Quality Control FAQ
- Dealer & Distributor FAQ
- Motorcycle Business & Market FAQ

## Internal Linking Rules

- Link every buying guide article to at least one technical specification article.
- Link every import article to shipping documents, payment terms, and compliance topics.
- Link every OEM/ODM article to MOQ, samples, packaging, and quality control topics.
- Link every warranty article to spare parts supply, technical manuals, and after-sales support.
- Link country import guides to certification, road conditions, best-selling models, and distributor requirements.

## Example FAQ Drafts

### What is the difference between CKD, SKD, and CBU motorcycles?

**Short answer:** CBU motorcycles are exported as complete bikes, SKD motorcycles are partially disassembled, and CKD motorcycles are exported as parts kits for local assembly. The best option depends on import duty, local assembly capacity, container loading efficiency, and registration requirements.

**Key considerations:**

- CBU is simpler for buyers without an assembly workshop.
- SKD can reduce freight volume and suit markets with basic assembly capability.
- CKD is best for buyers with trained workers, tools, quality control, and local compliance approval.
- Import duties and local content policies often influence the final choice.

### What documents are usually needed to import motorcycles?

**Short answer:** Common import documents include the commercial invoice, packing list, bill of lading, certificate of origin, and product specification sheet. Some countries also require import permits, homologation documents, emission certificates, or road registration paperwork.

**Key considerations:**

- Document requirements vary by country and vehicle category.
- The buyer should confirm HS code, duty rate, and local certification rules before shipment.
- A customs broker can help verify import permits and tax calculations.

### How should buyers choose motorcycle engine displacement?

**Short answer:** Engine displacement should match road conditions, payload, fuel cost, and target users. 110cc and 125cc models are common for commuting and cost-sensitive markets, while 150cc to 250cc models are better for heavier loads, rural roads, mountain roads, or commercial use.

**Key considerations:**

- Lower displacement usually means lower fuel consumption and easier maintenance.
- Higher displacement provides stronger torque and better load performance.
- Local licensing, insurance, and registration rules may vary by engine size.

### What should buyers check before choosing a motorcycle supplier in China?

**Short answer:** Buyers should check factory qualification, production capacity, export experience, product range, quality control process, certification ability, and after-sales support. A supplier with proven export records and transparent technical documentation reduces import and warranty risk.

**Key considerations:**

- Request business license, export records, and certification documents.
- Review production lines, assembly process, and inspection standards.
- Confirm spare parts supply, warranty terms, and technical support before ordering.

### What affects motorcycle wholesale pricing?

**Short answer:** Motorcycle wholesale pricing depends on engine configuration, parts quality, certification requirements, order quantity, packaging method, raw material cost, exchange rate, and trade terms such as FOB, CIF, CFR, or EXW.

**Key considerations:**

- FOB and CIF prices include different cost responsibilities.
- OEM branding, special colors, and configuration changes may require MOQ.
- Quotation validity should be confirmed when exchange rates or material costs change.
