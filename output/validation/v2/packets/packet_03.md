# Sentence labelling task: geopolitical risk in 10-K risk factors

You will see sentences from the "Risk Factors" section (Item 1A) of U.S. annual reports. Judge each SENTENCE on its own. The previous sentence is shown only to help you understand it; do not label the context.

## Labels (0 or 1)

**geo** — 1 if the sentence refers to geopolitical risk: (a) war, armed conflict, military action or terrorism; (b) tensions, disputes or hostile measures between states or political actors, including trade wars, tariffs, sanctions, export controls and embargoes; (c) political instability, civil unrest, coups, expropriation or nationalisation in foreign countries; (d) named geopolitical events or relations (e.g., the Russia-Ukraine war, U.S.-China tensions). A list of risks counts if at least one item is geopolitical. Score 0 for natural disasters, pandemics, domestic regulation or taxes, domestic elections, generic "economic conditions", and cyberattacks without a state actor.

If geo = 0, set all other labels to 0. If geo = 1, also score:

**negative** — 1 if the sentence states an adverse consequence or threat for the company.
**mitigation** — 1 if it describes measures the company takes to manage or reduce the exposure (e.g., diversification, insurance, compliance programs, hedging, contingency plans).
**forward** — 1 if it refers to future developments, plans or expectations ("we expect", "in the future", "going forward", "will"). A purely hypothetical risk statement ("could adversely affect") is not enough.
**hedged** — 1 if it expresses uncertainty about likelihood, magnitude or timing ("may", "could", "uncertain", "cannot predict", "unclear").
**specific** — 1 if it names a specific country or region, conflict, sanction regime or trade measure, or a concrete channel of exposure (e.g., suppliers in a named country, revenue from a named region). Generic phrases such as "foreign countries" or "international operations" score 0.

## Output

Return one CSV block only, one row per sentence, in the order given, with this header:

sid,geo,negative,mitigation,forward,hedged,specific

No comments, no extra columns.

---

### s0101
Context (previous sentence): In addition, sales and purchases in currencies other than our subsidiaries functional currencies (primarily the USD, Euro, Chinese Renminbi and British Pound) expose the Company to fluctuations in foreign currencies relative to those functional currencies.
SENTENCE: Increased strength of the functional currency will decrease the Company’s reported revenues or margins in respect of sales conducted in 14 Table of Contents foreign currencies to the extent the Company is unable or determines not to increase local currency prices.

### s0102
Context (previous sentence): Changes in our products or changes in export, import and economic sanctions laws and regulations may delay us introducing new products in international markets, prevent our customers from using our products internationally or, in some cases, prevent the export or import of our products to or from certain countries altogether.
SENTENCE: The U.S. government has imposed significant tariffs on a variety of items imported from China.

### s0103
Context (previous sentence): Any such events may result in decreased product sales, lower product revenue, loss of revenue, and/or reputational damage, which would harm our results of operations and business.
SENTENCE: With respect to the pre-commercial distribution of eteplirsen to patients outside of the U.S., we have contracted with third party distributors and service providers to distribute eteplirsen in certain countries on a named patient basis and through our EAP.

### s0104
Context (previous sentence): We engage qualified construction firms to perform this work.
SENTENCE: However, if such firms experience delays, if they perform sub-standard work or if we fail to properly monitor the quality of their work or the timeliness of their progress, we may not be able to complete our construction projects on time.

### s0105
Context (previous sentence): In addition, we face business trend-related climate risks including the increased attention to ESG considerations by our clients in connection with their determination of whether to engage with us for our services.
SENTENCE: Our international operations are subject to certain risks, which may affect our revenue.

### s0106
Context (previous sentence): The impairment charge and intercompany loan transactions were non-cash in nature 36 and did not affect the Company’s current liquidity, cash flows or any debt covenants under the Company’s existing credit agreements.
SENTENCE: As part of HEI’s comprehensive review of strategic options for certain assets of Pacific Current, on February 7, 2025, Pacific Current entered into a Securities Purchase Agreement to sell all the membership interests in Hamakua Holdings, LLC, a wholly owned subsidiary of Pacific Current, to an unaffiliated third party for cash consideration to be determined under the provisions of the agreement.

### s0107
Context (previous sentence): The ultimate impact of the announced tariffs and any future tariffs will depend on various factors, including if such tariffs are ultimately implemented, the timing of implementation and the amount, scope and nature of such tariffs.
SENTENCE: If such increased or additional tariffs or other restrictions, quotas, embargoes, or safeguards are placed on goods imported into the U.S., or any related counter-measures are taken by other countries, we may have to raise our prices or increase inventory levels, or find new sources of components that we import, and our revenue, gross margins, and results of operations may be materially harmed.

### s0108
Context (previous sentence): In addition, the terminal modernization programs may not result in improved operational productivity or generate expected returns.
SENTENCE: Heightened security measures, war, actual or threatened terrorist attacks, efforts to combat terrorism and other acts of violence may adversely impact the Company’s operations and profitability.

### s0109
Context (previous sentence): Changes in our tax rates or tax provisions, adverse tax audits and other proceedings, or changes in tax laws or their interpretation or enforcement could have an adverse effect on our business, results of operations, effective tax rate and financial condition.
SENTENCE: We are subject to income taxes in the United States and in numerous foreign jurisdictions, notably in India where we have substantial operations.

### s0110
Context (previous sentence): Legal and Regulatory Risks 23 Table of Contents Privacy concerns and laws as well as evolving regulation of cloud computing, AI services, cross-border data transfer restrictions and other domestic or foreign regulations may limit the use and adoption of our services and adversely affect our business.
SENTENCE: Regulation related to the provision of services over the Internet is evolving, as federal, state and foreign governments continue to adopt new, or modify existing, laws and regulations addressing data privacy, cybersecurity, data protection, data sovereignty and the collection, processing, storage, hosting, transfer and use of data, generally.

### s0111
Context (previous sentence): The medical device industry is highly competitive.
SENTENCE: We compete with many domestic and foreign medical device companies ranging from small start-up enterprises that might sell only a single or limited number of competitive products or compete only in a specific market segment, to companies that are larger and more established than us, have a broad range of competitive products, participate in numerous markets and have access to significantly greater financial and marketing resources than we do.

### s0112
Context (previous sentence): Gaming continues to become increasingly social and streaming viewership is more widely adopted along with increasing numbers of content creators.
SENTENCE: This trend, which has accelerated in the past few years experienced a setback in 2022 primarily due to challenging macroeconomic conditions and the ongoing war between Russia and Ukraine.

### s0113
Context (previous sentence): As a consequence, the diamond business is subject to various sovereign risks beyond Signet’s control, such as changes in laws and policies affecting foreign trade and investment.
SENTENCE: In addition, Signet is subject to various political and economic risks, including the instability of foreign economies and governments, labor disputes, war and civil disturbances and other risks that could cause production difficulties or stoppages, restrict the movement of inventory or result in the deprivation or loss of contract rights or the taking of property by nationalization or expropriation without fair compensation.

### s0114
Context (previous sentence): These regulations have caused the Company to stop selling or servicing our products temporarily in restricted areas, such as Russia, Belarus and portions of Ukraine.
SENTENCE: The BIS and OFAC have also placed restrictions on dealing with certain "blocked” entities, such as Russia’s federal security service (FSB), including the Company’s filing of notifications to the FSB for exporting certain products to Russia.

### s0115
Context (previous sentence): Among other factors, it is possible that homeland security concerns, other catastrophic events or any change in government legislation governing insurance coverage for acts of terrorism could materially adversely affect available insurance coverage and result in increased premiums on available coverage (which may cause us to elect to reduce our policy limits) and additional exclusions from coverag
SENTENCE: Among other potential future adverse changes, in the future we may elect not to, or may not be able to, obtain any coverage for losses due to acts of terrorism.

### s0116
Context (previous sentence): Future spending and program authorizations may not increase or may decrease or shift to programs in areas in which we do not provide services or are less likely to be awarded contracts.
SENTENCE: Such changes in spending authorizations and budgetary priorities may occur as a result of shifts in spending priorities from defense-related and other programs as a result of competing demands for federal funds and the number and intensity of military conflicts or other factors.

### s0117
Context (previous sentence): Certain aspects inherent in transacting business internationally could negatively impact our operating results, including: ● costs and difficulties in staffing and managing international operations; ● costs and difficulties in staffing and managing international operations; ● legislative or regulatory requirements and potential changes in, or interpretations of, requirements in the United States a
SENTENCE: Dollar, which can affect demand for our products and increase our costs. ● fluctuations in foreign currency exchange rates against the U.S.

### s0118
Context (previous sentence): Recessions, economic downturns, inflation, slowing economic growth and social and political instability in the industries and/or markets where we compete could negatively affect our revenues and financial performance in future periods, result in future restructuring charges, and adversely impact our ability to grow or sustain our business.
SENTENCE: Macroeconomic and political instability caused by global supply chain disruptions, inflation and the strength of the U.S. dollar could adversely impact our results of operations.

### s0119
Context (previous sentence): The nature of the Company’s business exposes it to the potential for disputes, legal or other proceedings, and government inquiries or investigations relating to antitrust matters, labor and employment matters, personal injury and property damage, environmental, shore power and other matters, as discussed in the other risk factors disclosed in this section or in other Company filings with the SEC.
SENTENCE: For example, Matson is a common carrier, whose tariffs, rates, rules and practices in dealing with its customers are governed by extensive and complex foreign, federal, state and local regulations, which may be the subject of disputes or administrative or judicial proceedings.

### s0120
Context (previous sentence): Any material interruption in our supply chain, such as: material interruption of the supply of raw materials and components due to the casualty loss of any of our manufacturing plants; interruptions in service by our third-party logistic service providers or common carriers that ship goods within our distribution channels; unexpected delays in shipping or processing through customs of goods; incre
SENTENCE: Additionally, our raw materials and components are sourced from a wide variety of domestic and international business partners.

### s0121
Context (previous sentence): The Organization for Economic Cooperation and Development (“OECD”) released Pillar Two model rules defining a 15% global minimum tax for large multinational corporations.
SENTENCE: The OECD continues to release additional guidance and countries are implementing legislation with widespread adoption of the Pillar Two Framework expected in the near future.

### s0122
Context (previous sentence): Any security breach or system failure in such systems could result in an interruption of our customer’s operations, significant delays under a contract, and a material adverse effect on our results of operations.
SENTENCE: Our operations involve several risks and hazards, including potential dangers to our employees and to third parties that are inherent in aspects of our federal business (e.g., counterterrorism training services).

### s0123
Context (previous sentence): Consequently, during periods in which we sell this existing inventory, the effects of changing metal prices could adversely affect our operating results.
SENTENCE: Excess capacity and over-production by foreign metal producers or decreases in tariffs could increase the level of metal imports into the U.S., resulting in lower domestic prices, which would adversely affect our sales, margins and profitability.

### s0124
Context (previous sentence): The unauthorized reproduction, theft or misappropriation of our intellectual property could diminish the value of our brands or reputation and cause a decline in sales.
SENTENCE: Protection of our intellectual property and maintenance of distinct branding are particularly important as they distinguish our products and services from those of our competitors.

### s0125
Context (previous sentence): The strong growth in consolidated net premiums written in 2021 principally reflects growth in commercial lines of 17.7 percent, and more moderate but positive growth in consumer lines of 1.5 percent.
SENTENCE: Commercial lines, which includes reinsurance and agriculture, grew across most lines of business, driven by higher new business, positive rate increases, increased exposure, and strong renewal retention. • Commercial casualty grew globally, driven by higher new business and positive rate increases, primarily across North America, Europe and Asia.

### s0126
Context (previous sentence): Similarly, any claims, even if fully indemnified or insured, could negatively impact our reputation among our customers and the public and make it more difficult for us to compete effectively or obtain adequate insurance in the future.
SENTENCE: See Part I, Item 3 “Legal Proceedings” of this form 10-K and Note 16 The nature of our industry and assets makes us a target for terrorist activities designed to disrupt our ability to service our customers.

### s0127
Context (previous sentence): It also exposes us to the risk that certain minerals and metals, known as “conflict minerals”, that are contained in our products have originated in the Democratic Republic of the Congo or an adjoining country.
SENTENCE: As a result of the passage of the Dodd-Frank Wall Street Reform and Consumer Protection Act of 2010 (“Dodd-Frank”), the Securities and Exchange Commission (the “SEC”) adopted disclosure requirements for public companies whose products contain conflict minerals that are necessary to the functionality or production of such products.

### s0128
Context (previous sentence): Certain materials for our products are currently available from a limited number of suppliers and, as a result, we may have limited control over pricing, availability, and delivery schedules.
SENTENCE: Additionally, factors beyond our control, including adverse political conditions, trade embargoes, increased tariffs or import duties, inclement weather, natural disasters, terrorism and labor disputes may adversely impact our supply chain, particularly if these conditions or disputes result in work slowdowns, lockouts, strikes, facility closures, or related disruptions.

### s0129
Context (previous sentence): The allocations are generally based on premiums ceded under reinsurance contracts, adjusted for actual loss experience and historical relationships between gross and ceded losses.
SENTENCE: If actual premium and loss experience vary materially from historical experience, the allocation of reinsurance recoverable by reinsurer will be reviewed and may change.

### s0130
Context (previous sentence): The U.S.
SENTENCE: Bureau of Industry and Security (“BIS”) enacted broad trade restrictions with respect to Huawei (which represented approximately 10% of our revenue in the fourth quarter of 2020 and 12% in 2019) that took effect on September 15, 2020 and currently prevent us from shipping products to Huawei.

### s0131
Context (previous sentence): Unfavorable currency fluctuations could reduce our royalty income and revenues.
SENTENCE: While we attempt to minimize our foreign currency risks, our risk management strategies may not be effective and our results of operations and financial condition could be adversely affected.

### s0132
Context (previous sentence): Even in the absence of direct physical damage to our hotels, the occurrence of any natural disasters, terrorist attacks, military actions, outbreaks of diseases, or other casualty events, may have a material adverse effect on our business, the impact of which could result in a material adverse effect on our financial condition, results of operations and our ability to make distributions to our sto
SENTENCE: Terrorist attacks and military conflicts may adversely affect the hospitality industry.

### s0133
Context (previous sentence): Further, our headquarters are located in Santa Barbara, California, in a seismically active region that is also prone to forest fires.
SENTENCE: Any catastrophic event that occurred near our headquarters, or near our manufacturing facilities in China, could impose significant damage to our ability to conduct our business and could require substantial recovery time, which could have an adverse effect on our business, operating results and financial condition.

### s0134
Context (previous sentence): Our insurance coverage may not be adequate to cover all the costs related to cybersecurity attacks or disruptions resulting from such events.
SENTENCE: We operate internationally and are subject to exchange rate fluctuations, exchange controls, political risks and other risks relating to international operations.

### s0135
Context (previous sentence): While we believe we have been successful to date in diversifying our Advanced Products customer base beyond early adopters, we cannot assure you our strategy will be successful and further diversification of customers will be achieved. 15 We also have filed “duty drawback” applications with U.S.
SENTENCE: Customs and Border Protection for the recovery of Section 301 Tariffs paid on raw materials and components used to produce products we subsequently exported.

### s0136
Context (previous sentence): We operate in a number of jurisdictions that pose a high risk of potential FCPA violations, and we participate in relationships with third parties whose actions could potentially subject us to liability under the FCPA or local anti-corruption laws.
SENTENCE: In addition, we cannot predict the nature, scope or effect of future regulatory requirements to which our international operations might be subject or the manner in which existing laws might be administered or interpreted. 46 Table of Contents We are also subject to other laws and regulations governing our international operations, including regulations administered by the U.S.

### s0137
Context (previous sentence): The same would be true in situations where we are required to share our exclusivity period with other ANDA sponsors with Paragraph IV certifications.
SENTENCE: In the EU and other countries and regions, there is no exclusivity period for the first generic product.

### s0138
Context (previous sentence): Failure to comply with these rules and regulations may result in substantial civil and criminal penalties, including fines and the disgorgement of profits, the imposition of a court-appointed monitor, the denial of export privileges and debarment from participation in U.S. government contracts, any of which could have a material adverse effect on our international operations or on our business, re
SENTENCE: Additionally, in connection with the ongoing conflict between Russia and Ukraine, the U.S. government has imposed enhanced export controls on certain products and sanctions on certain industry sectors and parties in Russia.

### s0139
Context (previous sentence): Public health issues such as a major epidemic or pandemic could adversely affect our business and financial results.
SENTENCE: The U.S. and other countries have experienced, and may experience in the future, outbreaks of contagious diseases that affect public health and public perception of health risk.

### s0140
Context (previous sentence): Any such difficulties noted above could effect our business.
SENTENCE: Sales of our foreign operations were $20,754,000, $15,421,000 and $33,906,000 in fiscal years 2021, 2020 and 2019, respectively.

### s0141
Context (previous sentence): War, terrorist attacks and other acts of violence may cause consumer confidence and spending to decrease, or may affect the ability or willingness of tourists to travel to Hawaii, Guam or Alaska, thereby adversely affecting those economies and the Company.
SENTENCE: Additionally, future terrorist attacks could increase volatility in the U.S. and worldwide financial markets.

### s0142
Context (previous sentence): In addition, we have incurred, are incurring and will incur in the future, costs and capital expenditures to comply with environmental, health and safety laws and regulations.
SENTENCE: For example, w e have several product lines that rely on lead-based solder and many others that historically did so.

### s0143
Context (previous sentence): The degree of containment of the virus, and the recovery in travel, has varied country by country.
SENTENCE: During the recovery period, there have been instances where cases of COVID-19 have started to increase again after a period of decline, which in some cases impacted the recovery of travel in certain countries.

### s0144
Context (previous sentence): Setting aside the circumstances of any given year or period, however, customer and product mix have contributed to the decline of our gross profit percentage over time and, based on the anticipated sources of our future growth, will likely continue to reduce our gross profit percentage into the foreseeable future.
SENTENCE: In 2025, tariff rates increased on many of the parts we sell.

### s0145
Context (previous sentence): While we regularly assess the likelihood of adverse outcomes from such examinations and the adequacy of our provision for income taxes, there can be no assurance that such provision is sufficient and that a determination by a tax authority will not have an adverse effect on our results of operations and cash flows.
SENTENCE: We are exposed to fluctuations in currency exchange rates, which could negatively affect our financial condition and results of operations Our sales contracts are denominated in U.S. dollars, and therefore, substantially all of our revenue is not subject to foreign currency risk.

### s0146
Context (previous sentence): Other products are subject to the International Traffic in Arms Regulations, which restrict the export of information and material that may be used for military or intelligence applications by a foreign person.
SENTENCE: U.S. regulators have announced “export control reform” that has changed and is expected to change many of the rules applicable to us in this area in the future in ways we do not yet fully understand and we have experienced and will continue to experience challenges in complying with the new rules as they become effective, resulting in difficulties or an inability to ship products to certain countries and customers.

### s0147
Context (previous sentence): In addition, regulators or legislators could limit our ability to charge adequate pricing for catastrophe exposures or shift more responsibility for covering risk.
SENTENCE: Terrorism is an example of a significant man-made caused potential catastrophe.

### s0148
Context (previous sentence): We may be required to expend significant capital and resources to address any breaches, protect against such threats or to alleviate problems caused by security breaches.
SENTENCE: Globally, the frequency, severity and sophistication of cybersecurity incidents have increased, and these trends will likely continue, especially during times of geopolitical tension or instability among countries from which a number of recent cybersecurity events have been alleged to have originated.

### s0149
Context (previous sentence): Moreover, such products could also be regulated as both drugs and cosmetics simultaneously, as the categories are not mutually exclusive.
SENTENCE: The statutory and regulatory requirements applicable to drugs are extensive and require significant resources and time to ensure compliance.

### s0150
Context (previous sentence): Import duties and tariffs vary by country and a different tariff classification for any of our products may result in higher duties or tariffs, which could have an adverse impact on our operating results and potentially increase the cost of the related products to our customers. 28 Table of Content s Our business and industry are subject to various laws and regulations that could adversely affect 
SENTENCE: Our business and industry are regulated under various federal, state, local and international laws.