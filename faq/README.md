# FAQ Contributing Guidelines

## Goals

1. Include questions in the FAQs as soon as they are identified; do not wait for an answer to solidify before adding them to the repository.
2. Make drafting the answers an iterative process; it is better to have an approximate answer than none, provided the answer is clearly identified as such (see next point).
3. Clearly identify the [maturity level](#maturity-level) of each answer.
4. Improve accuracy, consistency, and quality of answers through a more rigourous [final review process](#review).


## Maturity level

The maturity level of the answers contained in the FAQ are indicated using the following system:

| Maturity level status | Icon | Description |
| :-------------------- |:----:| :---------- |
| Draft                 |  ⚠️  | Hasn't been reviewed by the FAQ TF. Answer may be incomplete or incorrect. |
| Pending Guidance      |  🛑  | Identified by the FAQ TF as requiring input from the EU Commission. |
| Approved              |  ✅  | Has been reviewed by the FAQ TF. Represents community best effort to provide an actionable answer. |

### Questions which would benefit from European Commission guidance

FAQs which would benefit from guidance from the European Commission include a `pending-guidance` field in their YAML frontmatter that references a dedicated guidance request file in the `pending-guidance/` folder.

Example:
```yaml
---
Status: ⚠️ Draft
guidance-id: legal-person-definition
Related issues: https://github.com/...
---
```

## Review

The FAQ TF Review should check for the following:

- [ ] There are no objections about the inclusion of the question
- [ ] There are no objections about the provided answer
- [ ] The question and answer follow the same structure as the rest of the FAQ
- [ ] The tone is similar
- [ ] The answer is accurate
- [ ] The answer is properly sourced and referenced

## Lifecycle

FAQs follow the below lifecycle:

```mermaid
flowchart TD
    issue@{ shape: stadium, label: "New GitHub issue"} 
    draft[Status: ⚠️ Draft]
    pending[Status: 🛑 Pending Guidance]
    approved@{ shape: stadium, label: "Status: ✅ Approved"}
    iterate["Iterate on draft"]
    review{"Passes review?"}
    guidance{"Requires EU guidance?"}
    
    issue -- Identify question --> draft
    draft --> iterate
    iterate -- Ready for review --> review
    review -- YES --> guidance
    review -- NO --> iterate
    guidance -- NO ----> approved
    guidance -- YES --> pending
    pending -- Receive guidance --> iterate
```

## Format

There is one question per file.

The filename should be a short but informative slug.

All FAQ files are stored in subdirectories of the `faq` directory.

## Guidance Requests

The `pending-guidance/` folder contains dedicated files for EU Commission guidance requests that are referenced by multiple FAQs.

### File format

All files are markdown files with YAML frontmatter.

Please use [reference style links][].

```md
---
Status: [ICON] [MATURITY_LEVEL]
Related issues: [URL]
---

# [QUESTION]

[SHORT ANSWER]

[ADDITIONAL NUANCES]

[LINKS]
```



## References

### Cross-References

To reference FAQs, just use relative links as you normally would so:

**Examples:**
```markdown
[FAQ Title](../category/faq.md)
[FAQ Title](./same-category-faq.md)
```

### Auto-linking to CRA articles, recitals, and annexes

Use double-bracket notation, prefixed with `CRA`, to auto-link to CRA articles, recitals, and annexes:

```markdown
[[CRA Article 24]]
[[CRA Article 3(14)]]
[[CRA Recital 19]]
[[CRA Annex III]]
```

**Examples:**
```markdown
As described in [[CRA Article 9]], the Expert Group provides guidance.
Stewards are defined in [[CRA Article 3(14)]] as legal persons.
See [[CRA Recital 19]] for additional context on commercial activities.
```

The prefix can be left out (`[[Article 24]]`), but write it: it keeps CRA references consistent with references to other texts.

### Auto-linking to other EU legal texts

Prefix the reference with the number of the act to link to an article, recital, or annex of another EU legal text:

```markdown
[[2022/2555 Article 12(1)]]
[[2024/2853 Recital 15]]
```

The best-known texts can also be referenced by a short key: `CRA`, `PLD`, `NIS2`, `DORA`, `AI-ACT`, and `CRA-CATEGORIES` (Implementing Regulation (EU) 2025/2392, the technical description of the important and critical product categories).

```markdown
[[NIS2 Article 12(1)]]
[[PLD Recital 15]]
[[AI-ACT Annex III]]
[[CRA-CATEGORIES Annex I]]
```

Both forms render as "Article 12(1) of the NIS 2 Directive". The act must be listed in [the website's index of EU legal texts][eu-reg]; to add one, or give it a short key, open a pull request there.

### Several citations in a parenthesis

A parenthesis holding nothing but citations, separated by commas, renders in a short form grouped by document and part, with each citation still its own link:

```markdown
([[CRA Recital 15]], [[CRA-GUIDANCE point 58]], [[CRA-GUIDANCE point 61]])
```

renders as "(CRA Recital 15, Guidance points 58 and 61)"; a single citation in a parenthesis renders as "(CRA Article 5)", and an act without a short key by its number, "(2019/1020 Article 5)". Anything else in the parenthesis, such as "see", keeps the long form: "(see Article 5 of the CRA)".

### Auto-linking to the Commission's CRA guidance

Prefix the reference with `CRA-GUIDANCE` to link to a section, point, example, or figure of the [Commission's guidance on the application of the CRA][official guidance]:

```markdown
[[CRA-GUIDANCE Section 3.2.4]]
[[CRA-GUIDANCE point 71]]
[[CRA-GUIDANCE Example 1]]
[[CRA-GUIDANCE Figure 1]]
```

**Example:**
```markdown
Donations that exceed actual costs indicate monetisation ([[CRA-GUIDANCE Section 3.2.4]]).
```

### External References

1. References to an EU legal text as a whole should link to its landing page on EUR-Lex, for example: https://eur-lex.europa.eu/eli/reg/2019/2144/oj
2. Use standard reference-style links for all other external references

[eu-reg]: https://github.com/orcwg/cra.orcwg.org/blob/main/src/_data/eu-reg.json
[official guidance]: https://cra.orcwg.org/official-guidance/


[reference style links]: https://www.markdownguide.org/basic-syntax/#reference-style-links
