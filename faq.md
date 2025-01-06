# CRA FAQ

## The Cyber Resilience Act (CRA) itself

#### Q: What is the Cyber Resilience Act (CRA)?

The Cyber Resilience Act (CRA) is a new EU Regulation that aims to safeguard consumers and businesses who use software or products with a digital components. It creates mandatory cybersecurity requirements for manufacturers and retailers that extend throughout the product lifecycle and the whole software supply chain (including all open source dependencies ans transitive dependencies) and helps consumers and business identify such products through the CE mark.

#### Q: Where is the official text of the CRA?

The final text of the CRA can be found on [EUR-Lex][CRA] ([English HTML version][CRA HTML]).

#### Q: When does the CRA enter into force and when does the regulation start to apply?

The CRA enters into force on December 11, 2024. Reporting obligations of manufacturers ([Article 14][]) start to apply on September 11, 2026.
The notitifcation of conformity of assement bodies ([Chapter IV][]) start to apply on June 11, 2026. Everything else starts to apply on December, 11 2027.


## Open source projects

#### Q: What criteria determine whether an open source project is in scope of the CRA?

#### Q: Is distributing binaries or container images of an open source project considered as making it available on the market?

No. Monetization by the original manufacturer is what determines whether a product is made available on the market. As per [Recital 18][], merely supplying open source components isn't indicative of a commercial activity:

> Furthermore, the supply of products with digital elements qualifying as free and open-source software components intended for integration by other manufacturers into their own products with digital elements should be considered to be making available on the market only if the component is monetised by its original manufacturer. […] In addition, the mere presence of regular releases should not in itself lead to the conclusion that a product with digital elements is supplied in the course of a commercial activity.

## Maintainers

#### Q: Am I subject to the CRA if I only contribute to an open source project?

No. Contributions to an open source project are explicitely not in scope of the CRA. See [Recital 18][]: 

> This Regulation does not apply to natural or legal persons who contribute with source code to products with digital elements qualifying as free and open-source software that are not under their responsibility.

## Open-Source Software Stewards

#### Q: What is an _open-source software steward_?

_Open-source software steward_ is a term defined in [Article 3(14)][] of the CRA. It describes an organization which supports open source software but isn't itself a commercial actor (e.g. an open source foundation):

> ‘open-source software steward’ means a legal person, other than a manufacturer, that has the purpose or objective of systematically providing support on a sustained basis for the development of specific products with digital elements, qualifying as free and open-source software and intended for commercial activities, and that ensures the viability of those products;

#### Q: Can an solo maintainer be considered to be an _open-source software steward_?

#### Q: Can a loosely organized group of maintainers be considered to be an _open-source software steward_?

## Manufacturers

#### Q: What is a _manufacturer_?

The term _Manufacturer_ is defined in [Article 3(13)][] of the CRA:
	
> ‘manufacturer’ means a natural or legal person who develops or manufactures products with digital elements or has products with digital elements designed, developed or manufactured, and markets them under its name or trademark, whether for payment, monetisation or free of charge;

#### Q: Can a _manufacturer_ also be an _open-source software steward_?

Yes, a _manufacturer_ can also be an _open-source software steward_, but it cannot be both the _manufacturer_ and _open-source software steward_ of the same project.

## EU Legislation

#### Q: What is the _Blue Guide_?

#### Q: What is the _New Legislative Framework_ (NLP)?

#### Q: What is a _Harmonized Standard_ and why does it matter?

#### Q: What is a _legal person_?

[CRA]: https://eur-lex.europa.eu/eli/reg/2024/2847/oj
[CRA HTML]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847
[Recital 18]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#rct_18
[Article 3(13)]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_3
[Article 3(14)]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_3
[Article 14]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_14
[Chapter IV]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#cpt_IV
