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

### s0301
Context (previous sentence): Gross Margin Gross margin for fiscal 2025 was 38.8%, compared to 39.1% in fiscal 2024.
SENTENCE: The 30 basis point decline was primarily driven by the following factors: • Tariff-related costs negatively impacted gross margin by 30 basis points in the year. • Tariff-related costs negatively impacted gross margin by 30 basis points in the year. • Unfavorable channel and product mix negatively impacted gross margin by approximately 30 basis points.

### s0302
Context (previous sentence): Many of our Advanced Computing offerings, including Linux-based products and Penguin Solutions’ ClusterWare products, incorporate software components licensed under various open source licenses.
SENTENCE: The terms of many open source licenses to which we are subject have not been interpreted by U.S. or foreign courts, and there is a risk that open source software licenses could be construed in a manner that imposes unanticipated conditions or restrictions on our ability to provide or distribute our products or services.

### s0303
Context (previous sentence): Noncompliance with these laws could have negative consequences, including government investigations, penalties and reputational harm.
SENTENCE: Changes in our products or changes in export, import and economic sanctions laws and regulations may delay us introducing new products in international markets, prevent our customers from using our products internationally or, in some cases, prevent the export or import of our products to or from certain countries altogether.

### s0304
Context (previous sentence): Compliance with the import laws that apply to our businesses may restrict our access to, and may increase the cost of obtaining, certain products and could interrupt our supply of imported inventory. • We are required to comply with import laws and export control and economic sanctions laws, which may affect our transactions with certain customers, business partners and other persons, including de
SENTENCE: In certain circumstances, export control and economic sanctions regulations may prohibit the export of certain products, services and technologies.

### s0305
Context (previous sentence): We have a written Code of Conduct and Ethics (the “Code”) that applies to our directors and employees, including our Chief Executive Officer, Chief Financial Officer and Principal Accounting Officer.
SENTENCE: The Code includes guidelines relating to compliance with laws, including anti-bribery and illegal payment laws, the ethical handling of actual or potential conflicts of interest, the use of corporate opportunities, protection and use of our confidential information, accepting gifts and business courtesies, accurate financial reporting and procedures for promoting compliance with, and reporting violations of, the Code.

### s0306
Context (previous sentence): To the extent that we believe any of these costs are recoverable in rates, cost recovery could be resisted by our regulators and our regulators might attempt to deny or defer timely recovery of these costs.
SENTENCE: Moreover, we cannot predict the ultimate impact of achieving our emissions reduction goals, or the various implementation aspects, on our system reliability or our financial condition and results of operations. 25 Houston Electric and Indiana Electric, as a member of ERCOT and MISO, respectively, could be subject to higher costs for system improvements, as well as fines or other sanctions as a result of FERC mandatory reliability standards.

### s0307
Context (previous sentence): The translation risk is primarily concentrated in the exchange rate between the U.S. dollar and the euro.
SENTENCE: As the U.S. dollar fluctuates against other currencies in which we transact business, revenue and income can be impacted, include revenue decreases due to unfavorable foreign currency impacts.

### s0308
Context (previous sentence): In addition, pandemics and other public health crises, including the occurrence of a contagious disease or illness, such as the recent coronavirus outbreak, or concerns over the possibility of such crises could create economic, market and financial disruptions in the region.
SENTENCE: For example, the ongoing coronavirus outbreak emanating from China at the beginning of 2020 has resulted in massive city-wide quarantines in China, extended shutdown of businesses in the region and increased travel restrictions. 40 Table of Contents 40 Table of Contents A significant deterioration of economic conditions in Asia could expose us to, among other things, economic and transfer risk, and we could experience an outflow of deposits by those of our customers with connections to Asia.

### s0309
Context (previous sentence): The spread of COVID-19 has also disrupted and may continue to disrupt logistics necessary to import, export and deliver products to us and our customers.
SENTENCE: Further, we might experience temporary shortages of labor, making it difficult to provide field service technicians to install or service our equipment.

### s0310
Context (previous sentence): These systems require the collection, retention and transfer of large volumes of personally identifiable information of hotel guests, including credit card numbers.
SENTENCE: These information networks and systems can be vulnerable to threats such as system, network or internet failures; computer hacking or business disruption; cyber-terrorism; viruses, worms or other malicious software programs; and employee error, negligence or fraud.

### s0311
Context (previous sentence): A portion of our business depends on the ability of our employees to obtain the necessary visas and work or entry permits to travel to and do business in the countries where our clients and, in some cases, our delivery centers, are located.
SENTENCE: In recent years, in response to terrorist attacks, the COVID-19 pandemic and related border controls, global unrest and political rhetoric, immigration authorities generally, and those in the United States in particular, have increased the level of scrutiny in granting visas.

### s0312
Context (previous sentence): Approximately 7,500 of our 13,900 employees as of December 31, 2020 were located in China.
SENTENCE: At December 31, 2020, approximately $524 million of cash and marketable securities were held by our foreign subsidiaries, substantially all of which were located in China.

### s0313
Context (previous sentence): Tariffs and other trade measures could adversely affect the Company’s business, financial condition and results of operations.
SENTENCE: Additional or new tariffs, trade restrictions, or other trade measures could adversely impact the Company’s input costs and supply chain, which could reduce availability or increase the cost of goods sold to its customers, especially in KDS.

### s0314
Context (previous sentence): Ken West , 48 2024 Ken West , 48 Ken West , 48 2024 President and Chief Executive Officer, Energy and Sustainability Solutions since January 2024.
SENTENCE: President of UOP from July 2023 to December 2023, President of Advanced Materials from January 2022 to July 2023, Vice President and General Manager of the Fluorine Products business from April 2021 to January 2022, Vice President and General Manager of the Life Sciences, Protective, and Industrial Products business from June 2020 to April 2021, and Vice President and General Manager of the Packaging and Composites business from October 2018 to June 2020. 49 Honeywell International Inc. 49 Honeywell International Inc.

### s0315
Context (previous sentence): Furthermore, fluctuations in foreign currency exchange rates, combined with the seasonality of our business, could affect our ability to accurately predict our future results and earnings.
SENTENCE: Additionally, global events as well as geopolitical developments, including war in Ukraine and the Israel-Hamas war, fluctuating commodity prices, trade tariff developments and inflation have caused, and may in the future cause, global economic uncertainty and uncertainty about the interest rate environment, which has and could in the future amplify the volatility of currency fluctuations.

### s0316
Context (previous sentence): Compliance with these laws and regulations sometimes involves substantial operating costs and capital expenditures.
SENTENCE: Failure to maintain or achieve compliance with these laws and regulations or with the permits required for the Company's operations could result in substantial costs and liabilities, such as fines and civil or criminal sanctions, third-party claims for property damage or personal injury, cleanup costs or temporary or permanent discontinuance of operations, including claims arising from the businesses and facilities that the Company has sold.

### s0317
Context (previous sentence): Compliance with any such regulatory requirements increases our regulatory burden and gives rise to costs and expenses that may be material.
SENTENCE: Our regulators have broad enforcement powers to censure, fine, issue cease-and-desist orders, embargo future business activity or prohibit us from engaging in some of our businesses.

### s0318
Context (previous sentence): We are actively monitoring the situation in Ukraine and assessing its impact on our business, including our suppliers and customers.
SENTENCE: We have no way to predict the progress or outcome of the war in Ukraine or its impacts in Ukraine, Russia or Belarus as the war, and any resulting government reactions, are rapidly developing and are beyond our control.

### s0319
Context (previous sentence): Also, our ability to convert large amounts of patacas and HKDs into U.S. dollars over a relatively short period may be limited. 25 Table of Contents The ability of subsidiaries to make distributions to us depends on the earnings and cash flow generated from gaming operations and various other factors, including dividend requirements to third-party public stockholders in the case of funds being rep
SENTENCE: While currently there is no foreign exchange or capital control restriction applicable to transactions between us and our Singapore, Macao and Hong Kong subsidiaries, we cannot assure you that this will continue to be the case in the future.

### s0320
Context (previous sentence): These integration activities included the closure of duplicate facilities and termination of employees.
SENTENCE: Restructuring expenses for the year ended December 31, 2017 included $2 million, $2 million, and $1 million related to the integration of acquired businesses in our North America, Specialty, and Europe segments, respectively.

### s0321
Context (previous sentence): Our stores are located in public areas where large numbers of people typically gather.
SENTENCE: Terrorist attacks, threats of terrorist attacks, civil unrest, or health epidemics and pandemics (such as COVID-19) involving public areas could cause people not to visit areas where our stores are located.

### s0322
Context (previous sentence): For products subject to the Export Administration Regulations (“EAR”), administered by the Department of Commerce’s Bureau of Industry and Security, the requirement for a license is dependent on the type and end use of the product, the final destination, the identity of the end user and whether a license exception might apply.
SENTENCE: Virtually all exports of products subject to the ITAR require a license.

### s0323
Context (previous sentence): We have exposure to potential terrorist acts that can materially and adversely affect our business, results of operations and/or financial condition.
SENTENCE: Given the reinsurance retention limits imposed under TRIA (as defined below) and its subsequent legislative extensions, and that some or many of our policies may not include a terrorism exclusion, future foreign or domestic terrorist attacks may result in losses that have a material adverse effect on our business, results of operations and/or financial condition.

### s0324
Context (previous sentence): If any of those disruptions become significant, results could include, among other impacts, delays in settling claims, processing new business, renewals, cancellations and endorsements for insureds, billing and collecting premiums, transacting with reinsurers, contracting with and paying vendors, and disruptions to investment operations.
SENTENCE: We rely on vendors, including some located overseas, for a number of services including IT development, IT maintenance support and various business processes, including, among others, certain claims administration, policy administration, and other operational functions.

### s0325
Context (previous sentence): This increased focus on environmental protection and social responsibility initiatives led to the passage of Section 1502 of the Dodd-Frank Wall Street Reform and Consumer Protection Act of 2010 and its implementing SEC regulations.
SENTENCE: The act imposes supply chain diligence and disclosure requirements for certain manufacturers of products containing specific minerals that may originate in or near the Democratic Republic of the Congo and finance or benefit local armed groups.

### s0326
Context (previous sentence): Despite our programs, the extent to which governmental actions will impact our business, financial condition, results of operations and demand for our products and services will depend on future developments, which are highly uncertain and cannot be predicted.
SENTENCE: Continuous changes in bilateral, multilateral, and international trade agreements also have the potential to disrupt or impact Universal operations.

### s0327
Context (previous sentence): Our revenues are dependent on the continued operation of our various manufacturing facilities.
SENTENCE: Although presently all our manufacturing facilities are considered to be in good condition, the operation of our manufacturing facilities involves many risks which could cause product interruptions, including the breakdown, failure or substandard performance of equipment, construction delays, mislabeling, shortages of materials, labor problems, power outages, political and social instability, the improper installation or operation of equipment, natural disasters, terrorist activities, armed conflicts, the outbreak of any highly contagious diseases near our production sites and the need to comply with environmental and other directives of governmental agencies.

### s0328
Context (previous sentence): Additionally, fluctuations in foreign currencies, including devaluations, exchange controls and other restrictions on the repatriation of funds, have significantly affected and may continue to significantly affect our operating performance, liquidity and the value of any cash held outside the U.S. in local currency.
SENTENCE: Such fluctuations in foreign currencies, including devaluations, cannot be predicted by us and can significantly affect the value of our assets located outside the United States.

### s0329
Context (previous sentence): For example, the U.S. government could prevent or restrict exports of refined products, NGLs, natural gas or the conduct of business in or with certain foreign countries.
SENTENCE: In addition, foreign countries could restrict imports, investments or commercial transactions or revoke or refuse to grant necessary permits.

### s0330
Context (previous sentence): Commerce Department’s Export Administration Regulations, U.S.
SENTENCE: Customs regulations, U.S. supply chain regulations and various economic and trade sanctions regulations established by the U.S.

### s0331
Context (previous sentence): In many foreign countries, it is common for others to engage in business practices that are prohibited by our internal policies and procedures or U.S. regulations applicable to us.
SENTENCE: Although we have implemented policies, procedures and training designed to ensure compliance with these U.S. and foreign laws and policies, there can be no complete assurance that any individual employee, contractor, channel partner, or agent will not violate our policies and procedures.

### s0332
Context (previous sentence): In addition, certain laws and regulations, such as the Foreign Corrupt Practices Act and the 18 Foreign Account Tax Compliance provisions of the Hiring Incentives to Restore Employment Act in the U.S., and the Bribery Act of 2010 in the U.K., impact our operations outside of the legislating country by imposing requirements for the conduct of overseas operations, and in several cases, requiring com
SENTENCE: In addition to the complexity of the laws and regulations themselves, the development of new laws and regulations or changes in application or interpretation of current laws and regulations or conflict between them also increases our legal and regulatory compliance complexity.

### s0333
Context (previous sentence): This could greatly affect our ability to market our university partners’ online programs.
SENTENCE: Government agencies, regulatory agencies, and third parties may conduct compliance reviews, bring claims, or initiate litigation against us or our university partners based on alleged violations of the extensive regulatory requirements applicable to us and our university partners, which could cause the imposition of sanctions against us or our university partners.

### s0334
Context (previous sentence): Department of Commerce added certain China-based companies to its entity list, which precludes shipment of semiconductor products to these companies without a license.
SENTENCE: These restrictions could cause a reduction in demand for our products from contract manufacturing customers that manufacture for high performance compute OEMs, as well as a reduction in exports to customers on the entity list.

### s0335
Context (previous sentence): RISKS RELATING TO OUR BUSINESS AND INDUSTRY Macroeconomic conditions, as well as geopolitical events, could have a material adverse impact on our business, results of operations, cash flows and financial condition.
SENTENCE: Global macroeconomic conditions, including ongoing elevated interest rates, moderating inflation, fluctuating foreign currency exchange rates, supply chain issues and inconsistent consumer demand, continue to adversely impact global economic conditions and have had, and may continue to have, a negative impact on our business, results of operations, cash flows and financial condition.

### s0336
Context (previous sentence): The loss of revenue streams and the reduction of lower cost deposits as a source of funds could have a material adverse effect on our financial condition and results of operations.
SENTENCE: External funding which we rely on, in part, to provide liquidity may not be available to us on favorable terms or at all.

### s0337
Context (previous sentence): A significant additional decline in the value of assets for which risk is transferred in market transactions could have an adverse impact on the demand for our solutions.
SENTENCE: Our financial position may be impacted by tax audits or changes in tax laws or tax ruling We are subject to tax in the U.S., various state, and foreign jurisdictions, and are routinely under audit by various tax authorities.

### s0338
Context (previous sentence): These requirements may adversely affect our ability to source related minerals and metals and increase our related cost.
SENTENCE: We face difficulties and increased expenses associated with complying with the related disclosure requirements, such as costs related to determining the source of any conflict minerals used in our products.

### s0339
Context (previous sentence): In addition, existing debt may be refinanced prior to maturity with additional debt or equity financing (or both).
SENTENCE: Certain Maui windstorm and wildfires legal-related costs of HEI and the Utilities are recoverable under $165 million of excess liability insurance, $25 million of miscellaneous professional liability insurance, and $145 million of directors and officers liability insurance policies (see further information in Note 2 of the Consolidated Financial Statements).

### s0340
Context (previous sentence): While we have developed and implemented policies and procedures designed to ensure strict compliance by us and our personnel with the FCPA and other anti-corruption, sanctions and export control laws in jurisdictions in which we operate, such policies and procedures may not be effective in all instances to prevent violations.
SENTENCE: Any determination that we have violated the FCPA or other applicable anti-corruption, sanctions or export control laws could subject us to, among other things, civil and criminal penalties, material fines, profit disgorgement, injunctions on future conduct, securities litigation and a general loss of investor confidence, any one of which could adversely affect our business prospects, financial condition, results of operations or the market value of our Class A common stock.

### s0341
Context (previous sentence): See "Business Segment— Natural Gas Distribution " below. residential customers and 58 degrees Fahrenheit for commercial customers.
SENTENCE: The collections of any unbilled WARM amounts due to tariff caps and floors are deferred and earn a carrying charge until collected, or returned, in the PGA the following year.

### s0342
Context (previous sentence): Our products are subject to import and export controls in jurisdictions in which we distribute or sell our products.
SENTENCE: Import and exports control and economic sanctions laws and regulations include restrictions and prohibitions on the sale or supply of certain products and on our transfer of parts, components, and related technical information and know-how to certain countries, regions, governments, persons and entities.

### s0343
Context (previous sentence): Failure to comply with GDPR requirements could result in penalties of up to 4% of annual worldwide revenue.
SENTENCE: Additionally, other countries have enacted or are enacting data localization laws that require data to stay within their borders.

### s0344
Context (previous sentence): The Utility’s ability to efficiently construct, maintain, operate, protect, and decommission its facilities, and provide electricity and natural gas services safely and reliably is subject to numerous risks, some of which are beyond the Utility’s control, including those that arise from: • the breakdown, failure of, or supply challenges with equipment, electric transmission or distribution lines, 
SENTENCE: For more information, see “The Utility’s operational networks and information technology systems could be impacted by a cyber incident, cybersecurity breach, or physical attack” below. • attacks by third parties, including cyber-attacks, acts of terrorism, vandalism, or war.

### s0345
Context (previous sentence): Decrease in demand, depending on its scope and duration, together with any future issues affecting travel safety, could significantly and adversely affect our business, working capital and financial performance over the short and long-term.
SENTENCE: In addition, the disruption of the existing travel plans of a significant number of travelers upon the occurrence of certain events, such as severe weather conditions, actual or threatened terrorist activity, war or travel-related health events, could result in significant additional costs and decrease our revenues leading to constrained liquidity if we, as we have done historically in the case of severe weather conditions and travel-related health events, provide relief to affected travelers by refunding the price or fees associated with airline tickets, hotel reservations and other travel products and services.

### s0346
Context (previous sentence): During the fiscal year ended August 31, 2018 the interest rate on the 2018 Term Loan Facility was 3.1%.
SENTENCE: Interest is charged at a rate equal to (a) for the 2018 Revolving Credit Facility, either the base rate or 0.9750% above the Eurocurrency rate and (b) for the 2018 Term Loan Facility, either 0.125% above the base rate or 1.125% above the Eurocurrency rate.

### s0347
Context (previous sentence): In connection with the entry into the Gilead Collaboration Agreement in May 2020, we and Gilead also entered into a common stock purchase agreement and an investor rights agreement.
SENTENCE: Our agreements with Gilead pose a number of risks including, but not limited to, the following: • conflicts may arise between us and Gilead, such as conflicts regarding the combinations or indications to pursue or concerning the interpretation of clinical data, the commercial potential of any optioned investigational products, the interpretation of financial provisions or the ownership of intellectual property developed during the collaboration.

### s0348
Context (previous sentence): The success of our businesses is dependent on our ability to continue providing safe and reliable service to our customers while minimizing service disruptions.
SENTENCE: We are exposed to the risk of asset and equipment failures, gas explosions or leaks, accidents, pandemics, natural disasters, severe weather events, acts of war or terrorism or other acts of violence, including active shooter situations, sabotage, physical attacks or security breaches, cyberattacks or other incidents, which could result in damage to or destruction of our substations or other facilities or infrastructure, or damage to persons or property, fire, loss of life, outages, mechanical problems, environmental pollution, electric and gas supply interruptions or other adverse impacts to our business .

### s0349
Context (previous sentence): Prices and availability of petroleum products are subject to political, economic and geographic events, cyber attacks, global conflicts, and market factors, as well as weather-related events and other natural disasters (foreign and domestic), which could increase in frequency and severity due to climate change, each of which are outside our control and may lead to fluctuations in the cost and avai
SENTENCE: Fuel prices also are affected by the rising demand for fuel in developing countries, and could be materially adversely affected by the use of crude oil and oil reserves for purposes other than fuel production and by diminished drilling activity.

### s0350
Context (previous sentence): Varying degrees of political and economic risk exist in these countries.
SENTENCE: As a consequence, the diamond business is subject to various sovereign risks beyond Signet’s control, such as changes in laws and policies affecting foreign trade and investment.