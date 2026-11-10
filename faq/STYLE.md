# FAQ Style Guide

How to write a FAQ for the CRA Hub. The file format, the reference syntax, lists and pull requests are described in the [contributing guidelines](./README.md); this guide covers the writing.

The rules here are for text being written. They are not a reason to reword a FAQ the task force has approved: see [Review](./README.md#review).

## Contents

- [Who the FAQs are for](#who-the-faqs-are-for)
- [The question](#the-question)
- [The answer](#the-answer)
- [Language](#language)
- [Sources](#sources)
- [What is settled and what is not](#what-is-settled-and-what-is-not)
- [Links and citations](#links-and-citations)
- [Tables](#tables)
- [Lists](#lists)
- [Terms](#terms)

## Who the FAQs are for

The people who have to act on the answer: maintainers, contributors, developers at companies that ship software, foundation staff. Not lawyers, not policy people. They want to know what applies to them and what to do. Most haven't read the regulation, so an answer has to make sense without it.

- Address the reader as "you" and "your project".
- Lead with the practical consequence, then the reason.
- A FAQ never speaks of "the hub", "we" or "our reading". It states its answer, and the silence of the sources where that matters.
- UK spelling (monetisation, organisation).
- Professional and concise. No disclaimer that the FAQ is not legal advice: the site adds one to every FAQ.

## The question

The question is the FAQ's single `#` heading. Ask it the way the reader would: in the first person ("Does accepting donations make me a manufacturer?"; "we" for an organisation), in the words they would use, not the regulation's. The answer then addresses them as "you".

One question per file. Two small FAQs, each with its own question, are better than one that answers both: each is found by the question it answers, read in one go, and linked to from where its question arises.

The filename is a short, informative slug: lowercase, hyphens (`patent-royalties.md`).

## The answer

### Shape and size

A FAQ is an inverted pyramid: the direct, complete answer first; then the main condition or clarification; then supporting detail only where it improves understanding. The same order holds inside a sentence: the point, then its qualifications.

- 120 to 300 words of answer, usually about 200, in three to five paragraphs.
- The answer in one or two sentences; the official source that settles it, quoted and cited; then only what that source leaves open, one idea per paragraph; links to the FAQs that answer the next questions.
- One bullet list at most.
- Shorter is fine: a question an official source settles in a sentence is a FAQ of 80 words, not padded to 200.
- A FAQ past 300 words is answering two questions, or arguing a point an official source already settled. Split it or cut the argument.

### The first sentence carries the question

The first sentence stands on its own when quoted, shown in a list or read out of context. A bare "Yes.", "No." or "It depends." is not a first sentence; neither is background. Nor is a reply that only makes sense after the question: "No, not once a version has reached its end of life.", "On 11 December 2027, all of them.", "Neither."

The test: read the first sentence alone. If it doesn't say what was asked, make it a full sentence whose subject is the thing the question is about. A "Yes." or "No." may open the paragraph, followed by that sentence. The echo can be light: enough of the question's words that a reader knows what was asked, not the question repeated.

| Question | Not this | This |
|---|---|---|
| Does accepting donations make me a manufacturer? | No. | No, receiving donations does not make you a manufacturer, as long as those donations cover your actual costs rather than generate profit. |
| What does 'actual costs' mean under the CRA? | The legitimate expenses of designing, developing, maintaining and providing software. | Under the CRA, 'actual costs' are the legitimate expenses of designing, developing, maintaining and providing software. |
| When do the steward obligations start to apply? | On 11 December 2027, all of them. | The steward obligations all start to apply on 11 December 2027. |
| Is stewardship something you opt in to, or can you be designated as a steward? | Neither. | Neither: your organisation is an open-source software steward when it meets the definition, by what it does. |
| Do a steward's reporting obligations cover vulnerabilities in obsolete versions? | No, not once a version has reached its end of life. | A steward's reporting obligations do not cover a version once it has reached its end of life. |
| What qualifies a product as an important or critical product? | Having the core functionality of a listed category. | A product is an important or critical product when its core functionality is that of a category the CRA lists. |
| What do I need to set up before I can report through the single reporting platform? | An EU Login account for each person who will report. | Before you can report through the single reporting platform, each person who will report needs an EU Login account. |
| Does the steward regime apply to organisations outside the EU? | Yes. Where your organisation is based does not matter. | Yes, the steward regime applies to organisations outside the EU: where your organisation is based does not matter. |
| Am I subject to the CRA if I earn a living from the open source project I maintain? | It depends on your relationship to the project. | Not as long as what you earn from the project only covers your actual costs, which include a reasonable salary or living expenses. |
| What is an open-source software steward? | The CRA defines a steward as… | An open-source software steward is a company or foundation that systematically supports an open source project meant for commercial use. |

### Say who and what the answer is about

A FAQ is read on its own, from a search result or a link, without the list it sits in or the FAQ before it. So it names its subject outright instead of inheriting it from the category:

- which role it is about: an individual maintainer, a contributor, an open-source software steward, a manufacturer, a company that integrates the project;
- which kind of thing: an open source project that is not monetised, a monetised version, a commercial product, a component built into one.

"You" is pinned to one of these in the first paragraph, and a FAQ that switches role or subject says so at the switch: "Penalties only come into play if you monetise your project, which makes you its manufacturer".

Watch for a sentence true of one role being written as if it were true of all: "you may be treated as a manufacturer or steward" assumes the reader could be an organisation. A maintainers FAQ addresses an individual, and sends the organisation to the stewards FAQs.

The test: read the FAQ with its category hidden, and check that every "you", "project" and "product" still has one clear referent.

## Language

### Everyday words

A reader who has never heard of the CRA should be able to follow. No legal or policy jargon where an ordinary word does: "sell" rather than "place on the market", "company or foundation" rather than "legal person", "has to" rather than "is obliged to", "the EU" rather than "the Union". If a sentence would sound at home in the regulation, rewrite it.

Use the CRA's own terms only when the answer turns on them ("product with digital elements", "open-source software steward", "placing on the market"): in italics the first time, with the plain meaning next to them. Otherwise "open source project", "software", "maintainer", "company", "selling". A citation carries the legal precision; the sentence doesn't have to. The [terms](#terms) at the end of this guide give the plain words for the most common ones.

### Sentences readers can follow as they read

Avoid structures that make the reader hold one part of a thought while several clauses go by before they can see how it fits:

- Keep subject and verb close together. Don't bury the main action behind qualifications.
- Don't stack clauses inside clauses. Break a sentence with several nested ideas into simpler sentences, or rearrange it.
- Put modifiers next to what they modify. The reader shouldn't have to work backwards to find what a phrase refers to.
- Main point first, qualifications after.

The goal is not shorter sentences as such. It is sentences whose structure lets readers understand them on first reading, without going back to reconstruct the meaning. A sentence that stacks a rule, its condition, its exception and a quotation fails that test, however many words it has.

Two checks catch most failures:

1. **Count the words between a subject and its verb**, and restructure past about five. "A project that declares a version's end of life where users will see it draws that line itself" has nine; "The project itself decides which versions are still covered, by declaring…" has none.
2. **Make every "this", "that line", "it" point at something in the same or the previous sentence.** A rewrite often deletes an antecedent and leaves the pronoun behind.

Run both on every sentence of the finished FAQ, and again on each sentence a later edit touches: a sentence written to fix one rule is the one most likely to break another.

A definition with several parts is a sentence per part, or one sentence with the parts separated by semicolons.

> **Before:** Your organisation is a steward when it meets the definition, by what it does, not by declaring itself one or being named one: a company or foundation (a legal person), other than a manufacturer, that has the purpose or objective of systematically providing sustained support for specific open source software intended for commercial use, and that ensures its viability.
>
> **After:** Your organisation is a steward when it meets the definition. What counts is what it does, not whether it calls itself a steward or someone names it one. The definition has four parts: a company or foundation (a legal person); other than a manufacturer; whose purpose is to systematically provide sustained support for specific open source software intended for commercial use; and which ensures that software's viability.

### Say the thing

A FAQ states what the sources say and what follows from them. It doesn't comment on its own reasoning or soften it.

- **No hedges and no filler.** Cut "it is worth noting", "it should be noted", "importantly", "in practice", "arguably", "generally speaking", "the short answer is", "on that reading", and any sentence whose only job is to say how sure the FAQ is. What to write where a point really is unsettled: [What is settled and what is not](#what-is-settled-and-what-is-not).
- **No frames that announce a point instead of making it.** Their shape is a sentence whose subject is a clause or an abstraction standing in for the point: "what makes this hold is", "what this turns on is", "what counts is", "the key point is", "the answer lies in". The test is the subject: if it is "what …", "the thing that …", "the point", "the line", the sentence is announcing. Say the thing, with its real subject: "The project itself decides which versions are still covered, by declaring a version's end of life where users will see it", not "What makes this hold is saying which versions are maintained".
- **No sentence that announces the structure of the sentences after it**: "Each part in turn.", "Taking these one by one:", "There are three cases." Delete it and start on the first part.

### Assertive about the law, not towards the reader

Plain assertion is for what the CRA and the official sources say. It is misplaced when the FAQ turns to what the reader has to do: a FAQ informs, it does not give orders. Not "Say which versions are maintained." or "Create the accounts now.", but what follows for the reader and what helps, with the reason: "Accounts created before they are needed mean nobody is setting one up during the 24 hours you have". Advice stays in the indicative, with its reason attached.

## Sources

### Official sources come first

Read, in this order: the Commission's FAQs and ENISA's; the Commission's guidance; the CRA articles and recitals the question turns on; the related FAQs in the hub. The issue and its discussion are context and often settle what the answer should say, but they are not an authority.

Where the Commission's FAQ, its Q&A, ENISA's FAQ or the Commission's guidance answers the question, the FAQ says so first and rests on it. What follows adds only what the official source leaves open: how it applies to open source, to the situation the issue describes, or to the next question.

- Don't rebuild from the CRA's text an argument an official source has already settled, and don't present your own reasoning as if it were the authority.
- Where an official source contradicts the issue thread or an existing FAQ, the official source wins; say so.
- Don't write a FAQ that would only restate an official one. Add the official one to the [list](#lists) instead.
- Stay close to what the issue settled and to the sources. Don't introduce interpretations of your own.

### Assert the rule in plain words; the citation carries the authority

What an official source settles is stated as a fact, in the FAQ's own words, with the citation after it:

> Containing a component or having the functionalities of an important or critical product category doesn't place a product in that category if its core functionality is different (`[[official/faq_3-4]]`, `[[CRA-GUIDANCE point 141]]`).

Not:

> The Commission's FAQ says a product _"that has the ability to perform the function(s) of an important or critical product category but whose core functionality itself is different from that of such product category is not to be considered to have that core functionality"_.

### Quoting

Quote only where the exact words matter, and only the decisive words: a phrase, not a sentence of the regulation's prose. One quote per FAQ, in the paragraph that rests on the official source, is usually enough; everything else is paraphrased and cited.

Quotes are in italics, with the citation after: `_"quoted material"_ ([[CRA Recital 15]])`. Where a source says something differently from a contributor's draft, use the source's wording.

### Citing

- Only cite provisions you have read in the source; never from memory.
- Prefer Articles and Annexes over Recitals: Recitals explain, Articles bind. Cite a Recital for context, next to the Article.
- The Commission's guidance is the Commission's interpretation: authoritative but non-binding. Cite it by section or point for anything interpretive, and say "the Commission's guidance" where the answer rests on it.
- An official FAQ that answers the question is cited where the answer is given, in the first sentence or right after it, not buried among supporting citations.
- "Guidance" means the Commission's guidance. For anything else say "information", "clarification", "details".

## What is settled and what is not

A reader should be able to tell a rule from an interpretation, and an interpretation from an open question, without the FAQ softening its sentences. Each case has its own way of being written:

| The point is… | Write it as |
|---|---|
| Stated by the CRA | A plain statement, with the Article cited. |
| The Commission's or ENISA's interpretation | A plain statement, with the guidance point or official FAQ cited. Name the source in the sentence ("the Commission's guidance says") where the answer rests on it. |
| An exception or a condition | Its own sentence, after the rule it qualifies, with its own citation. |
| Not addressed by any source | One plain sentence saying so, once: "Neither the implementing regulation nor the guidance mentions interpreters." Then the answer reasoned from the CRA, without apology. |
| Unresolved, and needing the Commission to settle it | `Status: 🛑 Pending Guidance`, with a `guidance-id` naming the request in `pending-guidance/`. |
| Not yet reviewed by the task force | `Status: ⚠️ Draft`. |

The silence of the sources is a fact to state, not a reason to qualify every sentence after it.

## Links and citations

The syntax is in the [contributing guidelines](./README.md#references).

### Citation or linked phrase

A double-bracket reference can show as a citation ("Article 25 of the CRA") or as a phrase of your choosing (`[[CRA Article 25 | security attestations]]`).

- **Keep the citation visible** where the reader needs to know which provision supports a claim. This is the usual case for a legal source.
- **Link a phrase** where the reader mostly needs the explanation behind a term, and the sentence reads better with the term than with a citation: "This may count as `[[cra-itself/monetisation | an intention to monetise]]`."

### Point to other FAQs instead of repeating them

Each FAQ answers its own question and links to the FAQ that answers the next one, rather than restating that answer. Before writing a paragraph, check whether a FAQ already covers it. If so, give a short summary of the key takeaway and the link:

> Donations only make you a manufacturer when donating is really the price of the software: see `[[maintainers/donations]]`.

The reader shouldn't have to click through to follow the answer, and shouldn't find the other FAQ's argument repeated here. The same fact written twice at length drifts apart at the first edit.

A pointer is a sentence, written the plain way: "For more information on what does trigger manufacturer obligations, see `[[maintainers/become-manufacturer]]`", "Donations are covered in `[[maintainers/donations]]`". Not a fronted clause ("For what does make you a manufacturer, see …"), and not a label with a colon standing in for a sentence ("What helps them: …", "What a CSIRT is: see …"). The sentence reads as prose if the link is removed.

## Tables

A table is for an answer that is the same question asked of several cases (which dependencies count, which obligations apply at which support level): one row per case, a column for what the case covers and one for what follows, short cells.

- A table's sources go in footnotes below it (`[^1]: [[CRA Article 13(5)]], [[official/faq_4-3-6]]`), one marker per cell that needs one, not in the cells. `stewards/duties/notification-obligations.md` shows the pattern.
- A table is written in a neutral register: third person, "the manufacturer", "the product", no "you" and no asides. The prose around it addresses the reader; the table states the rule.
- The prose stays within the usual size; the table is on top of it.

## Lists

A category's `README.yml` is the order a reader meets its FAQs in. A list that grew one issue at a time reads like one, so a list is revisited as it grows. How lists and sublists are declared: [contributing guidelines](./README.md#lists).

### Order

Read the list top to bottom as a newcomer, one FAQ after the other, the way the site shows them. Note every place where an entry assumes something a later entry explains, two entries answer the same question, or the question a reader has next is not the next entry.

The order is the order the questions arise:

1. what the thing is and whether it applies to the reader;
2. what it requires of them;
3. the situations where the plain rule bends;
4. consequences and enforcement;
5. what comes next, with the FAQs of other categories that continue the story.

Each FAQ should read on what came before and never need one that comes after. Put the question most readers arrive with first, not the definition: "Do all open source projects have a steward?" before "What is a steward?".

### Splitting

A list that stops being one story gets split: a category past fifteen entries, or one that answers two audiences (maintainers who might be stewards; foundations that are). Each strand becomes a sublist, or a new category when the strand is a subject of its own. A FAQ that belongs to two lists is listed from both, not copied.

### Official FAQs and gaps

Where the Commission's or ENISA's FAQ answers a question readers of the category have and no hub FAQ does, list the official one at the point where the question falls. A hub FAQ that applies an official answer to open source goes right after the official entry it builds on.

The walk-through also shows what is missing: the question a reader has between two entries that neither answers, the edge case the issues keep raising, the obligation stated but never explained. Each gap is an issue labelled `faq`, unless an official FAQ already fills it.

### Descriptions

A list's `description` is shown on its card in the FAQ index and at the top of its page. Its job is to let a reader decide, in a glance, whether the list is for them.

A reader decides that by recognising their own situation and seeing what they will come away with. So a good description speaks to the reader about where they stand, in the words they would use about themselves, and says what the list will tell them. It sounds like a person pointing them to the right shelf, not like a table of contents: the entries sit right below it and already show what the list covers.

How it does that is up to the writer. One way that works is to put the reader's situation to them as a question, then say what they will find:

> You write, contribute to or maintain open source software? Here is what the CRA asks of you, and what it doesn't.

> Your software relies on cloud or other remote services? Here is when those services count as part of the product under the CRA.

Things that tend to get in the way:

- naming a topic instead of a reader ("Understanding product categories", "Essential information about …");
- the CRA's label for the reader where they wouldn't yet know it applies to them;
- a summary of the entries;
- length: a card holds a sentence or two.

A sublist's description does the same job within its parent: it tells the parent's readers which of them it is for.

One constraint is technical: no colon followed by a space (see [Lists](./README.md#lists) in the contributing guidelines).

## Terms

Use the same words for the same thing in every FAQ. The plain words are the default; the CRA's term appears, in italics, where the answer turns on it. The last column is the FAQ that explains the term: link to it rather than explaining it again.

| The CRA's term | Plain words | Explained in |
|---|---|---|
| _product with digital elements_ | software, product, device | `cra-itself/scope` |
| _placing on the market_, _making available on the market_ | selling, releasing | `cra-itself/placing-on-the-market` |
| _commercial activity_, _intention to monetise_ | monetising, making money from | `cra-itself/monetisation` |
| _actual costs_ | actual costs | `cra-itself/actual-costs` |
| _manufacturer_ | manufacturer | `manufacturers/what-is-a-manufacturer` |
| _open-source software steward_ | steward, after the full term once | `stewards/what-is-a-steward` |
| _legal person_ | company or foundation | `legislation/legal-person` |
| _due diligence_ | due diligence | `due-diligence/what-is-due-diligence` |
| _market surveillance authorities_ | the authorities that enforce the CRA | `cra-itself/market-surveillance-authorities` |
| the Union | the EU | |
| is obliged to, shall | has to | |
| guidance | the Commission's guidance only | |

"Open source" is written without a hyphen ("open source project", "open source software"), except in the CRA's term _open-source software steward_.

Add a row when a FAQ introduces a term other FAQs will need.
