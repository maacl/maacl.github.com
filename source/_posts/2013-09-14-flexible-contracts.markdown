---
layout: post
title: "Flexible Contracts"
date: 2013-09-14 12:00
comments: true
external-url:
categories: [contracts, law, drafting]
---
<h4 id="/posts/20130914000000.markdown"></h4>

It was suggested to me to look into the concept of [Flexible Contracts](http://flexiblecontracts.com/), a new approach to contracting for agile it projects championed by Gabrielle Benefield who will be providing training in agile practices in connection with [goto Aarhus 2013](http://gotocon.com/aarhus-2013/).

Flexible Contracts are born out of the observation that traditional contract models are a very poor fit for agile IT projects. This is hardly a novel observation, but Gabrielle's work (and that of her collaborators) distinguishes itself by actually having produced a practical alternative, which they have commendably licensed under the [CC Attribution 3.0 Unported license](http://creativecommons.org/licenses/by/3.0/). Only the lite version - Flexlite 0.1 as it is designated - appears to be presently available, and can be accessed if you are willing to sign up to the Flexible Contracts mailing list [here](http://flexiblecontracts.com/list/).

It is worth noting that the overview attached to the contract clearly states that the Flexlite contract is to be considered a "minimum viable contract", but after having reviewed the document I still find that the current version lacking in a number of ways.

Below I will outline a subset of the issues I have identified and for some suggests some possible remedies. Please note that I am commenting on the UK version (which you might want to keep handy if you want to make sense of my comments) of the contract which is the system of law I am most familiar with, but most of my comments should apply to both versions, with the exception of the issue of "best endeavours" where there is a significant difference between US and UK law.

##Statetment of Target Outcomes (SOTO)

The contract focuses on the use of SOTOs instead of specifying the desired results through requirements or a more traditional solution specification. A SOTO:

> means a statement of target outcomes as agreed by the parties in accordance with clause 1.1;

According to clause 2.2 the Supplier must for each Target Outcome create:

> Options that have the potential to achieve the Target Outcome.  In respect of each Option the Supplier shall provide a forecast in terms of the estimated value, costs, risks and expiry date (if any) for that Option and shall inform the Customer of any requirements for execution of the Option and any circumstances in which the Option may expire.

Even after reading the overview it remains unclear exactly what the function of the Options are and what, if any, the work-flow for calling these are.

It appears odd that acceptance (adoption) of the Outcome Delivery is left to the Supplier but I assume this is considered reasonable given that one of the objectives of the Flexible Contract is to provide as much flexibility to vendor in deciding in how to achieve the SOTO. I don't think any customer would be comfortable with this construct, especially if the Supplier's payment hinges in part on achieving the Target Outcomes, which is one of the models (option B) suggested in the model SOTO schedule attached to the contract. Clause 2.7 isn't much help in this context, as 2.7. (a) is stating the obvious and (b) lacks fundamental precision. As such in can easily be interpreted as granting the Customer defacto veto rights against any Outcome Delivery, which is hardly constructive either.

Related to this issue is the lack of consistency between clause 3.1 which states that:

> In consideration of the provision of the Services by the Supplier, the Customer shall pay the fees in the amount and on the dates or with the frequency as set out in each SOTO.

and the "Hybrid Outcome-based fees" model in the model SOTO schedule, where payment is conditioned upon achieving the Target Outcomes.

##Best Endeavours

I also find it fundamentally concerning that the contract relies on a unqualified "best endeavours" standard when defining the Suppliers responsibility under the contract. It is simply not good practice not to agree some further specification of what the parties intend "best endeavours" to mean. This can for instance be done by indicating what financial/resources the Supplier must expend in its attempt to fulfill its obligation. Failing to provide such guidance is to invite conflict and to introduce unnecessary uncertainty. While I applaud the authors stated aim of brevity this is not an area where one wants to sacrifice lack of precision for terseness. I have included a few links below that provides more in-depth information on the subject.

##Intellectual Property Rights (IPR)

The IPR as specified in clause 5 model appears fairly sensible and reflects the reality of the deliverables being a composite of bespoke, vendor, third party proprietary and FOSS. That said the specific license granted to the Customer in respect of Supplier Software (clause 5.4) will in many cases have to be adapted to the needs of the Customers, both in respect of scope but also rights to create derived works etc. I would suggest moving the specification of this license to the SOTO schedule to facilitate this. This also applies to the specification of what types of software (Customised, Supplier, Third Party, Open Source) will constitute part of the Outcome Delivery, so the Customer may determine the feasibility of the rights obtained and clear any necessary rights.

While the contract does provide a warranty for non-infringement in respect of the Services and Outcome Delivery it does not address the issue of indemnification for such infringement, which any prudent customer will require.

The above is a summary of some of the issues I have identified with the current draft of the Flexlite contract. I summation I think the contract does a good job of capturing the idea of an outcomes focused contract, but unfortunately it does so at the expense of the customers position under the contract should things not go as planned.

I hope to have the opportunity to discuss Flexible Contracts with Gabrielle during [goto Aarhus 2013](http://gotocon.com/aarhus-2013/) and do one or more follow posts on Flexible Contracts.

Links regarding best endeavours:

["All reasonable endeavours" a lesser obligation than "best endeavours"](http://www.ashfords.co.uk/news/reasonable_endeavours_aug10)

[Best and EffortsCase Analysis and Practical Guidance Under U.S. and U.K. Law](http://www.jonesday.com/best-efforts-and-endeavourscase-analysis-and-practical-guidance-under-us-and-uk-law-07-30-2007/)

[My delicious links about "best endeavours"](https://delicious.com/flatspace/endeavours)

Full Disclosure:  I am receiving a free GOTO ticket from the producers in exchange for blogging about the conference.


