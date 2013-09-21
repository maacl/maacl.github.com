---
layout: post
title: "An Acceptable EULA?"
date: 2010-06-04 12:00
comments: true
external-url:
categories: [license, law, copyright, drafting, eula]
alias: "index.php/2010/06/04/an-acceptable-eula/"
---
Is there such a thing? Until today I did not think so, but after having
watched Mixergy's
[interview](/web/20100907205218/http://mixergy.com/balsamiq-peldi-guilizzoni-interview/)
with Balsamiq’s Giacomo “Peldi” Guilizzoni, I was optimistic that I
might have finally found one. Check Balsamiq’s EULA out
[here](/web/20100907205218/http://www.balsamiq.com/images/BalsamiqEula.pdf).
Peldi mentions in the interview that a helpful customer in-house counsel
gave him some great feedback that helped improve the license. To
whatever she told him, I would add the following:

#### Preamble

Don’t use “represents and warrants” use only “represents”. The form is
needless legalese and part of the reason why people hate lawyers. If you
don’t agree read
[this](/web/20100907205218/http://www.adamsdrafting.com/2009/09/18/rs-and-ws-once-more-with-feeling/)
– then go change it.

#### Definitions

“Authorized Users” and “Authorized User” – makes no sense that the
plural form would have a completely different meaning than the singular.
“Authorized Users” is never used in the EULA. This might make sense when
read together with the Quote/Receipt/Invoice but I doubt it. The
definitions of “Authorized Machine” and “Authorized Server Node” do not
appear to deal well with virtual environments.

#### Section 3 Grant of License

The license granted is “irrevocable” but at he same time terminable by
Balsamiq as per section 12. This appears inconsistent. “(except pursuant
to Clause 12 below)” should be added after “irrevocable”.

#### Section 4 No Warranty

Excluding all warranties does not strike me as compatible Balsamiqs
mission to produce high quality software. You can’t claim to aim for
excellence in everything you do, and the refuse to back it up – that’s
simply not credible. On the other hand warranties provided for goods are
not appropriate for software, as these are calibrated for defects that
occur in individual instances (copies) of the product. I would suggest a
warranty that better correspond to the apparently fanatical customer
service Balsamiq provides. This does no mean warranting to fix bugs
within a certain timeframe, but it does mean warranting a meaningful
response to reported bugs etc. If you are doing it already it such a
warranty is essential free, if you make sure that the customers remedies
if you fail are manageable. If such remedies for instance only apply to
the (first) reporter of the bug, you contain the effect of the warranty
from spreading to all customers.

#### Section 6.1 Software Maintenance – For Plug-in Versions

Excellent to see inclusion of a reasonable price-escalation clause for
Software Maintenance. This is something that I have had to negotiate
many times and which any prudent licensee should always remember. You
don’t want to be
[treated](/web/20100907205218/http://www.zdnet.com/blog/howlett/sap-pulls-the-trigger-on-higher-support-costs/442)
like SAP’s customers, do you?

#### Section 9 Investigation of Unauthorized Use and Distribution

This is a very pragmatic alternative to audit rights which especially a
company the size of Balsamiq would have very little use for. The
fairness of allocating the cost of producing the certificate to the
licensee should be considered, since this might exceed the license fee
by a factor of many in some cases. I would consider some kind of
compensation (free maintenance?) to the customer if a request for a
certificate is made and this is provided, as this is would indicate that
Balsamiqs suspicion was not well-founded.

#### Section 10 (a) Licensee’s Restrictions

Very common provision which is also very unenforceable in the EU if the
motif for the reverse engineering is a desire to “achieve the
interoperability of an independently created computer program with other
programs” (thanks to art. 5 and 6 of this
EU [directive](/web/20100907205218/http://eur-lex.europa.eu/LexUriServ/LexUriServ.do?uri=CELEX:31991L0250:EN:HTML)).

#### Section 10 (b) Licensee’s Restrictions

Appears superfluous. How would the customer ever unilaterally be able to
vary the “Authorized Use”? That said there might be a technicality in
California law that makes it prudent to include this.

#### Section 10 (d) and (e) Licensee’s Restrictions

WTF! I can’t refer to Balsamiq’s name or do anything that has a
“material and adverse effect on Balsamiq’s” interests. I am glad that I
did not license Balsamiq’s software before writing this post. How can
you promote Balsamiq as an open organisation in continuous dialog with
its customers, and then muffle the same audience with your EULA?

#### Section 12 – Termination

The destruction of all copies of the software is a practical
impossibility in many enterprise environments due to the back-up
strategies employed. Since this will only become a requirement in case
of a breach it might be justified nonetheless, but a more balanced
alternative might be to require the destruction of all “readily usable
copies” of the software or similar.

#### Section 13 – Infringement Indemnification

For the software in question and taking into account the size of the
vendor (Balsamiq) this is a very reasonable clause, and it is a wise
move to include indemnification if you want to have any hope selling
your software to enterprise customers.

#### Section 14 – Limitation of Liability

Good to see that the indemnification obligations are exempted from the
limitation of liability.

#### Section 16 – Open Source Code

For Balsamiq’s present product I wouldn’t worry much about the “viral”
nature of the GPL and other similar licenses, which is clearly what this
section is meant to address, but the section clearly does no harm
either. If the software was meant for combination with the customer’s
code or other software and subsequent distribution, I would be more
interested in the list of of open source products/licenses in Exhibit A
as this would enable me to assess any challenges related hereto.

#### Section 17 – Publicity Rights

This section solves a very common problem in a fairly practical way (the
customer can opt out of Balsamiqs right to use the customer for
publicity purpose prior to or any time after purchase) but a better more
honest and straight forward solution, would be to permit the customer to
opt out via the web form used to purchase the product.

#### Section 24 – Notices

While not critical why appear unreasonable by biasing this section in
Balsamiqs favour? On Export Control (especially US) you really want to
provide the relevant export control classification codes if you expect
any one to comply with the rules. In general you want to try to avoid
having your software subject to US export control rules as these are
absolutely not trivial.

On balance Balsamiq’s EULA is above average but still suffers from a few
weakness as outlined above. Most of these can be fixed without exposing
Balsamiq to any liability that is unmanageable.

DISCLAIMER: Above is not legal advice bla, bla, bla.
