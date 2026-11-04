---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/169
---

# Do programming language interpreters fall into the operating system category?

No. Interpreters, compilers and language runtimes are not among the important or critical product categories, and the lists are exhaustive; the Commission can add a category only by delegated act ([[CRA Article 7(3)]]). An interpreter is in the default category, like most products in scope: see [[important-and-critical-products/what-qualifies]].

The operating system category does not reach it. Implementing Regulation (EU) 2025/2392 describes operating systems as products _"that provide an abstract interface of the underlying hardware and control the execution of software"_ ([[CRA-CATEGORIES Annex I]]). An interpreter controls the execution of the programs it runs, but it runs on top of an operating system and relies on it for the interface to the hardware. The Commission's guidance says a product that _"may have the ability to perform the functions of an important or critical product category, but nonetheless have a core functionality different from that of such a product category"_ is not in it ([[CRA-GUIDANCE point 141]], [[CRA-CATEGORIES Recital 5]]).

Neither the implementing regulation nor the guidance mentions interpreters, compilers or language runtimes, so this is a reading of the descriptions, not an official answer. The execution environments the Commission did list are hypervisors and container runtime systems, in class II ([[CRA-CATEGORIES Annex I]]); whether interpreters ought to join them is a question for the Commission, and ORC WG's comments on the descriptions are in [its input to the implementing regulation](https://github.com/orcwg/cra-hub/blob/main/product-definitions/input-to-draft-regulation.md).

The category only decides the conformity assessment procedure, not how much security work the product needs. The risk assessment and the essential requirements are the same for every product in scope and scale with the product's own risk: the Commission's FAQ says that _"irrespective of whether the product with digital elements is considered to be an important or critical product"_, manufacturers carry out a comprehensive cybersecurity risk assessment ([[official/faq_3-3]], [[CRA Article 13(2)]]). An interpreter that a great deal of other software runs on still needs a thorough risk assessment, and the requirements that follow from it, even though it can assess its own conformity: see [[manufacturers/self-assessment]].
