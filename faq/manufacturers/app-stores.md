---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/252
---

# Are free app store listings considered 'making available on the market' under the CRA?

A free app store listing is _making available on the market_ only if you supply the app in the course of a commercial activity, that is, if you monetise it in some way. Listing an open source app that you do not monetise is not, however many people download it.

What counts is the commercial activity, not the price. The CRA defines _making available on the market_ as supplying software _"for distribution or use on the Union market in the course of a commercial activity, whether in return for payment or free of charge"_, and _placing on the market_ as the first time that happens ([[CRA Article 3(22)]], [[CRA Article 3(21)]]). Commercial activity is a condition of the definition, not a consequence of it: when [[CRA Recital 15]] says the CRA applies to products _"made available on the market, hence supplied for distribution or use on the Union market in the course of a commercial activity"_, the words after "hence" restate the whole definition, commercial activity included. Reaching users in the EU is not commercial on its own.

For open source software, the CRA says outright that providing it without monetising it _"should not be considered to be a commercial activity"_, and the regular releases that a store listing implies do not change that ([[CRA Recital 18]], [[CRA-GUIDANCE point 42]]). The test applies to each product and to the person supplying it, not to the platform ([[CRA-GUIDANCE point 11]], [[CRA-GUIDANCE point 50]]), so it makes no difference that the store also carries paid or closed-source apps. A free, unmonetised open source app on an app store is therefore in the same position as the same app offered from your own website: outside the CRA.

A free listing does count as making available on the market when the free download is how you monetise something else. The Commission's guidance gives three examples of apps that are _"available free of charge"_ and nevertheless placed on the market ([[CRA-GUIDANCE point 54]]):

- a marketplace app through which its publisher earns advertising, commission or subscription fees ([[CRA-GUIDANCE Example 14]]);
- a VPN app whose users can pay for extra servers or dedicated IP addresses, that is, in-app purchases or a paid service reached through the app ([[CRA-GUIDANCE Example 15]]);
- a fitness app whose use is conditional on processing personal data for targeted advertising or analytics ([[CRA-GUIDANCE Example 16]]).

Charging for the app itself, for its binaries, or for a version whose updates or support are only available to paying users is a sale ([[CRA-GUIDANCE point 51]], [[CRA-GUIDANCE point 57]]). In all of these cases the app is placed on the market the first time it is offered in the store, every later download is a further making available ([[CRA-GUIDANCE point 13]], [[CRA-GUIDANCE point 14]]), and you are its manufacturer, _"whether for payment, monetisation or free of charge"_ ([[CRA Article 3(13)]]). See [[cra-itself/monetisation]] for the forms monetisation can take, and [[maintainers/monetization]] for what does and does not count as earning from your project.

The store itself does not change the answer. The sole act of hosting software on open repositories, package managers or collaboration platforms _"does not in itself constitute the making available on the market"_ ([[CRA Recital 20]]), and in the guidance's example of an individual's free library on a public package repository, neither the developer nor the repository has obligations under the CRA ([[CRA-GUIDANCE Example 34]]).

If you are an individual, an unmonetised app is outside the CRA altogether. If you are a company or foundation, it is not placed on the market, but you may be its _open-source software steward_, with lighter obligations, if the app is intended for commercial activities ([[CRA-GUIDANCE point 43]], [[CRA-GUIDANCE point 53]]): see [[maintainers/solo-maintainer-steward]] and [[stewards/what-is-a-steward]].

Two related points. The part of [[CRA Recital 18]] about components _"intended for integration by other manufacturers"_ is about libraries and other building blocks, not end-user apps; an app you publish to users is covered by the general rule above, that unmonetised open source is not a commercial activity (see [[projects/binaries]] for components). And a free app that is not open source cannot rely on that rule: for it, whether the supply happens in a business-related context is assessed case by case, taking into account the regularity of the supplies, the characteristics of the product and the intentions of the supplier, with occasional supplies by hobbyists not normally considered business-related (section 2.2 of the Blue Guide, recalled in [[CRA-GUIDANCE point 40]]): see [[cra-itself/freeware]].
