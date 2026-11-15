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

### s0201
Context (previous sentence): In addition, the PRC government continues to play a significant role in regulating industry development by imposing industrial policies.
SENTENCE: The PRC government also exercises significant control over economic growth in the PRC by allocating resources, controlling payment of foreign currency-denominated obligations, setting monetary policy, regulating financial services and institutions, and providing preferential treatment to particular industries or companies.

### s0202
Context (previous sentence): Series A Cumulative Redeemable Preferred Units The Company issued Series A Cumulative Redeemable Preferred Units (“Preferred Units”) on June 12, 2019.
SENTENCE: Because the Transaction was accounted for as a reverse merger, certain Preferred Units that were issued and outstanding were assumed at Closing for accounting purposes.

### s0203
Context (previous sentence): Bribery Act (discussed in greater detail above under " Risks from the improper conduct of employees, agents, contractors, or collaborators could adversely affect our reputation and our business, prospects, operating results, and financial condition "); • other laws and regulatory requirements to which our business activities abroad are subject, such as the FCPA and the U.K.
SENTENCE: Bribery Act (discussed in greater detail above under " Risks from the improper conduct of employees, agents, contractors, or collaborators could adversely affect our reputation and our business, prospects, operating results, and financial condition "); • changes in the political or economic condition of a specific country or region; • changes in the political or economic condition of a specific country or region; • fluctuations in the value of foreign currency versus the U.S. dollar; • fluctuations in the value of foreign currency versus the U.S. dollar; 61 Table of Contents • tariffs, trade protection measures, import or export licensing requirements, trade embargoes, and sanctions (including those administered by the Office of Foreign Assets Control of the U.S.

### s0204
Context (previous sentence): Our failure to maintain and increase the number and quality of relationships with channel partners, and any inability to successfully execute on the partnerships we initiate, could significantly impede our revenue growth prospects in the short and long term.
SENTENCE: Our success depends, in part, on our ability to manage our international research and development operations and related partnerships.

### s0205
Context (previous sentence): Claims of intellectual property infringement are inherently uncertain, and might require us to redesign affected services, enter into costly settlement or license agreements, pay costly damage awards for which we may not have insurance coverage, or face a temporary or permanent injunction prohibiting us from marketing or selling certain of our services.
SENTENCE: Even if we have an agreement for indemnification against such costs, the indemnifying party, if any in such circumstances, may be unable to uphold its contractual obligations.

### s0206
Context (previous sentence): We have significant manufacturing operations in Mexico, Canada and China.
SENTENCE: Changes in U.S. trade policy with these countries (including the North American Free Trade Agreement, NAFTA, or higher duties on imports from China or other countries), or other changes in U.S. laws and policies governing foreign trade, as well as any responsive or retaliatory changes in regulations or policies by such countries, could have an adverse impact on our business, either directly or in the form of increased costs due to their impacts on our supply chain.

### s0207
Context (previous sentence): The discount rate reflects the market rate on December 31 (measurement date) for high-quality fixed income investments with maturities corresponding to our benefit obligations and is subject to change each year.
SENTENCE: The discount rate can be volatile from year to year as it is determined based upon prevailing interest rates as of the measurement date.

### s0208
Context (previous sentence): While management believes the Company will be able to raise the necessary capital, there is no assurance that management’s plans will be successful.
SENTENCE: The potential damages and losses related to the Maui windstorm and wildfires and related lawsuits (see further information in Note 2 of the Consolidated Financial Statements), the suspension of dividends from Hawaiian Electric, the economic impact of higher fuel prices, inflation, higher interest rates, tightening of monetary policy and geopolitical situations, create significant uncertainty, and the Company cannot predict the extent or duration of these conditions, the future effects that these conditions will have on the Company’s financing plan, cost of capital and its ability to access 41 additional capital, or the future impacts on the Company’s financial position, results of operations, and cash flows.

### s0209
Context (previous sentence): These players may make their decision based upon a number of factors, including the compensation they are offered, the makeup and competitiveness of the team bidding for their services, geographic preferences and other non-economic factors.
SENTENCE: There can be no assurance that we will be able to retain players upon expiration of their contracts or sign and develop talented players to replace those who leave for other teams, retire or are injured, traded or released.

### s0210
Context (previous sentence): Systems that are subject to review include, but are not limited to, our accounting systems, estimating systems, material management systems, earned value management systems, purchasing systems and government property systems.
SENTENCE: If improper or illegal activities, errors or system inadequacies come to the attention of the U.S. government, as a result of an audit or otherwise, then we may be subject to civil and criminal penalties, contract adjustments and/or agreements to upgrade existing systems as well as administrative sanctions that may include the termination of our U.S. government contracts, forfeiture of profits, suspension of payments, fines and, under certain circumstances, suspension or debarment from future U.S. government contracts for a period of time.

### s0211
Context (previous sentence): This could have a material adverse impact on our business, results of operations and financial condition.
SENTENCE: We may have limited legal recourse under the laws of China if disputes arise under our agreements with third parties.

### s0212
Context (previous sentence): Weather-related catastrophes may include meteorological events such as hurricanes, severe convective storms and winter weather; and climatological events such as drought, wildfires and heatwaves.
SENTENCE: In addition, catastrophe losses can occur from events such as lava flows in Hawaii and terrorist events in the United States.

### s0213
Context (previous sentence): Henrique Braun 53 President of the Latin America operating unit since January 2021, and prior to that, President of the Brazil business unit from September 2016.
SENTENCE: President of the Greater China and Korea business unit from March 2013 to September 2016.

### s0214
Context (previous sentence): Global economic uncertainties or downturns could adversely affect our business and results of operations, including financial and credit market fluctuations, changes in economic policy, elevated inflation and responsive actions, elevated interest rates, labor shortages, supply chain disruptions, trade uncertainty, political unrest, geographical instability, unanticipated disasters or global health
SENTENCE: Additionally, tariffs, trade barriers and restrictions, and other acts by governments to protect domestic markets or to retaliate against the trade tariffs and restrictions of other nations could negatively affect our business operations.

### s0215
Context (previous sentence): We believe that the state of global economic conditions is particularly uncertain due to recent and expected shifts in political, legislative and regulatory conditions concerning, among other matters, international trade and taxation, and that an uneven recovery or a renewed global downturn may put pressure on our sales due to reductions in customer demand as well as customers deferring purchases.
SENTENCE: Volatile or uncertain economic conditions, as well as continuing political unrest in markets in which we conduct significant business, including Hong Kong, can adversely impact sales and profitability and make it difficult for us and our competitors to accurately forecast and plan our future business activities.

### s0216
Context (previous sentence): To remain qualified as a REIT for U.S. federal income tax purposes, not more than 50% in value of our outstanding Shares may be owned, directly or indirectly, by five or fewer individuals at any time during the last half of any year.
SENTENCE: To facilitate maintenance of our REIT qualification, our Declaration of Trust, subject to certain exceptions, prohibits ownership by any single shareholder of more than five percent of the lesser of the number or value of any outstanding class of common or preferred shares (the “Ownership Limit”).

### s0217
Context (previous sentence): The following table presents information on the portion of the Company’s unpaid claims liability, which is included in other liabilities on the Company's consolidated balance sheets, that relates to tenant insurance for the periods indicated: For the Year Ended December 31, Tenant Reinsurance Claims: 2020 2019 2018 Unpaid claims liability at beginning of year $ 8,109 $ 7,326 $ 5,167 Claims and cla
SENTENCE: These costs are expensed as incurred.

### s0218
Context (previous sentence): Therefore, increases or decreases in the value of the U.S. dollar against major currencies will affect our operating revenues, operating income and the value of balance sheet items denominated in foreign currencies.
SENTENCE: We generally do not mitigate the risks associated with fluctuating exchange rates, although we may from time to time through forward contracts or other derivative instruments hedge a portion of our translational foreign currency exposure or exchange rate risks associated with material transactions which are denominated in a foreign currency.

### s0219
Context (previous sentence): Regulatory inquiries and rumors can tarnish or substantially damage our reputation, even if those inquiries are satisfactorily addressed.
SENTENCE: Our global presence and investments on behalf of our clients around the world could also lead to heightened scrutiny and criticism in an increasingly fragmented geopolitical landscape.

### s0220
Context (previous sentence): If the timing of FDA’s review and approval of new products is delayed, the timing of our or our partners’ development process may be delayed which would result in delayed milestone revenues and materially harm our operations of business.
SENTENCE: Separately, in response to the COVID-19 pandemic, in March 2020, the FDA announced its intention to postpone most inspections of foreign manufacturing facilities, and on March 18, 2020, the FDA temporarily postponed routine surveillance inspections of domestic manufacturing facilities.

### s0221
Context (previous sentence): The increase in cost of sales in 2017 is primarily attributed to the acquisition of TAP in November 2016, Victory motorcycles wind down costs, and manufacturing network realignment costs, partially offset by lower warranty costs. 27 Table of Contents Gross Profit: The following table reflects our gross profit in dollars and as a percentage of sales: For the Years Ended December 31, ($ in millions)
SENTENCE: Consolidated gross profit, as a percentage of sales, increased in 2018 due to lower Victory Motorcycle wind down costs, favorable foreign exchange, and lower warranty expense, partially offset by increased tariff, logistics, and commodity costs.

### s0222
Context (previous sentence): In addition, open skies agreements, which are now in place with a substantial number of countries around the world, provide international airlines with open access to U.S. markets, potentially subjecting us to increased competition on our international routes.
SENTENCE: See also “Our business is subject to extensive government regulation, which may result in increases in our costs, disruptions to our operations, limits on our operating flexibility, reductions in the demand for air travel, and competitive disadvantages.” Our international service exposes us to foreign economies and the potential for reduced demand when any foreign country we serve suffers adverse local economic conditions or if governments restrict commercial air service to or from any of these markets.

### s0223
Context (previous sentence): In addition, media or other reports of perceived security vulnerabilities to our systems or those of our third-party suppliers, even if no breach has been attempted or occurred, could also adversely impact our reputation and materially impact our business. 18 Table of Contents 18 Table of Contents We may lose key business assets, through the loss of data center capacity or the interruption of tele
SENTENCE: Our operations depend on our ability, as well as that of third-party service providers to whom we have outsourced several critical functions, to protect data centers, whether in cloud or dedicated environments, and related technology against damage from hardware failure, fire, flood, power loss, telecommunications failure, impacts of terrorism, breaches in security (such as the actions of computer hackers), natural disasters, or other disasters.

### s0224
Context (previous sentence): The availability of various raw materials and their prices depends on global and local supply and demand forces, governmental regulations (including tariffs and duties), level of production, resource availability, transportation, and other factors, including natural disasters such as floods and earthquakes, and the COVID-19 pandemic.
SENTENCE: In particular, in recent years the consolidation of steel suppliers, shortage of raw materials affecting the production of steel and the increased global demand for steel, including in China and other developing countries, have contributed to an overall tighter supply for steel, resulting in increased steel prices and, in some cases, special surcharges and allocated cut backs of products by steel suppliers.

### s0225
Context (previous sentence): An adverse outcome in any such litigation could require us to pay damages, which may include punitive damages, attorneys’ fees and costs.
SENTENCE: As a result, noncompliance or any related enforcement or civil actions could result in governmental sanctions and possible civil or criminal litigation, which could seriously harm our business and result in a significant diversion of management’s attention and resources.

### s0226
Context (previous sentence): These and any similar future U.S. government restrictions on our suppliers or customers may adversely affect our business operations in mainland China, overall company results or our financial condition.
SENTENCE: Mainland China’s currency exchange control and government restrictions on investment repatriation may impact our ability to transfer funds outside of mainland China, which could materially and adversely affect our ability to grow, make investments or acquisitions that could benefit our business, otherwise fund and conduct our business, or pay dividends on our common stock.

### s0227
Context (previous sentence): As a result of the restructuri ng, we recorded a restructuring charge of $3.7 million for the year ended December 31, 2019.
SENTENCE: Other Income, Net Year Ended December 31, 2019 vs 2018 2018 vs 2017 (in thousands) 2019 2018 2017 Change Change Other income, net $ 1,242 $ 808 $ 508 $ 434 $ 300 Year Ended December 31, 2019 vs 2018 2018 vs 2017 Year Ended December 31, 2019 vs 2018 2018 vs 2017 (in thousands) 2019 2018 2017 Change Change (in thousands) 2019 2018 2017 Change Other income, net $ 1,242 $ 808 $ 508 $ 434 $ 300 Other income, net $ 1,242 $ 808 $ 508 $ 434 $ 300 Other income, net consists of interest and accretion income earned on our cash, cash equivalents and short-term investments and remeasurement gains and losses on foreign currency.

### s0228
Context (previous sentence): As a result, we may be unable to effectively implement our strategy in new jurisdictions.
SENTENCE: Investment opportunities in certain jurisdictions also may be restricted by legal limits on foreign investment in local assets or classes of assets. 17 Table of Contents Our business may be materially adversely affected by geopolitical and other risks associated with global operations.

### s0229
Context (previous sentence): Accordingly, for purposes of consolidation, we translate the assets and liabilities of our foreign subsidiaries into U.S. dollars at the foreign exchange rates in effect at the balance sheet date.
SENTENCE: The unrealized gains or losses resulting from the translation of these foreign denominated assets and liabilities are included as a component of accumulated other comprehensive income (loss) in the Consolidated Balance Sheets.

### s0230
Context (previous sentence): More recently, in late 2023 and early 2024, U.S. officials have suggested potentially targeting Chinese origin legacy semiconductors with additional tariffs.
SENTENCE: Certain U.S. officials have also called for revocation of, or revisions to, China’s permanent normal trade relations (PNTR) status, which would increase tariffs significantly on goods of Chinese origin.

### s0231
Context (previous sentence): In KMT, Company also transports customer cargoes that are imported into the U.S. or which are destined for export from the U.S.
SENTENCE: Trade discussions and arrangements between the U.S. and various of its trading partners are fluid, and existing and future trade agreements are, and are expected to continue to be, subject to a number of uncertainties, including the imposition of new tariffs or adjustments and changes to the products or materials covered by existing tariffs.

### s0232
Context (previous sentence): Our competitors may succeed in developing, acquiring or licensing, on an exclusive basis, pharmaceutical 39 Table of Contents which have also been delayed pending review by the Biden administration until March 22, 2021.
SENTENCE: On November 20, 2020, CMS issued an interim final rule implementing President Trump’s Most Favored Nation executive order, which would tie Medicare Part B payments for certain physician-administered drugs to the lowest price paid in other economically advanced countries, effective January 1, 2021.

### s0233
Context (previous sentence): Our third-party service providers, including cloud service providers could be disrupted by fire, flood, power loss, telecommunications failure, earthquakes, pandemics, acts of war or terrorism, acts of God, malware (including viruses and malicious software), physical or electronic break-ins and other similar events or disruptions.
SENTENCE: Our principal executive offices are located in New York City, a region that has experienced acts of terrorism in the past.

### s0234
Context (previous sentence): We outsource a portion of our research and development activities for both our Video and Cable Access business segments to a third-party partner with engineering resources located in Ukraine.
SENTENCE: Political, social and economic instability and unrest or violence in Ukraine, including the ongoing conflict with Russian-backed separatists or conflict with the Russian Federation directly, could cause disruptions to the business and operations of our outsourcing partner, which could slow or delay the development work our partner is undertaking for us.

### s0235
Context (previous sentence): Components of our Operating Results Net Revenue We generate materially all of our net revenue from the sale of gamer and creator peripherals and gaming components and systems to retailers, including online retailers, gamers and distributors worldwide.
SENTENCE: Our revenue is recognized net of allowances for returns, discounts, sales incentives and any taxes collected from customers. 44 Table of Contents Cost of Revenue Cost of revenue consists of product costs, including costs of contract manufacturers, inbound freight costs from manufacturers to our distribution hubs as well as inter-hub shipments, cost of materials and overhead, duties and tariffs, warranty replacement cost to process and rework returned items, depreciation of tooling equipment, warehousing costs, excess and obsolete inventory write-downs, and certain allocated costs related to facilities and information technology, or IT, and personnel-related expenses and other operating expenses related to supply chain logistics.

### s0236
Context (previous sentence): In June 2021, the United States, the EU and the UK announced agreements to suspend the imposition of these tariffs, contingent upon each party remaining satisfied that subsidies do not arise.
SENTENCE: However, if and to the extent any of these tariffs are reimposed on us without any available means for us to mitigate or pass on the burden of these tariffs to Airbus, the effective cost of new Airbus aircraft required to implement our fleet plan would increase.

### s0237
Context (previous sentence): Consequently, depending on the facts and circumstances, we could face substantial criminal penalties if we knowingly receive individually identifiable health information from a HIPAA-covered health care provider or research institution that has not satisfied HIPAA's requirements for disclosure of individually identifiable health information.
SENTENCE: There are instances where we collect and maintain sensitive personally identifiable information, which may include health information outside of the scope of HIPAA.

### s0238
Context (previous sentence): Any of these disruptions or other extraordinary events outside of our control that impact our operations or the operations of our suppliers and key distributors could affect our business negatively, harming operating results.
SENTENCE: In addition, 7 Table of Contents these types of events also could negatively impact consumer spending in the impacted regions or depending on the severity, globally, which could materially and adversely affect our financial condition, results of operations and cash flows.

### s0239
Context (previous sentence): Higher inflation levels could adversely affect our business, including by further increasing the cost of capital, resulting in a slowdown of the growth of early stage companies, causing companies to stay private longer.
SENTENCE: Factors that are particularly likely to affect price and interest rate levels and volatility, and thus trading and mortgage loan production volumes, include: • global economic and market conditions; • global political conditions including political uncertainty and discord as a result of elections in many jurisdictions, including in the U.S. and the U.K.; and • concerns over recession, inflation, deflation, legislative and regulatory changes, government fiscal and monetary policy, including actions by the Federal Reserve and other foreign monetary units governing bodies, developments related to the U.S. federal debt ceiling, including the possibility of a government shutdown, default by the U.S. government on its debt obligations or related credit rating downgrades, and investor and consumer confidence levels.

### s0240
Context (previous sentence): As of December 31, 2023, approximately half of our footprint has been overbuilt by wired competitors offering high-speed data services with speeds of 100 Mbps or higher.
SENTENCE: Further overbuilding could cause more of our customers to purchase data and video services from our competitors instead of from us.

### s0241
Context (previous sentence): There is no guarantee that our efforts and strategies to expand sales in emerging markets will succeed.
SENTENCE: Emerging market countries may be especially vulnerable to periods of global and local political, legal, regulatory and financial instability, including sovereign debt issues and/or the imposition of international sanctions in response to certain state actions.

### s0242
Context (previous sentence): In addition, U.S. banking agencies and the SEC have adopted or proposed enhanced cyber risk management standards that could apply to us and our financial institution clients and that would address cyber risk governance and management, management of internal and external dependencies, and incident response, cyber resilience and situational awareness.
SENTENCE: Several states and foreign countries also have adopted or proposed new privacy and cybersecurity laws targeting these issues.

### s0243
Context (previous sentence): New regulatory requirements, including more stringent capital rules, could adversely affect financing availability and/or terms from our counterparties, reduce market liquidity and mortgage loan origination and limit activities of significant organizations and entities that are important to our business.
SENTENCE: Tariff actions by the U.S and other countries may adversely affect our business, financial condition and results of operations.

### s0244
Context (previous sentence): The Company’s spot contract rates generally reflect current fuel prices at the time the contract is signed but do not have escalators for fuel.
SENTENCE: Significant increases in the construction cost of tank barges and towing vessels may limit the Company’s ability to earn an adequate return on its investment in new tank barges and towing vessels .

### s0245
Context (previous sentence): Some of these tariffs have been stayed for brief periods of at least 30 days.
SENTENCE: If the provisions of those tariffs are maintained as proposed, we would expect added market volatility, with the longer term impacts to our refining and marketing margin uncertain.

### s0246
Context (previous sentence): For example, cybersecurity risks may increase in the future as Truist continues to expand its mobile-payment and internet-based product offerings and expand the Company’s internal usage of web-based products and applications.
SENTENCE: In addition, cybersecurity risks have significantly increased in recent years in part due to the increased sophistication and activities of organized crime affiliates, terrorist organizations, hostile foreign governments, disgruntled employees or vendors, activists and other external parties, including those involved in corporate espionage.

### s0247
Context (previous sentence): Armed conflicts around the world, such as those in Ukraine and Israel, may exacerbate certain risks we face.
SENTENCE: Armed conflicts around the world, such as those in Ukraine and Israel, as well as the global response to such conflicts, including the imposition of sanctions by the United States and other countries, could create or exacerbate risks facing our business.

### s0248
Context (previous sentence): Additionally, foreign governments outside of the EU are also taking steps to fortify their data privacy laws and regulations.
SENTENCE: For example, some countries in Africa, Asia and Latin America, including Brazil and Egypt, where we have operations, have implemented or are considering GDPR-like data protection laws.

### s0249
Context (previous sentence): Total segment operating income (1) increased $1.7 million, primarily due to the increase in revenue, offset in part by higher accruals for performance-based incentives, the revenue mix at GES, and additional costs to support the growth initiatives of Pursuit. (1) Refer to Note 23 – Segment Information of the Notes to Consolidated Financial Statements (Part II, Item 8 of this 2019 Form 10-K) for a 
SENTENCE: Foreign Exchange Rate Variances We conduct our foreign operations primarily in Canada, the United Kingdom, the Netherlands, Germany, and to a lesser extent, in certain other countries.

### s0250
Context (previous sentence): These laws and regulations generally prohibit companies and their intermediaries from offering or making improper payments to non-U.S. officials for the purpose of obtaining, retaining or directing business.
SENTENCE: Our exposure for violating these laws and regulations increases as our international presence expands and as we increase sales and operations in foreign jurisdictions.