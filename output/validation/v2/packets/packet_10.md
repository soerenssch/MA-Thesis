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

### s0451
Context (previous sentence): In addition, our leases, loans and other agreements may require us to comply with OFAC and related requirements, and any failure to do so may result in a breach of such agreements.
SENTENCE: If a tenant or other party with whom we conduct business is placed on the OFAC list or is otherwise a party with whom we are prohibited from doing business, we may be required to terminate the lease or other agreement or face other penalties.

### s0452
Context (previous sentence): Prior to that, Senior Vice President and Chief Human Resources Officer for AMB Group LLC, which is the investment management and shared services arm of The Blank Family of Businesses, from 2014 through 2018.
SENTENCE: Prior to joining AMB Group LLC, Vice President of Human Resources for International at Equifax Inc. from 2013 through 2014, where she led human resources for all of its global locations.

### s0453
Context (previous sentence): Disruptions or cost increases in our supply chain, including labor shortages, could materially impact our business.
SENTENCE: The supply chain of goods and services could be impacted by several factors, including sanctions, tariffs, manufacturing labor shortages, domestic and international shipping constraints, increases in demand, physical alterations in technologies that create cyber risks, and shortages of raw materials and specialty components.

### s0454
Context (previous sentence): For the year ended December 31, 2022, Section 301 Tariffs totaled approximately $10,201,000, an increase of 52.8% over the $6,678,000 incurred for 2021.
SENTENCE: For 2022, 2021 and 2020, Section 301 Tariffs totaled approximately 2.6%, 1.9% and 2.4%, respectively, of annual revenue, representing a material reduction in our gross profit margin as a percentage of annual revenue.

### s0455
Context (previous sentence): It is unknown whether and to what extent new tariffs (or other new laws or regulations) will be adopted, or the effect that any such actions would have on us or our industry and customers.
SENTENCE: Any unfavorable government policies on international trade, such as export and import controls, capital controls or tariffs, may affect the demand for our products and services, increase the cost of components, delay production, impact the competitive position of our products or prevent us from being able to sell products in certain countries.

### s0456
Context (previous sentence): Fluctuations in foreign currency exchange rates could result in declines in our reported sales and net earnings.
SENTENCE: The changing relationships of the United States dollar to the Canadian dollar, Australian dollar, the Euro, the Swiss franc, the Mexican peso, and certain other foreign currencies have from time to time had a negative impact on our results of operations.

### s0457
Context (previous sentence): Department of State raised their travel advisory for mainland China from Level 3 (reconsider travel) to ).
SENTENCE: The outbreak of COVID- 19 has harmed the Chinese economy, shut down business operations in China and disrupted manufacturing, travel, drayage of containers, and transportation of goods within and from China.

### s0458
Context (previous sentence): For example, our sales in certain emerging markets have suffered from extended periods of disruption due to natural disasters.
SENTENCE: Furthermore, we have also experienced lower than expected sales in certain emerging markets due to local, regional and global restrictions on banking and commercial activities in those countries.

### s0459
Context (previous sentence): For example, the Company cannot terminate leases early for chartered vessels in the CLX+ service.
SENTENCE: The high volumes of freight from China and supply chain congestion at U.S.

### s0460
Context (previous sentence): On March 29, 2019, the actuary for the IAM Pension Fund certified that the fund was in “endangered” status despite reporting a funded status of over 80%.
SENTENCE: Additionally, the IAM Pension Fund’s Board voluntarily elected to enter into “critical” status on April 17, 2019.

### s0461
Context (previous sentence): The increase in sales and marketing expenses included increases of $191 million in employee-related expenses, including share-based compensation, primarily due to higher average headcount, $51 million related to marketing programs, $21 million in facilities and IT-related expenses, and $21 million in travel expenses.
SENTENCE: We expect sales and marketing expenses to increase in absolute dollars as we continue to invest in our domestic and international selling and marketing activities to expand awareness of our brand and product offerings to attract new and existing customers.

### s0462
Context (previous sentence): Weather-related catastrophes may include meteorological events such as hurricanes, severe convective storms and winter weather; and climatological events such as drought, wildfires and heatwaves.
SENTENCE: In addition, catastrophe losses can occur from events such as lava flows in Hawaii and terrorist events in the United States.

### s0463
Context (previous sentence): Further, we are subject to risks associated with disruptions or delays in shipments whether due to port congestion, container shortages, labor disputes (such as the recent port strike), product regulations and/or inspections or other factors, natural disasters or health pandemics, or other transportation disruptions.
SENTENCE: If we experience significant increases in demand or need to replace a significant number of existing suppliers or manufacturers, there can be no assurance that additional supply and manufacturing capacity will be available when required on terms that are acceptable to us, or at all, or that any supplier or manufacturer will allocate sufficient capacity to us in order to meet our requirements.

### s0464
Context (previous sentence): Our reliance on sole or limited suppliers, particularly foreign suppliers, and our reliance on contractors for manufacturing and installation of our products, involves several risks, including a potential inability to obtain an adequate supply of required components, subassemblies or modules; reduced control over costs, quality and timely delivery of components, subassemblies or modules; supplier 
SENTENCE: In addition, our financial results may be impacted by tariffs imposed by the U.S. on goods from other countries and tariffs imposed by other countries on U.S. goods, including the tariffs proposed by the U.S. government on various imports from China and by the Chinese government on certain U.S. goods, the scope and duration of which, if implemented, remain uncertain.

### s0465
Context (previous sentence): Item 2.
SENTENCE: Properties We have delivery centers in 24 countries.

### s0466
Context (previous sentence): Financial Statements and Supplementary Data – Notes to Consolidated Financial Statements – Recently Adopted Accounting Standards.” Recently Issued Accounting Standards See “Item 8.
SENTENCE: Financial Statements and Supplementary Data – Notes to Consolidated Financial Statements – Recently Issued Accounting Standards.” ITEM 7A.

### s0467
Context (previous sentence): These laws and regulations are broad in scope and are subject to evolving interpretation and we have in the past been, and in the future could be, required to incur substantial costs to monitor compliance or to alter our practices.
SENTENCE: Violations of these laws may be punishable by criminal or civil sanctions, including substantial fines, imprisonment of current or former employees and exclusion from participation in governmental healthcare programs.

### s0468
Context (previous sentence): It is possible that we will not be able to develop new technologies, products or distribution channels to align with consumer purchasing behavior and consumer preferences, which could materially and adversely affect our financial condition, results of operations and cash flows. ■ The occurrence or threat of extraordinary events, including natural disasters, political disruptions, terrorist attacks
SENTENCE: Extraordinary events, including natural disasters, political disruptions, terrorist attacks, public health issues, such as the current COVID-19 pandemic, and acts of war may disrupt our business and operations and impact our supply chain and access to necessary raw materials or could adversely affect the economy generally, resulting in a loss of sales and customers.

### s0469
Context (previous sentence): Any impairment of the value of goodwill or other intangible assets recorded in connection with previous acquisitions would result in a non-cash charge against earnings, which could have a material adverse effect on our financial condition and results of operations.
SENTENCE: Risks Related to Economic, Geopolitical and Legal Factors.

### s0470
Context (previous sentence): In addition, we may be subject to successor liability for FCPA violations or other acts of bribery, or violations of applicable sanctions or other export control laws committed by companies in which we or our funds invest or which we or our funds acquire.
SENTENCE: While we have developed and implemented policies and procedures designed to ensure strict compliance by us and our personnel with the FCPA and other anti-corruption, sanctions and export control laws in jurisdictions in which we operate, such policies and procedures may not be effective in all instances to prevent violations.

### s0471
Context (previous sentence): In March 2022, the DOC announced it would initiate an investigation into whether imports of solar cells and panels produced in Cambodia, Malaysia, Thailand and Vietnam are circumventing U.S. rules and laws, such as antidumping and countervailing duty rates, which impose a tariff on imports of solar cells and panels manufactured in China.
SENTENCE: In December 2022, the DOC issued its preliminary findings noting that circumvention was occurring in each of the four countries.

### s0472
Context (previous sentence): We may be adversely affected by conflicts overseas or terrorist attacks; the travel industry continues to face ongoing security concerns.
SENTENCE: Acts of terrorism or fear of such attacks, including elevated national threat warnings, wars or other military conflicts, may depress air travel, particularly on international routes, and cause declines in revenues and increases in costs.

### s0473
Context (previous sentence): Our sales growth is dependent primarily on our ability to attract new customers and increase our activity with existing customers within North America and abroad.
SENTENCE: In recent years, we have increased the resources devoted to developing a multi-dimensional, differentiated service offering, including our Digital Footprint (which incorporates our FMI and eBusiness capabilities), contract accounts, international capabilities, and process and consumption analytics.

### s0474
Context (previous sentence): We cannot predict the likelihood of any such activities or the extent of their adverse impact on our operations. 19 We are also exposed to risks caused by new or ongoing armed conflicts.
SENTENCE: For example, the ongoing war between Russia and Ukraine and the war between Israel and Hamas have caused and continue to cause disruption, instability and volatility in global markets.

### s0475
Context (previous sentence): Our business, prospects, results of operations, cash flows or financial condition could be materially and adversely affected by any of these risks, and, as a result, the trading price of our common stock could decline.
SENTENCE: RISKS RELATING TO OUR BUSINESS AND INDUSTRY Macroeconomic conditions, as well as geopolitical events, could have a material adverse impact on our business, results of operations, cash flows and financial condition.

### s0476
Context (previous sentence): These fluctuations in currency exchange rates may result in losses that materially and adversely affect our results of operations.
SENTENCE: Additionally, we may incur foreign exchange losses in connection with the designation of the U.S. dollar as the functional currency of our international subsidiaries.

### s0477
Context (previous sentence): To the extent that any disruption or security breach results in a loss or damage to our data or applications, or inappropriate disclosure of confidential or proprietary information, we may incur liability, reputation damage and harm to our business operations.
SENTENCE: Any collaboration arrangements that we may enter into in the future may not be successful, which could adversely affect our ability to develop and commercialize our product candidates.

### s0478
Context (previous sentence): However, many of the policies covering casualty losses may be subject to substantial deductibles and carveouts, and we will be self-insured up to the amount of the deductibles and carveouts.
SENTENCE: There are also some losses, including losses from floods, windstorms, fires, earthquakes, hurricanes, acts of war, acts of terrorism or riots, that may not always be insured against or that are not generally fully insured against because it is not practical to do so.

### s0479
Context (previous sentence): TRIA, and its related rules, contain certain definitions, requirements and procedures for insurers filing claims with the Treasury for payment of the federal share of compensation for insured losses under TRIP.
SENTENCE: TRIA also contains specific provisions designed to manage litigation arising out of, or resulting from, a certified act of terrorism.

### s0480
Context (previous sentence): This may significantly increase our cost of doing business, particularly as we expand our localization efforts.
SENTENCE: For example, the GDPR imposes stringent operational requirements for controllers and processors of personal data of individuals in the European Economic Area (the “EEA”), and noncompliance can trigger fines of up to the greater of €20 million or 4% of global annual revenues.

### s0481
Context (previous sentence): System disruptions and defects in our services could result in lost revenue, delays in customer deployment, or legal claims and could be detrimental to our reputation.
SENTENCE: Because we store, process, and use data, some of which contain personal information, we are subject to complex and evolving federal, state, and foreign laws and regulations regarding privacy, data protection, and other related matters, which are subject to change.

### s0482
Context (previous sentence): Southernmost Beach Resort (4) November 30, 2018 Key West, FL 262 60.
SENTENCE: The Marker Key West November 30, 2018 Key West, FL 96 60.

### s0483
Context (previous sentence): These developments could increase the costs of maintaining or improving our properties and could also result in increased compliance costs or additional operating restrictions that could adversely impact our tenants’ businesses and their ability to pay rent, which could adversely affect our financial condition, results of operations and cash flows.
SENTENCE: Potential terrorist attacks, shooting incidents, and other acts of crime or violence could also harm the demand for and value of our properties, including through damage, destruction, or loss at our properties; increased security costs; utility outages; and limited availability of terrorism insurance.

### s0484
Context (previous sentence): Our Future Success Depends on Continued International Sales, and Our Global Operations are Complex, and Present Multiple Challenges to Manage Sales to customers in countries other than the United States accounted for approximately 68%, 69% and 63% of revenues during the years ended June 30, 2018, 2017 and 2016, respectively.
SENTENCE: We anticipate that international sales will continue to account for a significant portion of our revenues for the foreseeable future.

### s0485
Context (previous sentence): Several countries within the European Union continue to experience sovereign debt and credit issues, which causes more volatility in the economic environment throughout the European Union and the U.K.
SENTENCE: Additionally, sales in countries other than the U.S., together with finished goods and raw materials imported into the U.S., are subject to risks related to fundamental changes to tax laws as well as the imposition of tariffs, quotas, trade barriers and other similar restrictions.

### s0486
Context (previous sentence): Reductions in, or eliminations or expirations of, governmental incentives (including the ITC) or NEM policies in regions where we focus our sales efforts could result in decreased demand for and lower revenue from solar PV systems, which would adversely affect sales of our products.
SENTENCE: In addition, our ability to successfully penetrate new geographic markets may depend on new countries adopting and maintaining tax credits, tax incentives, NEM policies, or other programs to promote solar electricity and storage, to the extent such incentives or programs are not currently in place.

### s0487
Context (previous sentence): We are not permitted to market or promote any of our investigational products before we receive marketing approval from the applicable regulatory authority in that foreign market, and we may never receive such marketing approval for any of our investigational products.
SENTENCE: To obtain marketing approval in many foreign countries, we must comply with numerous and varying regulatory requirements of such countries regarding safety and efficacy and governing, among other things, clinical trials and commercial sales, pricing and distribution of our investigational products, and we cannot predict success in these 60 jurisdictions.

### s0488
Context (previous sentence): Our business is subject to numerous legal and regulatory requirements and any violation of these requirements or any misconduct by our employees, subcontractors, agents or business partners could harm our business and reputation.
SENTENCE: In addition to government contract procurement laws and regulations, we are subject to numerous other federal, state and foreign legal requirements on matters as diverse as data privacy and protection, employment and labor relations, immigration, taxation, anti-corruption, import/export controls, trade restrictions, internal and disclosure control obligations, securities regulation and anti-competition.

### s0489
Context (previous sentence): Governmental regulations of imports or exports affecting internet security could affect our revenue.
SENTENCE: Any additional governmental regulation of imports or exports or failure to obtain required export approval of our encryption technologies could adversely affect our international and domestic sales.

### s0490
Context (previous sentence): From time to time we investigate, remediate and monitor soil and groundwater contamination at certain of our operating sites.
SENTENCE: In certain instances where contamination existed prior to our ownership or occupation of a site, landlords or former owners have retained some contractual responsibility for contamination and remediation.

### s0491
Context (previous sentence): This may prevent us from registering our own marks in those jurisdiction, and could adversely affect our ability to effectively operate our business or market certain products.
SENTENCE: War, terrorism, civil unrest or other violence may negatively impact availability of merchandise and/or otherwise adversely impact our business.

### s0492
Context (previous sentence): If we fail to maintain compliance with applicable regulations or obtain government licenses and approvals for our desired international trading activities or technology transfers, we may be forced to recall products and cease their distribution, and we could be subject to civil or criminal penalties.
SENTENCE: Our business is subject to various significant laws and other legal requirements imposed by the U.S. and other countries we conduct business with, including export control laws such as the Export Administration Act, the Export Administration Regulations (“EAR”) and other laws, regulations and requirements governing international trade and technology transfer.

### s0493
Context (previous sentence): Our investment objectives may overlap with the investment objectives of such affiliated investment funds, accounts or other investment vehicles.
SENTENCE: As a result, those individuals may face conflicts in the allocation of investment opportunities among us and other investment funds or accounts advised by or affiliated with our Adviser.

### s0494
Context (previous sentence): In addition, in certain instances, one of our vendors may be the sole source of highly specialized processing services or materials.
SENTENCE: If such vendor is unable or unwilling to manufacture and deliver components to us on the time schedule and of the quality or quantity that we require, we may be forced to seek to engage an additional or replacement vendor, which could result in additional expenses and delays in product development or shipment of product to our 14 customers.

### s0495
Context (previous sentence): Should that occur, we may not be able to accurately report our financial results, prevent fraud, or file our periodic reports in a timely manner, which may cause investors to lose confidence in our reported financial information and may lead to a decline in our stock price.
SENTENCE: In addition, our failure to timely file our periodic reports could eventually result in the delisting of our common stock, regulatory sanctions from the SEC, and/or the breach of the terms contained in our credit facility, or any preferred equity or debt securities we may issue in the future, any of which could have a material adverse impact on our operations and your investment in our common stock.

### s0496
Context (previous sentence): Terrorism risk: The Company has terrorism insurance coverage which excludes losses from nuclear, biological and chemical attacks.
SENTENCE: In the event of a terrorist attack impacting one or more of our properties, we could lose the revenues from the property, our capital investment in the property and possibly face liability claims from residents or others suffering injuries or losses.

### s0497
Context (previous sentence): In April 2022, Entergy Texas filed on behalf of the parties an unopposed settlement agreement supporting approval of Entergy Texas’s proposed voluntary renewable option tariffs.
SENTENCE: As part of the settlement agreement, Entergy Texas agreed to revise the cost allocation between the rate tiers of Rider SVRO and committed to collaborating with and considering the input of customers to develop an asset-backed green tariff program.

### s0498
Context (previous sentence): These laws and regulations provide public sector customers various rights, many of which are not typically found in commercial contracts.
SENTENCE: For instance, the process of evaluating potential conflicts of interest and developing necessary provisions and contract clauses, where needed, may delay or prevent Workday from being awarded certain U.S. federal government contracts.

### s0499
Context (previous sentence): These transactions expose our account balances to movements in foreign currency exchange rates that could have a material effect on our financial results.
SENTENCE: Our primary foreign currency exposure relates to non-U.S. dollar denominated transactions in our international subsidiary operations, the most significant of which is the euro.

### s0500
Context (previous sentence): In addition, we may become subject to exchange control regulations that restrict or prohibit the conversion of our foreign revenue currencies into United States dollars.
SENTENCE: Any of these factors could decrease the value of revenues and earnings we derive from our international operations and have a material adverse effect on our business.