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

### s0351
Context (previous sentence): We have operations in Canada, Mexico, the European Union, and Asia, and our vendors, independent manufacturers, and licensees are located around the world.
SENTENCE: The value of the U.S. dollar against other foreign currencies has experienced significant volatility in recent years.

### s0352
Context (previous sentence): Ongoing international trade disputes and changes in trade policies could also impact economic activity and lead to a general contraction of customer demand.
SENTENCE: In addition, tariffs on components that we import from China or other nations that have imposed, or may in the future impose, tariffs will adversely affect our profitability unless we are able to exclude such components from the tariffs or we raise prices for our products, which may result in our products becoming less attractive relative to products offered by our competitors.

### s0353
Context (previous sentence): If the conditions arising from such events persist or worsen, they could materially and adversely affect our results of operations and financial condition.
SENTENCE: The occurrence of catastrophic events ranging from natural disasters (such as hurricanes, fires, floods, and earthquakes), acts of war or terrorism, accidents involving our travel offerings or experiences, the effects of climate change, including any impact of global warming, or the prospect of these events could disrupt our business.

### s0354
Context (previous sentence): In addition to selling our products directly to customers, we also sell to distributors who, in turn, sell our products to third parties.
SENTENCE: Inventory levels at our distributors may increase or decrease as a result of various factors, including end customer demand, new customer contracts, the influence of competition, political and socio-economic climate, contractual obligations related to minimum inventory levels, changing perceptions, including those of alternative products, our ability to renew distribution contracts with expected terms, our ability to implement commercial strategies, regulatory restrictions, armed conflicts, unexpected customer behavior, proactive measures taken by us in response to shifting market dynamics and procedures and environmental factors beyond our control, including weather conditions or an outbreak of infectious disease such as COVID-19 or diseases carried by farm animals such as African Swine fever.

### s0355
Context (previous sentence): These laws and regulations restrict our ability to collect, transfer and use certain personal data, absent an application to and, in some cases, approval from relevant governmental authorities in China.
SENTENCE: Additional regulations, guidelines, and measures relating to data privacy and data protection are expected to be adopted, including more guidance from industry sector regulators on the catalogues of important data and publication of implementation rules for certifications for cross-border transfers of personal information out of China, which may contain additional requirements for transferring personal information out of mainland China.

### s0356
Context (previous sentence): Plaintiffs did not appear for depositions in the United States as of April 26, 2013.
SENTENCE: Defendant CACI Premier Technology, Inc. then renewed its motion for sanctions, seeking dismissal, for the three Plaintiffs’ violation of the Court order to appear for depositions and medical examinations.

### s0357
Context (previous sentence): As a result, competitors may be better able to adapt to changes in conditions in our industries, fluctuations in the costs of raw materials or changes in global economic conditions.
SENTENCE: Competitors may also be able to introduce new products with enhanced features that may cause a decline in the demand and sales of our products.

### s0358
Context (previous sentence): Ablecom and Compuware are both privately-held Taiwan-based companies.
SENTENCE: In addition, we have entered into a distribution agreement with Compuware, under which we have appointed Compuware as a nonexclusive distributor of our products in Taiwan, China and Australia.

### s0359
Context (previous sentence): Failure to fully pass any such increased prices and costs through to our customers or to modify our activities to mitigate the impact would have an adverse effect on our operating income.
SENTENCE: We are exposed to foreign currency exchange rate risk, and changes in foreign exchange rates could increase the cost of purchasing products and impact our foreign sales.

### s0360
Context (previous sentence): As a result, we may incur higher state income tax expense in the future.
SENTENCE: Depending on our future tax position, continued suspension of our ability to use NOL carryforwards in states in which we are subject to income tax could have an adverse impact on our results of operations and financial condition.

### s0361
Context (previous sentence): Risks Relating to Information Technology and Cybersecurity ● Cybersecurity attacks on any of our vessels, facilities, or those of third parties, may result in potential liability or reputational damage or otherwise adversely affect our business. ● Cybersecurity attacks on any of our vessels, facilities, or those of third parties, may result in potential liability or reputational damage or otherwis
SENTENCE: Risks Relating to Our Securities ● Our common stock is subject to restrictions on foreign ownership and possible required divestiture by non-U.S.

### s0362
Context (previous sentence): In addition, many of our customers rely heavily on international trade.
SENTENCE: The imposition of tariffs, duties, border adjustment taxes or other trade restrictions by the United States could also result in the adoption of new or increased tariffs or other trade restrictions by other countries.

### s0363
Context (previous sentence): There is significant uncertainty over potential changes in consumer behavior and shopping patterns as the pandemic continues and as different regions experience surges.
SENTENCE: Currently, there is also a rapidly developing Russia-Ukraine conflict, which has already escalated into a significant military confrontation, and is resulting in major, potentially prolonged economic sanctions and other responses from the United States and other countries, which present significant risks and uncertainties.

### s0364
Context (previous sentence): As such, we face risks in doing business globally.
SENTENCE: For example, while our corporate headquarters are located in California, additional key engineering, sales, and administrative personnel are located in China, Germany, Japan, Malaysia, Philippines, Singapore, Switzerland, Taiwan and elsewhere in the U.S., and our manufacturing operations are primarily located in Germany, Japan, Malaysia, Philippines and the U.S.

### s0365
Context (previous sentence): Income tax authorities regularly perform audits of our income tax filings.
SENTENCE: Income tax audits associated with the allocation of income and other complex issues, including inventory transfer pricing and cost sharing, product royalty and foreign branch arrangements, may require an extended period of time to resolve and may result in significant income tax adjustments.

### s0366
Context (previous sentence): For example, building codes implemented in Washington, if determined to be valid, would have the effect of restricting or eliminating the use of gas space and water heating in new commercial and residential construction, or otherwise increasing the cost of new home construction incorporating natural gas.
SENTENCE: Certain jurisdictions in Oregon and Washington are considering similar measures.

### s0367
Context (previous sentence): In Oregon, NW Natural has a conservation tariff which is designed to recover lost utility margin due to declines in residential and small commercial customers’ consumption.
SENTENCE: However, NW Natural does not have a conservation tariff in Washington that provides it this margin protection on sales to customers in that state.

### s0368
Context (previous sentence): These alternative measures may not be successful and may not permit us to meet our scheduled debt service obligations.
SENTENCE: If our operating results and available cash are insufficient to meet our debt service obligations, we could face substantial liquidity problems and might 24 be required to dispose of material assets or operations to meet our debt service and other obligations.

### s0369
Context (previous sentence): We may incur increased costs, including increased supply chain costs, and experience delays or disruptions in production schedules, product deliveries or payments in connection with international manufacturing and sales that could cause loss of revenues and earnings.
SENTENCE: Among other things, there are additional logistical requirements associated with international sales, which increase the amount of time between the completion of production and our ability to recognize related revenue.

### s0370
Context (previous sentence): Further, Apple implemented certain changes, including introducing an AppTrackingTransparency framework that limits the ability of mobile applications to request an iOS device’s advertising identifier and affects our ability to track user actions off our platform and connect their interactions with on-platform advertising.
SENTENCE: In addition, third parties, such as Apple, Microsoft or Google, have implemented and may continue to implement changes and restrictions in browser or device functionality including by limiting the use of cookies, or that limit our ability to communicate with or understand the identity of our users.

### s0371
Context (previous sentence): Past terrorism attacks in the U.S. and in other locations worldwide and the potential for future attacks have caused commercial insurance for such threats to become extremely difficult to obtain.
SENTENCE: In the event that we are found liable following an act of terrorism, the insurance we currently have in place would not fully cover the claims for damages.

### s0372
Context (previous sentence): It and other such systems could have a competitive advantage in comparison with other international payments networks .
SENTENCE: In general, national laws that protect domestic providers or processing may increase our costs; decrease our payments volumes and impact the revenue we generate in those countries; decrease the number of Visa products issued or processed; impede us from utilizing our global processing capabilities and controlling the quality of the services supporting our brands; restrict our activities; limit our growth and the ability to introduce new products, services and innovations; force us to leave countries or prevent us from entering new markets; and create new competitors, all of which could harm our business.

### s0373
Context (previous sentence): If we have to resort to legal proceedings to enforce our rights, the proceedings could be burdensome, protracted, distracting to management and expensive and could involve a high degree of risk and be unsuccessful.
SENTENCE: Although we believe that we are not infringing on the intellectual property rights of others, claims may nonetheless be successfully asserted against us in the future.

### s0374
Context (previous sentence): While some of these costs are likely to be recovered in the form of higher rates, there can be no assurance that the Regulators will approve a rate increase to recover all or part of such costs and, as a result, our operating results and business may be adversely affected.
SENTENCE: Further, despite these tightened security measures, we may not be in a position to control the outcome of terrorist events should they occur.

### s0375
Context (previous sentence): Specifically, from time to time, certain of our independent foreign subsidiaries sell products to companies and entities located in, or controlled by the governments of, certain countries that are or have previously been subject to sanctions and embargoes imposed by the U.S. government, the United Nations or other 23 countries where we maintain operations.
SENTENCE: With the exception of the U.S. sanctions against Cuba and Iran, the applicable sanctions and embargoes generally do not prohibit our foreign subsidiaries from selling non-U.S.-origin products and services to countries that are or have previously been subject to sanctions and embargoes.

### s0376
Context (previous sentence): Our total contributions to the plan were $ 3.9 million, $ 3.3 million and $ 2.9 million for the years ended December 31, 2020, 2019, and 2018, respectively.
SENTENCE: NOTE P – Related Party Transactions SPS Commerce Foundation (the “Foundation”) is a Minnesota non-profit organization exempt from federal taxation under Section 501(c)(3) of the Internal Revenue Code.

### s0377
Context (previous sentence): The retail industry is highly competitive and the marketplace is highly fragmented, as many different retailers compete for market share by utilizing a variety of store and online formats and merchandising strategies.
SENTENCE: We expect competition to increase in the future.

### s0378
Context (previous sentence): Favorable pricing impacted sales by 0.2%.
SENTENCE: Favorable volume and product mix increased sales by 1.7% driven by higher sales to foodservice customers in China.

### s0379
Context (previous sentence): Geopolitical events beyond our control may impact or increase our cost of doing business or disrupt our operations.
SENTENCE: Events such Geopolitical events beyond our control may impact or increase our cost of doing business or disrupt our operations.

### s0380
Context (previous sentence): These proposals include changes to the existing framework to calculate income tax, as well as proposals to change or impose new types of non-income taxes, including taxes based on a percentage of revenue.
SENTENCE: For example, several countries in the European Union have proposed or enacted taxes applicable to digital services, which includes business activities on social media platforms and online marketplaces, and would likely apply to our business.

### s0381
Context (previous sentence): The occurrence of an earthquake, fire or any other catastrophic event could disrupt our operations or the operations of third parties who provide vital support functions to us, which could have a material adverse effect on our business and financial condition.
SENTENCE: We and some of the third-party service providers on which we depend for various support functions are vulnerable to damage from catastrophic events, such as power loss, natural disasters, extreme weather, terrorism, pandemics and similar unforeseen events beyond our control.

### s0382
Context (previous sentence): Our standard terms and conditions permit payment within a specified number of days following the receipt of our solution.
SENTENCE: Volatile economic conditions, including those related to the COVID-19 pandemic and its variants, or the war in Ukraine and the global response, could result in our customers and resellers facing liquidity concerns leading to them not being able to satisfy their payment obligations to us, which would have a material adverse effect on our financial condition, operating results and cash flows.

### s0383
Context (previous sentence): If our policies, procedures and systems are deemed deficient, we would be subject to liability, including fines and regulatory actions, which may include restrictions on our ability to pay dividends and the necessity to obtain regulatory approvals to proceed with certain aspects of our business plan, including our acquisition plans.
SENTENCE: Failure to maintain and implement adequate programs to combat money laundering and terrorist financing could also have serious reputational consequences for us.

### s0384
Context (previous sentence): Any data security breaches, cyber-attacks, malicious intrusions or significant disruptions could result in actions by regulatory bodies and/or civil litigation, any of which could materially and adversely affect our business, results of operations, financial condition, cash flows, reputation or competitive position.
SENTENCE: Our worldwide operations mean that we are subject to laws and regulations, including data protection and cybersecurity laws and regulations, in many jurisdictions.

### s0385
Context (previous sentence): The chip manufacturing industry is highly concentrated, and we derive most of our revenue from a limited number of customers.
SENTENCE: In 2019, 73.8% of our revenue was derived from three customers: Yangtze Memory Technologies Co., Ltd., a leading PRC memory chip company, together with one of its subsidiaries, accounted for 27.5% of our revenue; Shanghai Huali Microelectronics Corporation, and the operations of The Huahong Group in Wuxi, China, a leading PRC foundry, accounted for 26.5% of our revenue; and SK Hynix Inc., a leading Korean memory chip company, accounted for 19.8% of our revenue.

### s0386
Context (previous sentence): This exposes us to risks of disruption and cost increases in our established patterns for sourcing our merchandise and creates increased uncertainties in planning our sourcing strategies and forecasting our margins.
SENTENCE: Changes in U.S. tariffs, quotas, trade relationships, or tax provisions that reduce the supply or increase the relative cost of goods produced in other countries could increase our cost of goods and/or increase our effective tax rate.

### s0387
Context (previous sentence): On March 1, 2018, the United States announced a plan to indefinitely impose a 25 percent tariff on certain imported steel products and a 10 percent tariff on certain imported aluminum products under Section 232 of the Trade Expansion Act of 1962 (the “Section 232”) tariffs.
SENTENCE: Application of the tariffs commenced March 23, 2018, with temporary or long-term exemptions for a number of countries and subject to a product exemption process.

### s0388
Context (previous sentence): We could be subject to lawsuits, claims, and criminal and civil enforcement actions.
SENTENCE: Additionally, we may not be able to maintain the level or types of insurance we desire, and the insurance coverage we do obtain may contain large deductibles or fail to cover certain hazards or cover all potential losses.

### s0389
Context (previous sentence): Furthermore, while we do not knowingly source any products or product inputs from the XUAR, we have no known involvement with any entity list company and we prohibit our suppliers from using forced labor, our supply chain is complex, and we may not have the ability to completely map and monitor it.
SENTENCE: We could be subject to penalties, fines or sanctions if any of the producers from which we purchase goods is found or suspected to have dealings, directly or indirectly, with the XUAR or entity list companies, and any actions taken by customs officials to block the import of products suspected of being manufactured with forced labor, whether or not founded, could adversely impact our operations and financial results.

### s0390
Context (previous sentence): These items could have a negative impact on our cash flows and a negative effect on the net carrying value of the mortgage servicing right (“MSR”) on our balance sheet and could result in a charge to our earnings.
SENTENCE: Because of the foregoing, a rise in delinquencies could have a material adverse effect on us.

### s0391
Context (previous sentence): Current or future global market uncertainties or downturns and associated macroeconomic conditions, such as growing inflation, rising interest rates, recessionary fears, changes in foreign currency exchange rates, supply chain disruptions, the impact of global instability in many parts of the world and public health crises, may disrupt the operations of our clients and partners and cause advertise
SENTENCE: As we explore new countries to expand our business, economic downturns or unstable market conditions in any of those countries could also result in our investments not yielding the returns we anticipate.

### s0392
Context (previous sentence): We face security risks, including denial of service attacks, hacking, social engineering attacks targeting our colleagues and customers, malware intrusion or data corruption attempts, and identity theft that could result in the disclosure of confidential information, adversely affect our business or reputation, and create significant legal and financial exposure.
SENTENCE: Our computer systems and network infrastructure and those of third parties, on which we are highly dependent, are subject to security risks and could be susceptible to cyber-attacks, such as denial of service attacks, hacking, terrorist activities or identity theft.

### s0393
Context (previous sentence): The increase for the year ended December 31, 2023 was primarily due to the increase in acquisition and integration and compensation expenses, partially offset by lower charges related to facilities exit activities in the current year.
SENTENCE: Operating Income and Operating Margin Consolidated operating income for the year ended December 31, 2023 was $1,716.4 million, compared to $640.2 million for the prior year.

### s0394
Context (previous sentence): In addition, our business could be negatively affected if our home sales, homes delivered or backlog-to-homes delivered conversion rate falls; if often-volatile building materials prices or subcontractor rates increase, which has been the trend over the past few years; or if our community openings are delayed due to, among other things, prolonged development, our strategic adjustments, or protract
SENTENCE: The federal government has imposed new or increased import tariffs, and other countries have implemented retaliatory measures, raising the cost and reducing the supply of several home construction items.

### s0395
Context (previous sentence): The tariffs on imports, most notably imports from China, have impacted the cost of steel, a key commodity that we consume in producing products.
SENTENCE: Given the significance of steel costs to our direct materials costs, we closely monitor trade tensions between the U.S. and China.

### s0396
Context (previous sentence): Our international operations are subject to additional risks, including fluctuations in currency values, foreign currency exchange controls, discriminatory fiscal policies, compliance with U.S. and foreign laws, enforcement of remedies in foreign jurisdictions and other economic or political uncertainties.
SENTENCE: Several countries within the European Union continue to experience sovereign debt and credit issues, which causes more volatility in the economic environment throughout the European Union and the U.K.

### s0397
Context (previous sentence): The APSC approved an initial offering of 100 MW of solar capacity to be made available under this tariff.
SENTENCE: In June 2023 the APSC approved Entergy Arkansas’s Go ZERO tariff, which provides participating industrial and commercial customers the opportunity to chose from a number of clean energy options to help them achieve their sustainability goals.

### s0398
Context (previous sentence): Loan demand could also be negatively impacted.
SENTENCE: The imposition of tariffs or immigration reform could directly or indirectly adversely impact our clients businesses, and in turn demand for our loan and deposit products or borrowers' ability to repay their loans.

### s0399
Context (previous sentence): Increases in the market prices of manufacturing materials may negatively affect our profitability.
SENTENCE: The costs of certain manufacturing materials used in our operations are sensitive to shifts in commodity market prices, including the impact of the U.S. and retaliatory tariffs.

### s0400
Context (previous sentence): The state of the ongoing conflict remains highly uncertain and could worsen or expand which can further impact economic conditions and activity in Israel, the region and the broader global economy, including revenues from customers located in the region.
SENTENCE: Our operations could be disrupted by, for example, the prolonged absence of a large number of employees due to Israel military service call-ups.