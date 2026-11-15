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

### s0401
Context (previous sentence): These blends are based on MPC’s refining capacity by region in each period. 2024 Compared to 2023 Refining & Marketing segment revenues decreased $10.21 billion primarily due to decreased average refined product sales prices of $0.24 per gallon, partially offset by increased refined product sales volumes of 75 mbpd.
SENTENCE: Refinery crude oil capacity utilization was 92 percent during 2024 and net refinery throughput increased 19 mbpd in 2024.

### s0402
Context (previous sentence): For example, as described in Part I, Item 1. "Business," in August 2020, we announced a collaboration agreement with Roche to develop, manufacture, and distribute REGEN-COV.
SENTENCE: We cannot be certain that the technology transfer process required to allow Roche to manufacture REGEN-COV will be completed in the expected time frame or at all nor can we be certain that this collaboration will result in the anticipated increase in the current manufacturing and distribution capacity for REGEN-COV or that any increased manufacturing and distribution capacity will be sufficient.

### s0403
Context (previous sentence): Any liability resulting from such claims could have a material adverse effect on our future business, financial condition, results of operations and cash flows.
SENTENCE: If foreign investment in us or MPLX exceeds certain levels, we could be prohibited from operating vessels engaged in U.S. coastwise trade, which could adversely affect our business, financial condition, results of operations and cash flows.

### s0404
Context (previous sentence): Negative or uncertain economic conditions that cause John Deere’s customers to lack confidence in the general economic outlook can significantly reduce their likelihood of purchasing John Deere’s equipment.
SENTENCE: The COVID pandemic, geopolitical instability, including the conflict between Russia and Ukraine, and other global events have significantly increased economic and demand uncertainty.

### s0405
Context (previous sentence): Clinical trials of potential products often reveal that it is not practical or feasible to continue development efforts.
SENTENCE: Regulatory authorities may require us or our partners to conduct additional clinical testing, in which case we would have to expend additional time and resources.

### s0406
Context (previous sentence): The volatility and uncertainty caused by the pandemic have adversely affected our stock price and may continue to do so.
SENTENCE: The impact of this pandemic on the U.S., Indian, Chinese and world economies is uncertain and, unless the pandemic is effectively contained, these adverse impacts could worsen, impacting all segments of the global economy, and result in a significant recession or worse.

### s0407
Context (previous sentence): Adverse economic or real estate trends in these states or the surrounding regions or any decrease in demand for retail space resulting from the local regulatory environment, business climate, or fiscal problems in these states could have a material adverse effect on us and limit our ability to meet our financial obligations. 13 Table of Contents Uninsured losses or losses in excess of insurance co
SENTENCE: We do not carry insurance for generally uninsurable losses such as loss from riots, war or acts of God and, in some cases, floods.

### s0408
Context (previous sentence): Our leases generally require tenants to carry comprehensive liability and extended coverage insurance on our properties.
SENTENCE: However, there are certain losses, including losses from environmental liabilities, terrorist acts or catastrophic acts of nature, that are not generally insured against or that are not generally fully insured against because it is not deemed economically feasible or prudent to do so.

### s0409
Context (previous sentence): Sustained uncertainty about, or worsening of, current global economic conditions and further escalation of trade tensions between the U.S. and its trading partners could result in a global economic slowdown and long-term changes to global trade.
SENTENCE: Such events may also (i) cause our customers and consumers to reduce, delay or forgo technology spending, (ii) result in customers sourcing products from other suppliers not subject to such restrictions or tariffs, (iii) lead to the insolvency or consolidation of key suppliers and customers and (iv) intensify pricing pressures.

### s0410
Context (previous sentence): Entities listed on the Unverified List are ineligible to receive items subject to the EAR by means of a license exception if a U.S. export license is required.
SENTENCE: In December 2022, YMTC was moved from the Unverified List to the Entity List.

### s0411
Context (previous sentence): Unfavorable volume and product mix decreased segment sales by 4.2% as compared to 2019, while pricing actions, taken in response to increased costs, during the period increased sales by 1.8%.
SENTENCE: The unfavorable impact of foreign currency rates decreased flavor solutions segment sales by 1.1% as compared to 2019 and is excluded from our measure of sales decline of 2.4% on a constant currency basis.

### s0412
Context (previous sentence): Our future results could be adversely affected by changes in interpretations of existing laws and regulations, or changes in laws and regulations, including, among others, changes in accounting standards, taxation requirements, competition laws, trade laws, import and export restrictions, privacy laws and environmental laws in the U.S. and other countries.
SENTENCE: The U.S. government has made statements and taken certain actions that have led to, and may lead to further, changes to U.S. and international export and import controls or trade policies, including tariffs affecting certain products exported by a number of U.S. trading partners, including China.

### s0413
Context (previous sentence): One or more of these third-party vendors may experience financial distress, technology challenges, cybersecurity incidents, staffing shortages, liquidity challenges, file for bankruptcy protection, go out of business, suffer disruptions in their business or experience significant increases in the cost of their goods or services sold due to factors beyond their control, including tariffs.
SENTENCE: The use of third-party vendors represents an inherent risk to our company that could have a material adverse effect on our business, sales and results of operations.

### s0414
Context (previous sentence): Our foreign operations are subject to economic, social, and political risks inherent in maintaining operations abroad such as economic and political destabilization, land use risks, international conflicts, pandemics and other health-related crises, restrictive actions by foreign governments, and adverse foreign tax laws.
SENTENCE: In addition to economic and political risk, a risk associated with our European manufacturing operations is the higher relative expense and length of time required to adjust manufacturing employment capacity.

### s0415
Context (previous sentence): The Company could be adversely affected by any changes in the services provided or to the costs of such services provided by SSAT.
SENTENCE: The Company is subject to risks associated with conducting business in foreign shipping markets.

### s0416
Context (previous sentence): The cost of coverage may become so high that we may need to reduce our policy limits or agree to certain exclusions from our coverage.
SENTENCE: Among other factors, it is possible that homeland security concerns, other catastrophic events or any change in government legislation governing insurance coverage for acts of terrorism could materially adversely affect available insurance coverage and result in increased premiums on available coverage (which may cause us to elect to reduce our policy limits) and additional exclusions from coverage.

### s0417
Context (previous sentence): Changes in, and responses to, U.S. trade policy could reduce the competitiveness of our products and cause our sales to decline, which could materially and adversely impact our business, financial condition and results of operations. 33 The U.S. or foreign governments may take administrative, legislative or regulatory action that could materially interfere with our ability to sell products in cert
SENTENCE: For example, the United States and China have imposed a number of tariffs and other restrictions on items imported or exported between the United States and China, and have proposed to impose a number of additional tariffs.

### s0418
Context (previous sentence): Accordingly, we are subject to risks associated with potential disruption caused by changes in political, economic and social environments, including war, civil and political unrest, illnesses declared as a public health emergency (including viral pandemics such as COVID-19), terrorism, expropriation, local labor conditions, changes in laws, regulations and policies of foreign governments and trad
SENTENCE: We could be adversely affected by higher manufacturing costs and international trade regulations, including, tariffs (including recent U.S. tariffs imposed or threatened to be imposed on China, Canada and Mexico and other countries and any retaliatory actions taken by such countries), duties and antidumping penalties.

### s0419
Context (previous sentence): We have experienced, and may continue to experience, rapid growth in our headcount and operations, which has placed, and may continue to place, significant demands on our management, operational and financial resources.
SENTENCE: We have also experienced significant growth in the number of clients and transactions and the amount of client and employee data that our infrastructure supports.

### s0420
Context (previous sentence): If any such risks, or any other risks that we do not currently consider to be material, or which are not known to us, materialize, our business, financial condition and operating results could be materially adversely affected.
SENTENCE: Business and Industry Risks If operators of, or algorithms installed in, our security and inspection systems fail to detect weapons, explosives or other devices or materials that are used to commit a terrorist act, we could be exposed to product and professional liability and related claims for which we may not have adequate insurance coverage.

### s0421
Context (previous sentence): We are also subject to anti-bribery and anti-corruption laws, such as the FCPA and the U.K.
SENTENCE: Anti-Bribery Act, trade sanctions, export control regulations and restrictions and anti-money laundering laws.

### s0422
Context (previous sentence): Moreover, in the event any of these suppliers breach their contracts with us, our legal remedies associated with such a breach may be insufficient to compensate us for any damages it may suffer.
SENTENCE: Financial and Market Risks The impact of changes in customs duties and trade policies in the United States and corresponding actions by other countries in which the Company does business could adversely affect our financial performance.

### s0423
Context (previous sentence): As a result of the complexity and rapid development of AI, it is also the subject of evolving review by various U.S. governmental and regulatory agencies, and other foreign jurisdictions are applying, or are considering applying, their platform moderation, intellectual property, cybersecurity, and data protection laws to AI and/or are considering general legal frameworks on AI.
SENTENCE: For example, the Artificial Intelligence Act (“EU AI Act”) recently came into effect in August 2024 and gives companies one to three years to comply with its various requirements which are principally focused on creating transparency with respect to generative AI systems and AI-generated content.

### s0424
Context (previous sentence): The EAR require licenses for, and sometimes prohibit, the export of certain products.
SENTENCE: The CCL sets forth the types of goods and services controlled by the EAR, including civilian science, technology, and engineering dual use items.

### s0425
Context (previous sentence): In addition, auditor judgment was required to evaluate the sufficiency of the audit evidence obtained.
SENTENCE: This assessment of the ALL encompassed the methodologies, inputs, and assumptions used to estimate the general allowance including use of the historical loss experience by loan category, the determination of the loan segmentation, look-back period, loss emergence periods, the loan risk grades, and the environmental factors.

### s0426
Context (previous sentence): For example, Insulet Corporation is our single-source of the on-body injector for our Neulasta ® Onpro ® kit.
SENTENCE: Also, certain of the raw materials required in the commercial and clinical manufacturing of our products are sourced from other countries and/or derived from biological sources, including mammalian tissues, bovine serum and human serum albumin.

### s0427
Context (previous sentence): As a result of adopting ASC 842, we recognized $ 567 million for operating lease liabilities and right-of-use assets and reclassified an additional $ 66 million of other balances to right-of-use assets to conform to the new presentation requirements of ASC 842. 55 | 2020 10-K 55 | 2020 10-K Recently Issued Accounting Standards In August 2020, the FASB issued ASU 2020-06 – Debt - Debt with Conversi
SENTENCE: This ASU requires a convertible debt instrument to be accounted for as a single liability measured at its amortized cost, as long as no other features require bifurcation and recognition as derivatives.

### s0428
Context (previous sentence): We anticipate capital expenditures for fiscal 2024 to be between $175 million and $225 million.
SENTENCE: Transition Tax Payments The Tax Cuts and Jobs Act of 2017 imposed a mandatory, one-time transition tax on accumulated foreign earnings and profits that had not previously been subject to U.S. income tax.

### s0429
Context (previous sentence): This includes the EU’s General Data Protection Regulation, the California Privacy Rights Act, the Virginia Consumer Data Protection Act, and other similar laws that have been or are expected to be enacted by other jurisdictions.
SENTENCE: In addition, China and certain other jurisdictions have enacted more stringent data localization requirements.

### s0430
Context (previous sentence): Government authorities in affected regions have in the past taken actions, sometimes 7 drastic and including mandatory capacity restrictions, reduced operating hours, and closure of retail operations, in an effort to slow down the spread of the disease.
SENTENCE: We may still face required store closures and distribution center closures, nationally, regionally, or in specific locations.

### s0431
Context (previous sentence): The Company is an international company, and the risks associated with operating in foreign countries may have a negative impact on the Company's liquidity and net income.
SENTENCE: The Company's international operations generated approximately 63 % , 62% and 64% of its consolidated net sales in the years ended 2021, 2020 and 2019.

### s0432
Context (previous sentence): While we are working closely with the FAA and other aviation industry participants to develop a long-term strategy that permits the full implementation of the 5G spectrum without disruption to safe aviation operations, any new restrictions imposed to mitigate interference risks would require us to adjust our operating procedures and could impact our ability to operate certain aircraft or to serve 
SENTENCE: Our technologies and automated systems are not completely protected against events that are beyond our control, including natural disasters, power failures, terrorist attacks, cyber-attacks, data theft, equipment and software failures, computer viruses or telecommunications failures.

### s0433
Context (previous sentence): In addition, in November 2017, the Chinese government adopted new rules to control the cross-border transportation of cash and bearer negotiable instruments, specifically to reduce the international transfer of cash in connection with activities that are illegal in China, including gambling.
SENTENCE: The Chinese government has recently taken steps to prohibit the transfer of cash for the payment of gaming debts.

### s0434
Context (previous sentence): We do not have any investigational products approved for sale in any jurisdiction, including international markets, and we do not have experience in obtaining regulatory approval in international markets.
SENTENCE: If we or our collaborators fail to comply with regulatory requirements in international markets or fail to obtain and maintain required approvals, our ability to realize the full market potential of our products will be harmed.

### s0435
Context (previous sentence): The U.S. federal government, certain U.S. states and certain other countries and regions have adopted or are considering legislation or regulation imposing overall caps or taxes on greenhouse gas emissions from certain sectors or facility categories.
SENTENCE: Such new laws or regulations, or stricter enforcement of existing laws and regulations, could increase the costs of operating our businesses, reduce the demand for our products and services and impact the prices we charge our customers, any or all of which could adversely affect our results of operations.

### s0436
Context (previous sentence): ACM may not be able to import, or may face substantial restrictions in importing, certain parts from the United States or parts subject to U.S. export controls from outside the United States to support tool shipments to such facilities, or to be embedded into tools defined by affected ECCNs.
SENTENCE: We believe that as a result of the October 2022 and October 2023 restrictions, several ACM Shanghai customers have significantly reduced production and related capital spending at facilities meeting the restricted advanced node capabilities.

### s0437
Context (previous sentence): Many member nations in the European Union have been addressing the issues with controversial austerity measures.
SENTENCE: In addition, the potential consequences of the “Brexit” process in the United Kingdom have led to significant uncertainty in the region.

### s0438
Context (previous sentence): We are subject to governmental export and import controls that could subject us to liability or impair our ability to compete in international markets.
SENTENCE: The U.S. and various foreign governments have imposed controls, export license requirements and restrictions on the import or export of certain products, technologies and software.

### s0439
Context (previous sentence): The use of open source software can also carry security risks arising from unknown vulnerabilities that can be exploited by malware in unanticipated ways, which can lead to disruption and / or harm to operations and protected data. 29 Table of Contents Catastrophic events or other interruptions or failures of our information technology systems could hurt our ability to effectively provide our prod
SENTENCE: Our third-party service providers, including cloud service providers could be disrupted by fire, flood, power loss, telecommunications failure, earthquakes, pandemics, acts of war or terrorism, acts of God, malware (including viruses and malicious software), physical or electronic break-ins and other similar events or disruptions.

### s0440
Context (previous sentence): The occurrence of any of these events could impede our ability to effectively compete against competitors with similar technologies, any of which could materially adversely affect our business, financial condition and results of operations.
SENTENCE: Our use of “open source” software and materials could subject our proprietary software to general release, adversely affect our ability to sell our products and services and subject us to possible litigation.

### s0441
Context (previous sentence): The outbreak of COVID- 19 has harmed the Chinese economy, shut down business operations in China and disrupted manufacturing, travel, drayage of containers, and transportation of goods within and from China.
SENTENCE: A reduction or delay in container volume from China resulting from decreased manufacturing activity, lower transportation demand or service disruptions from restrictions related to COVID- 19 could adversely affect volumes or rates in our CLX service, Matson Logistics’ business related to China, and/or SSAT lift volume at its U.S.

### s0442
Context (previous sentence): Legislative and regulatory changes, including changes to agency practice, in the future may negatively impact our ability to realize value from certain existing and future investments, including by limiting exit opportunities or causing us to favor buyers that we believe are less likely to require CFIUS review, even in circumstances where other buyers may offer better terms or more consideration. 
SENTENCE: Our products are subject to import and export controls in jurisdictions in which we distribute or sell our products.

### s0443
Context (previous sentence): Operations outside the U.S. expose us to risks including fluctuations in currency values, trade restrictions, tariff and trade regulations, U.S. export controls, U.S. and non‑U.S. tax laws, shipping delays and economic and political instability.
SENTENCE: For example, violations of U.S. export controls, including those administered by the U.S.

### s0444
Context (previous sentence): Our net cash flows used in financing activities were $104.5 million during 2018 .
SENTENCE: We repurchased $113.3 million in stock and paid $33.4 million in dividends, offset by borrowings of $40.0 million under our Facility.

### s0445
Context (previous sentence): Bribery Act and local laws which also prohibit corrupt payments to governmental officials or third parties, data privacy requirements, labor relations laws, tax laws, anti-trust or competition laws, U.S., E.U. or U.N. sanctioned country or sanctioned persons mandates, and consumer protection laws.
SENTENCE: Violations of these laws and regulations could result in fines and/or criminal sanctions against us, our officers or our employees and/or prohibitions on the conduct of our business.

### s0446
Context (previous sentence): The amount of interest expense capitalized as construction in progress was $ 1.0 million, $ 1.6 million and $ 1.7 million during 2020, 2019 and 2018, respectively.
SENTENCE: Property, plant and equipment, net, is recorded at cost and includes construction in progress (see Note 2).

### s0447
Context (previous sentence): We are also subject to a variety of federal, state and foreign employment and labor laws and regulations, including the Americans with Disabilities Act, the Federal Fair Labor Standards Act and other laws and regulations related to working conditions, wage-hour pay, overtime pay, employee benefits, anti-discrimination and termination of employment.
SENTENCE: Noncompliance with applicable regulations or requirements could subject us to investigations, sanctions, mandatory product recalls, enforcement actions, fines, damages, civil and criminal penalties or injunctions.

### s0448
Context (previous sentence): An adverse outcome in such litigation or proceedings may expose us to loss of our proprietary position.
SENTENCE: We may not be able to protect our intellectual property rights throughout the world, including mainland China, which could materially, negatively affect our business.

### s0449
Context (previous sentence): In addition, countries may impose other restrictions on the importation of products.
SENTENCE: For example, in 2018 China imposed a ban on the importation of various types of solid waste allegedly in an effort to reduce environmental pollution.

### s0450
Context (previous sentence): In addition, compliance with legal, regulatory or tax requirements in multiple jurisdictions places demands on our time and resources, and we may nonetheless experience unforeseen and potentially adverse legal, regulatory or tax consequences.
SENTENCE: In some markets such as China, legal and other regulatory requirements may prohibit or limit participation by foreign businesses, such as by making foreign ownership or management of internet or travel-related businesses illegal or difficult, or may make direct participation in those markets uneconomic, which could make our entry into and expansion in those markets difficult or impossible, require that we work with a local partner or result in higher operating costs.