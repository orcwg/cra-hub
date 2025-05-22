**EG CRA – OSS work strand – real world use cases from the industry (collected via VDMA, VDW)**  
April 15, 2025

**Role/view:** 	manufacturer of a final product with digital elements, where OSS is not the main activity.

**Why it matters:** 	European manufacturers should take advantage of OSS in the future, therefore guidance and clarification based on real world use cases should be provided.

**Note:**	Questions provided come from manufacturers and are included to give full view on the use cases.

**UseCase 1**  
(e.g. open62541 SDK)

The manufacturer of the final product with digital elements integrates an open-source software component.   
This OSS component is maintained by a not-for-profit entity.  
Maintenance is funded by public money (research projects) and donations from users or projects to develop new features.

Questions:

* What is the role of the manufacturer of the final product and the not-for-profit entity?  
* What is the role of both if a certain feature was developed in a project between the  
  manufacturer and the not-for-profit?

**UseCase 2**  
(e.g. .NET SDK – OPC Foundation)

A not-for-profit foundation develops an OSS software development kit (SDK) with a GPL-2 license.   
This SDK is used by manufacturers of the final product to build products with digital elements.  
Maintenance of the SDK is funded by membership fees to the not-for-profit foundation and provided by developer resources from its members. This same SDK is also provided to the members using a non-OSS license.

Questions:

* Who is responsible for this SDK?  
* Who is responsible for providing patches and maintaining a vulnerability disclosure process?  
* How is liability structured for these scenarios?

**UseCase 3**  
(e.g. library from the package systems NPM, PyPi, NuGet)

A manufacturer of the final product with digital elements uses open-source libraries from the large package ecosystems as a component in the product.

Questions:

* What are the obligations for proper due diligence before a manufacturer may integrate such libraries?  
* What is the manufacturer ‘s liability for such a library?  
* May the manufacturer only use libraries which have an Open-Source Stewart or where there is a responsible manufacturer for the library?

**UseCase 4**  
(e.g. providing a library which one uses in their product also as open source to be reused)

A manufacturer provides a product with digital elements to the European market. The manufacturer needs to develop a new software library on its own to use it as a component in the product with digital elements. The software library is also made available under an open-source license to be used by others, without charging a prize for it.

Questions:

* What are the manufacturers obligations, does he automatically become manufacturer for this library with all obligations?

Special case: The manufacturer develops a software library to interact with its product. This library is provided under an open-source license as is, as a sample implementation to interact with the product. How can the manufacturer ensure that this library is not a product with digital elements? Otherwise it would not be published.

**UseCase 5**  
(e.g. providing software implementations as a demo software under an open-source license)

A not-for-profit association, where manufacturers of products used as components are members, is developing sample software which showcases the use of industry standards (e.g. OPC UA) and how various components from different manufacturers can work together.  
The not-for-profit association also runs a test bed which is publicly accessible to showcase certain use cases and  
provide guidance.

Questions:

* How can it be ensured that the not-for-profit association does neither become an Open-Source Steward nor a manufacturer for sample implementations?

**UseCase 6**  
(e.g. manufacturer providing code as a demo software under an open-source license)

A final product manufacturer directly provides sample computer code (e.g. python script, C code, PLC code...) which showcases the use and integration of its products with digital elements.

Questions:

* How is the manufacturer classified regarding the demo software, as a manufacturer or as a steward? If as an OSS steward, what are the obligations on sample code/implementations?

**UseCase 7**  
(e.g. embedded device as part of a product with custom build operating system)

Yocto is a toolkit for building operating system distributions for embedded systems. Operating systems are classified as "important". An embedded device manufacturer leverages the Yocto toolkit to build a custom operating system for the product with digital elements (used as a component).

Questions:

* What does the use of a customized OS mean for the embedded device manufacturer that uses the toolkit to build a custom OS for its embedded device?  
* Does this mean the embedded device manufacturer is building an operating system and has the obligations to fulfil all requirements according to the CRA important product class of Operating Systems?

