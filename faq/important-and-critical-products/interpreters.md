---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/169
---

# Do programming language interpreters fall into the operating system category?

No. Interpreters, compilers and language runtimes are not among the important or critical product categories, and the lists are exhaustive; the Commission can add a category only by delegated act ([[CRA Article 7(3)]]). An interpreter is in the default category, like most products in scope, unless its own core functionality matches a listed category: see [[important-and-critical-products/what-qualifies]].

The operating system category does not reach it. Implementing Regulation (EU) 2025/2392 describes operating systems as products _"that provide an abstract interface of the underlying hardware and control the execution of software"_, with services such as resource management, scheduling, input-output control and the interface through which applications reach system resources and peripherals ([[CRA-CATEGORIES Annex I]]). An interpreter controls the execution of the programs it runs, but it does not provide the interface to the hardware: it runs on top of an operating system and relies on it for that. The Commission's guidance says a product that _"may have the ability to perform the functions of an important or critical product category, but nonetheless have a core functionality different from that of such a product category"_ is not in it ([[CRA-GUIDANCE point 141]], [[CRA-CATEGORIES Recital 5]]), and that a product whose core functionality falls substantially short of a category's is not classified in it ([[CRA-GUIDANCE point 142]]).

Neither the implementing regulation nor the guidance mentions interpreters, compilers or language runtimes, so this is a reading of the descriptions, not an official answer. The execution environments the Commission did list are hypervisors and container runtime systems, in class II ([[CRA-CATEGORIES Annex I]]).

Whether interpreters ought to be listed is a question for the Commission; ORC WG's comments on the technical descriptions are in [its input to the implementing regulation](https://github.com/orcwg/cra-hub/blob/main/product-definitions/input-to-draft-regulation.md). For the conformity assessment the default category allows, see [[manufacturers/self-assessment]].
