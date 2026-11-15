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

### s0151
Context (previous sentence): Department of the Treasury’s Office of Foreign Assets Control (OFAC) and the U.S.
SENTENCE: State Department administer certain laws and regulations that impose penalties upon U.S. persons and entities and, in some instances, non-U.S. entities, for conducting activities or transacting business with certain countries, governments, entities, or individuals subject to Economic Sanctions Laws.

### s0152
Context (previous sentence): Since the terms of the United Kingdom's exit from the European Union and/or the European Economic Area are uncertain, we are unable to predict the effect Brexit will have on our business and results of operations.
SENTENCE: The United Kingdom's decision to leave the European Union could result in other member countries also determining to leave, which could lead to added economic and political uncertainty and devaluation or eventual abandonment of the Euro common currency, any of which could have a negative impact on travel and therefore our business and results of operations.

### s0153
Context (previous sentence): In addition, tariffs on components that we import from China or other nations that have imposed, or may in the future impose, tariffs will adversely affect our profitability unless we are able to exclude such components from the tariffs or we raise prices for our products, which may result in our products becoming less attractive relative to products offered by our competitors.
SENTENCE: Future actions or escalations by either the United States or China that affect trade relations may also impact our business, or that of our suppliers or customers, and we cannot provide any assurances as to whether such actions will occur or the form that they may take.

### s0154
Context (previous sentence): If we do not continuously strengthen our capabilities in marketing and innovation to maintain consumer interest and 13 brand loyalty and market share while we selectively expand into other profitable categories in the nonalcoholic and alcoholic beverage segments of the commercial beverage industry, our business could be negatively affected.
SENTENCE: If we are unable to renew collective bargaining agreements on satisfactory terms, or we or our bottling partners experience strikes, work stoppages or labor unrest, our business could suffer.

### s0155
Context (previous sentence): Other factors include levels of unemployment, the size and timing of federal stimulus programs, salaries and wage rates, prevailing economic conditions, increasing inflation, rising interest rates, recession and fears of recession, housing costs, energy and fuel costs, income tax rates and the timing of tax refunds, consumer perceptions of personal well-being and security, availability of consumer
SENTENCE: The COVID-19 pandemic, the Russia-Ukraine conflict, and other potential, adverse developments in any of these areas, could reduce demand for our merchandise, increase our cost of goods, freight cost, and payroll costs, decrease our inventory turnover, cause greater markdowns, and negatively affect our sales and margins.

### s0156
Context (previous sentence): Our policies mandate strict compliance with U.S. and non-U.S. trade laws applicable to our products.
SENTENCE: However, even when we are in strict compliance with law and our policies, we may suffer reputational damage if certain of our products are sold through various intermediaries to sanctioned entities or to entities operating in sanctioned countries.

### s0157
Context (previous sentence): For example, Matson is a common carrier, whose tariffs, rates, rules and practices in dealing with its customers are governed by extensive and complex foreign, federal, state and local regulations, which may be the subject of disputes or administrative or judicial proceedings.
SENTENCE: If these disputes develop into proceedings, these proceedings, individually or collectively, could involve or result in significant expenditures or losses by the Company, or result in significant changes to Matson’s tariffs, rates, rules and practices in dealing with its customers, all of which could have an adverse effect on the Company’s future operating results, including profitability, cash flows and financial condition. 19 19 Table of Contents Non-compliance with, or changes to, federal, state or local law or regulations, including passage of climate change legislation or regulation, may adversely affect the Company’s business.

### s0158
Context (previous sentence): The costs of defending any such challenge and any adverse outcome arising from such a challenge could damage our reputation or could have a material adverse effect on our business, financial condition, or results of operations.
SENTENCE: We are subject to the USA PATRIOT Act, OFAC guidelines and requirements, the BSA, and related FinCEN and FFIEC Guidelines and regulations and any failure to comply with them could result in material implications that could harm our business.

### s0159
Context (previous sentence): As these changes are adopted by countries, tax uncertainty could increase and may adversely affect our provision for income taxes.
SENTENCE: WE OPERATE GLOBALLY AND ARE SUBJECT TO SIGNIFICANT RISKS IN MANY JURISDICTIONS Global Regulation and Economic and Political Conditions, as well as Potential Changes in Regulations, Legislation and Government Policy, May Negatively Affect Our Business.

### s0160
Context (previous sentence): See Item 1A of this Annual Report on Form 10-K for further details.
SENTENCE: In addition, our revenues and results of operations have been affected by various fluctuations in macroeconomic conditions and regulatory and policy changes, both on a global level and in particular markets, which include inflation and slowing economic growth and contractions, a rising interest rate environment, supply chain interruptions, tariff policy changes, volatility in capital markets and the availability of credit, tax rates and the rate of exchange between the United States dollar and foreign currencies.

### s0161
Context (previous sentence): Risks Relating to Government Regulations Changes in U.S. and international laws, accounting standards, export and import controls and trade policies or the enforcement of, or attempt to enforce, such laws, standards, controls and policies may adversely impact our business and operating results.
SENTENCE: Our future results could be adversely affected by changes in interpretations of existing laws and regulations, or changes in laws and regulations, including, among others, changes in accounting standards, taxation requirements, competition laws, trade laws, import and export restrictions, privacy laws and environmental laws in the U.S. and other countries.

### s0162
Context (previous sentence): In particular, we currently host our online betting and gaming offerings and support our operations using Amazon Web Services (“AWS”) and other third-party technology, platforms and services.
SENTENCE: Our third-party providers may experience service interruptions, delays, outages or damage, including due to capacity constraints, an event causing an unusually high volume of Internet use (such as a pandemic or public health emergency), infrastructure changes or upgrades (such as 5G or 6G services), human or software errors, website hosting disruptions, natural disasters, cybersecurity attacks, terrorist attacks, power outages and similar events or acts of misconduct.

### s0163
Context (previous sentence): Risks related to our data, intellectual property and listings • If we are not able to obtain and maintain accurate, comprehensive, or reliable data, we could experience reduced demand for our services. • If we are not able to obtain and maintain accurate, comprehensive, or reliable data, we could experience reduced demand for our services. • If we are unable to enforce or defend our ownership and 
SENTENCE: Risks related to our international operations • We are expanding our operations outside of the United States, which may subject us to increased business, regulatory, and economic risks that could harm our business. • We are exposed to additional business risks from our international operations, including volatility in foreign currency exchange rates.

### s0164
Context (previous sentence): In addition, we own four hotels located in seismically active areas of California and five hotels located in areas that have an increased potential to experience hurricanes (Florida, Hawaii, and Louisiana).
SENTENCE: We have acquired and intend to maintain comprehensive insurance on each of our hotels, including liability, terrorism, fire, and extended coverage, of the type and amount that we believe are customarily obtained for or by hotel owners.

### s0165
Context (previous sentence): We operate or are registered in locations throughout the U.S. and Canada and, as a result, we are subject to the tax laws and regulations of U.S. federal, state and local and Canadian governments.
SENTENCE: We have investments in unconsolidated affiliates that operate in the U.S. and international locations.

### s0166
Context (previous sentence): Trends, Risks and Uncertainties Related to Our Business Changes in tariffs or other government trade policies may materially adversely affect our business and results of operations, including by reducing demand for our products.
SENTENCE: The imposition of tariffs and trade restrictions as a result of international trade disputes or changes in trade policies may adversely affect our sales and profitability.

### s0167
Context (previous sentence): Our international operations, including U.S. exports, represent more than half of the Company’s sales.
SENTENCE: Risks related to international operations include exchange control regulations, wage and price controls, fluctuations in foreign currency exchange rates, antitrust regulations, employment regulations, foreign investment laws, import, export, and other trade restrictions and barriers (such as tariffs, sanctions, and embargoes), differing levels of protection of intellectual property, acts of industrial espionage, violations by our employees or business partners of anti-corruption or anti-money-laundering laws (despite our efforts to mitigate such risk), changes in regulations regarding transactions with state-owned enterprises, nationalization of private enterprises, acts of terrorism, acts of war, civil strife, and our ability to hire and maintain qualified staff and maintain the safety of our employees in these regions.

### s0168
Context (previous sentence): In addition, we and our manufacturers and suppliers may not be able to find a sufficient number of qualified workers due to the intensely competitive and fluid market for skilled labor in China.
SENTENCE: Furthermore, pursuant to Chinese labor laws, employers in China are subject to various requirements when signing labor contracts, paying remuneration, determining the term of employees’ probation and unilaterally terminating labor contracts.

### s0169
Context (previous sentence): While the cost and availability of most insurance is stable, there are still certain types and levels of insurance that remain difficult to obtain, such as professional liability insurance, which is expensive to obtain for the amount of coverage often requested by certain customers.
SENTENCE: As we grow our global solutions and services business, we are being asked to obtain higher amounts of professional liability insurance, which could result in higher costs to do business.

### s0170
Context (previous sentence): E&Y is a PCAOB-registered firm that is headquartered in mainland China; however, we do not believe ACM Research will appear on the “Conclusive list of issuers identified under the HFCAA” for a second consecutive time, as the determinations announced by the PCAOB on December 16, 2021 were vacated by the PCAOB on December 15, 2022.
SENTENCE: It may be difficult for overseas regulators to conduct investigations or collect evidence within mainland China.

### s0171
Context (previous sentence): Our strategic plan does not require the repatriation of foreign cash in order to fund our operations in the U.S., and it is our current intention to permanently reinvest the foreign cash and cash equivalents outside of the U.S.
SENTENCE: If we were to repatriate the foreign cash to the U.S., we may be required to accrue and pay U.S. taxes in accordance with applicable U.S. tax rules and regulations as a result of the repatriation.

### s0172
Context (previous sentence): As a result, we must comply with increasingly complex and rigorous, and sometimes conflicting laws, regulatory standards, industry standards, external and internal privacy and security policies, contracts and other obligations that govern the processing of business and personal data by us and on our behalf.
SENTENCE: For example, the European Union’s General Data Protection Regulation (the “EU GDPR”), the United Kingdom’s GDPR (the “UK GDPR”) and California’s Consumer Privacy Act of 2018, as amended (the "CCPA") impose obligations on companies regarding the handling of personal data and provide certain individual privacy rights to persons whose data is stored.

### s0173
Context (previous sentence): Severe weather, natural disasters, acts of war or terrorism and other adverse external events could have a significant impact on our ability to conduct business.
SENTENCE: These events could affect the stability of our deposit base, impair the ability of borrowers to repay outstanding loans, impair the value of collateral securing loans, cause significant property damage, result in loss of revenue and cause us to incur additional expenses.

### s0174
Context (previous sentence): Like many other multinational corporations, we are subject to tax in multiple United States and foreign tax jurisdictions and have structured our operations to reduce our effective tax rate.
SENTENCE: Our determination of our tax liability is always subject to audit and review by applicable domestic and foreign tax authorities.

### s0175
Context (previous sentence): These encryption solutions and underlying technology may be exported outside of the United States only with the required export authorizations or exceptions, including by license, a license exception, appropriate classification notification requirement, and encryption authorization.
SENTENCE: Furthermore, our activities are subject to U.S. economic sanctions laws and regulations that prohibit the shipment of certain products and services without the required export authorizations, including to countries, governments, and persons targeted by U.S. embargoes or sanctions.

### s0176
Context (previous sentence): Macroeconomic and political instability caused by global supply chain disruptions, inflation and the strength of the U.S. dollar could adversely impact our results of operations.
SENTENCE: In addition, military conflicts and their impact on economies may adversely impact our results of operations.

### s0177
Context (previous sentence): Efforts to conduct our operations in compliance with all applicable laws and regulations, including environmental rules and regulations, require programs to promote compliance, such as training employees and customers, purchasing health and safety equipment and in some cases hiring outside consultants and lawyers.
SENTENCE: Even with these programs, we and other companies in the environmental services industry are routinely faced with government enforcement proceedings, which can result in fines or other sanctions and require expenditures for remedial work on waste management facilities and contaminated sites.

### s0178
Context (previous sentence): After the five-year period, a business combination with an Interested Stockholder must be approved by two super-majority stockholder votes unless, among other conditions, our common stockholders receive a minimum price for their shares and the consideration is received in cash or in the same form as previously paid by the Interested Stockholder for shares of our common stock.
SENTENCE: The Board of Directors has exempted from these provisions under Maryland law any business combination with Samuel Zell, who is Chairman of our Board of Directors, certain holders of OP Units who received them at the time of our initial public offering and our officers who acquired common stock at the time we were formed and each and every affiliate of theirs.

### s0179
Context (previous sentence): In the event of a breach, we could incur substantial operational and financial costs related to mitigation and remediation, including preparation and delivery of notices to affected individuals.
SENTENCE: Additionally, HIPAA and its implementing regulations provide for significant civil fines, criminal penalties, and other sanctions for failure to comply with the privacy, security, and breach notification rules, including for wrongful or impermissible use or disclosure of PHI.

### s0180
Context (previous sentence): The outbreak of COVID- 19 has harmed the Chinese economy, shut down business operations in China and disrupted manufacturing, travel, drayage of containers, and transportation of goods within and from China.
SENTENCE: A reduction or delay in container volume from China resulting from decreased manufacturing activity, lower transportation demand or service disruptions from restrictions related to COVID- 19 could adversely affect volumes or rates in our CLX service, Matson Logistics’ business related to China, and/or SSAT lift volume at its U.S.

### s0181
Context (previous sentence): Adverse changes may occur in the future as a result of declining or flat global or regional economic conditions, fluctuations in currency and commodity prices, wavering confidence, capital expenditure reductions, unemployment, decline in stock markets, contraction of credit availability or other factors affecting economic conditions.
SENTENCE: For example, factors that may affect our operating results include disruption in the credit and financial markets in the United States, Europe and elsewhere, adverse effects of slowdowns in the European and Chines economies, slowdown in the Chinese economy, reductions or limited growth in consumer spending or consumer credit, global trade tariffs and other adverse economic conditions that may be specific to the Internet, e-commerce and payments industries.

### s0182
Context (previous sentence): To the extent periods of volatility are coupled with a lack of realizations from clients’ existing private markets portfolios, such clients may be left with disproportionately outsized remaining commitments, which significantly limits their ability to make new commitments.
SENTENCE: In addition, during periods of adverse economic or geopolitical conditions, our specialized funds may have difficulty accessing financial markets, which could make it more difficult or impossible for them to obtain funding for additional investments.

### s0183
Context (previous sentence): These concerns and the related harm to our reputation could materially adversely affect our financial condition and results of operations, regardless of whether such reports are accurate.
SENTENCE: We are dependent on suppliers having current regulatory approvals, and the failure of those suppliers to maintain these approvals or other challenges in replacing any of those suppliers could affect our supply of materials or affect the distribution or sale of our products.

### s0184
Context (previous sentence): Accordingly, an acquisition of more than a majority of our common stock by the Gerdin family will not result in certain shares in excess of a majority losing their voting rights and may enhance the Gerdin family's ability to exercise control over decisions affecting us.
SENTENCE: The interests of the Gerdin family may conflict with the interests of other holders of our common stock, and they may take actions affecting us with which other stockholders disagree.

### s0185
Context (previous sentence): The COVID-19 pandemic and 2008 credit crisis and related turmoil in the global financial system and ensuing recession had an impact on our business and financial position, and similar events in the future could also impact us.
SENTENCE: The re-emergence of a financial crisis or recession or reduced economic activity in the United States, China, India and other industrialized or developing countries, or disruption of key sectors of the economy such as oil and gas, may have a significant effect on our results of operations or limit our ability to raise capital through credit and equity markets.

### s0186
Context (previous sentence): In addition, Brexit may lead other European Union member countries to consider referendums regarding their European Union membership.
SENTENCE: Any of these events, along with any political, economic and regulatory changes that may occur, could cause political and economic uncertainty in Europe and internationally and harm our business and financial results.

### s0187
Context (previous sentence): If we are not able to comply with the requirements of Section 404 of the Sarbanes-Oxley Act in a timely manner, or if we are unable to maintain proper and effective internal controls, we may not be able to produce timely and accurate financial statements.
SENTENCE: If that were to happen, the market price of our stock could decline and we could be subject to sanctions or investigations by the stock exchange on which our common stock is listed, the SEC, or other regulatory authorities.

### s0188
Context (previous sentence): Individuals also have a right to compensation under GDPR for financial or non-financial losses.
SENTENCE: Additionally, Brexit took effect in January 2020, which will lead to further legislative and regulatory changes.

### s0189
Context (previous sentence): Ltd. (“Huawei”) and many of its affiliates to its Entity List (and subsequently added additional Huawei affiliates), which effectively blocks exports of U.S. products to Huawei and such affiliates.
SENTENCE: Additionally, in October 2022 and 2023, the BIS introduced restrictions related to semiconductor manufacturing, supercomputer and advanced computing items and end-uses, which restrict or prohibit the ability to sell, ship and support certain equipment and services to China.

### s0190
Context (previous sentence): The outstanding claims at December 31, 2021 also exclude approximately 19,000 inactive claims, as well as claims in Texas filed after June 11, 2003.
SENTENCE: Due to the passage of time, the Company considers it unlikely that the plaintiffs in these cases will pursue further action.

### s0191
Context (previous sentence): As part of our business, we manage, utilize and store sensitive or confidential client or employee data, including personal data.
SENTENCE: As a result, we are subject to various risks and costs associated with the collection, handling, storage and transmission of sensitive information, including those related to compliance with U.S. and foreign data collection and privacy laws and other contractual obligations, as well as those associated with the compromise of our systems collecting such information.

### s0192
Context (previous sentence): Since we operate in an industry which is inherently driven by the element of chance and the winnings of our gaming customers may exceed our winnings, we do not have full control over our gaming revenues.
SENTENCE: This may result in our having to record a loss from our gaming operations, which could have a material adverse effect on our financial condition, results of operations and cash flows. 18 Table of Contents OUR RESULTS OF OPERATIONS MAY BE ADVERSELY AFFECTED BY HIGH-END PLAYERS’ WINNINGS OR THEIR FAILURE TO REPAY FUNDS EXTENDED ON CREDIT Although not the major focus of our marketing efforts, we have selectively targeted high-end players.

### s0193
Context (previous sentence): Additionally, third parties with whom we do business or that facilitate our business activities, including exchanges, clearing houses, financial intermediaries, or vendors that provide services or security solutions for our operations, could also be sources of operational and information security risk to us, including breakdowns or failures of their own systems, capacity constraints, and cyber-att
SENTENCE: In recent years, information security risks for financial institutions have risen due to the increased sophistication and activities of organized crime, hackers, terrorists, hostile foreign governments, activists, and other external parties.

### s0194
Context (previous sentence): Our foreign operations are primarily in Canada, the United Kingdom, Iceland, the Netherlands, and Germany.
SENTENCE: The functional currency of our foreign subsidiaries is their local currency.

### s0195
Context (previous sentence): In addition, if terrorist activity, armed conflict, civil, economic or military unrest, natural disasters, global pandemics, embargoes or other economic sanctions, enforcement actions against governments, governmental entities or private entities or political instability occurs in the U.S. or other locations, such events may disrupt our manufacturing, assembly, logistics, security and communicatio
SENTENCE: We have in the past and, may again in the future, experience difficulties relating to employees traveling in and out of countries facing civil unrest or political instability and with obtaining travel visas for our employees.

### s0196
Context (previous sentence): Production Cost Allocation Rider Entergy Arkansas has in place an APSC-approved production cost allocation rider for recovery from customers of the retail portion of the costs allocated to Entergy Arkansas as a result of System Agreement proceedings.
SENTENCE: Other In June 2022 the APSC approved Entergy Arkansas’s compliance tariff filing for a proposed green tariff designed to help participating customers meet their renewable and sustainability goals and to enhance economic development efforts in Arkansas.

### s0197
Context (previous sentence): A disruption, failure or breach of our networks or systems, including as a result of cyber-attacks, could harm our business .
SENTENCE: Our cybersecurity and processing systems, as well as those of financial institutions, merchants, and third-party service providers, may experience errors, interruptions, delays or damage from a number of causes, including power outages, hardware, software and network failures, computer viruses, malware or other destructive software, internal design, manual or usage errors, cyber-attacks, terrorism, workplace violence or wrongdoing, catastrophic events, natural disasters and severe weather conditions.

### s0198
Context (previous sentence): The failure to prevent a cybersecurity incident affecting our or third-party systems could result in the disruption of our services or the disclosure or misuse of sensitive information, which could harm our reputation, decrease demand for our services and products, expose us to liability, penalties, and remedial costs, or otherwise adversely affect our financial performance.
SENTENCE: Our daily business operations depend on our information technology systems and third-party systems (collectively, "IT Systems") for a wide variety of functions, including, among other things, identifying consulting and staffing resources, matching personnel with client assignments, and managing our accounting and financial reporting functions.

### s0199
Context (previous sentence): Although prior disruptions have not been material, the inability of a supplier to deliver, and our inability to secure timely and cost-effective alternatives, could impair our ability to manufacture products or provide services.
SENTENCE: Our operations may be adversely affected by delivery delays, capacity constraints, upstream or downstream production disruptions, price spikes, cyber-related attacks, or decreased availability of materials and commodities arising from war or other hostilities, natural disasters, public health emergencies, increased tariffs or trade restrictions, or other business continuity events.

### s0200
Context (previous sentence): In addition, the 2017 Tax Act will no longer permit deferral of U.S. taxation on Puerto Rico earnings of U.S. companies (or their foreign subsidiaries), although these earnings generally will be taxed in the United States at a reduced 10.5% rate.
SENTENCE: Given Puerto Rico’s challenged economy and hurricane recovery needs, it may be difficult for Puerto Rico to sustain or grow its manufacturing base due to competition from other foreign locations subject to a similar level of U.S. taxation, or U.S. locations due to the reduction in the U.S. corporate tax rate from 35% to 21%.