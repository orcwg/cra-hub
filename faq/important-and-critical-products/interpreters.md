---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/169
---

# Do programming language interpreters fall into the operating system category?

No. Interpreters, compilers and language runtimes are not among the important or critical product categories, and the lists only change by delegated act ([[CRA Article 7(3)]]). An interpreter is in the default category, like most products in scope: see [[important-and-critical-products/what-qualifies]].

The operating system category does not reach it. Implementing Regulation (EU) 2025/2392 describes operating systems as products _"that provide an abstract interface of the underlying hardware and control the execution of software"_ ([[CRA-CATEGORIES Annex I]]). An interpreter controls the execution of the programs it runs, but it runs on top of an operating system, which provides the interface to the hardware. Containing a component or having the functionalities of an important or critical product category doesn't place a product in that category if its core functionality is different ([[official/faq_3-4]], [[CRA-GUIDANCE point 141]], [[CRA-CATEGORIES Recital 5]]).

Neither the implementing regulation nor the guidance mentions interpreters, compilers or language runtimes. The Commission did list hypervisors and container runtime systems, in class II ([[CRA-CATEGORIES Annex I]]). ORC WG's comments on the descriptions are in [its input to the implementing regulation](https://github.com/orcwg/cra-hub/blob/main/product-definitions/input-to-draft-regulation.md).

The category only decides the conformity assessment procedure, not how much security work the product needs. The risk assessment and the essential requirements apply to every product in scope and scale with its own risk: the Commission's FAQ says that _"irrespective of whether the product with digital elements is considered to be an important or critical product"_, manufacturers carry out a comprehensive cybersecurity risk assessment ([[official/faq_3-3]], [[CRA Article 13(2)]]). An interpreter that much other software depends on still needs a thorough risk assessment, even though it can assess its own conformity under module A, like every product in the default category ([[official/faq_6-1]]): see [[manufacturers/self-assessment]].
