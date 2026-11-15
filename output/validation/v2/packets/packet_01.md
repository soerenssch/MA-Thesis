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

### s0001
Context (previous sentence): Any system or service disruptions, including those caused by ongoing projects to improve our information technology systems and the delivery of services, whether through our shared services organization or outsourced services, if not anticipated and appropriately mitigated, could materially and adversely affect our business including, among other things, an adverse effect on our ability to perform
SENTENCE: We, and the service providers, suppliers and subcontractors on which we rely, are also subject to systems failures, including network, software or hardware failures, whether caused by us, third-party service providers, cybersecurity threats, malicious insiders, natural disasters, power shortages, terrorist attacks, pandemics or other events, which could cause loss of data and interruptions or delays in our business, cause us to incur remediation costs, subject us to claims and damage our reputation.

### s0002
Context (previous sentence): In some instances, however, the manufacturing of certain product lines is concentrated in one or only a few of our plants.
SENTENCE: The functioning of our manufacturing and distribution assets and systems could be disrupted for reasons either within or beyond our control, including, without limitation: extreme weather or longer-term climatic changes; natural disasters; pandemic; war; accidental damage; disruption to the supply of material or services; product quality and safety issues; systems failure; workforce actions; or environmental matters.

### s0003
Context (previous sentence): We are subject to a variety of environmental laws relating to the manufacture of our products.
SENTENCE: If there are changes to the current regulations, we may be required to make product design changes which may result in excess or obsolete inventory, which could adversely impact our operating results.  We make commitments to our third-party contract manufacturers and other suppliers to manage lead times and meet product forecasts and to other parties to purchase various key components used in the manufacture of our products.

### s0004
Context (previous sentence): Foreign Currency Translation and Remeasurement The majority of the Company's business is transacted in U.S. dollars; however, the functional currencies of some of the Company's subsidiaries are their local currencies.
SENTENCE: In accordance with ASC No. 830, Foreign Currency Matters (“ASC 830”), for a subsidiary of the Company that has a functional currency other than the U.S. dollar, gains and losses resulting from the translation of the functional currency into U.S. dollars for financial statement presentation are not included in determining net income, but are accumulated in the cumulative translation adjustment account as a separate component of shareholders' equity (accumulated other comprehensive income / (loss)).

### s0005
Context (previous sentence): In addition, we may incur certain additional costs to comply with the disclosure requirements, including costs related to conducting diligence procedures to determine the sources of conflict minerals that may be used or necessary to the production of our products and, if applicable, potential changes to products, processes or sources of supply as a consequence of such verification activities.
SENTENCE: It is also possible that we may face reputational harm if we determine that certain of our products contain minerals not determined to be conflict-free and/or we are unable to alter our products, processes or sources of supply to avoid such materials.

### s0006
Context (previous sentence): Our sales are affected by weather conditions.
SENTENCE: Our DTC sales are dependent in part on the weather and our DTC sales growth is likely to be adversely impacted or may even decline in years in which weather conditions do not stimulate demand for our products.

### s0007
Context (previous sentence): Accordingly, our equity holders do not control these policies.
SENTENCE: OUR OWNERSHIP STRUCTURE AND RELATED-PARTY TRANSACTIONS MAY GIVE RISE TO CONFLICTS OF INTEREST.

### s0008
Context (previous sentence): In connection with the termination of the agreement, we took a $12 million impairment charge, in addition to suffering losses from legal fees and other expenses.
SENTENCE: Additionally, because we had expected Ziglu’s team and technology to help accelerate our international expansion, the termination of the deal has delayed our plans to expand our operations in Europe, particularly with respect to cryptocurrency trading.

### s0009
Context (previous sentence): Acts of terrorism, war, natural disasters, severe weather, and political, economic and military conditions may impede our ability to operate or may negatively impact our financial results.
SENTENCE: Terrorist attacks and other acts of war or hostility have created many economic and political uncertainties.

### s0010
Context (previous sentence): Factors beyond our control can significantly influence the fair value of investment securities in our portfolio and can cause potential adverse changes to the fair value of these investment securities, potentially reducing AOCI and/or earnings.
SENTENCE: These factors include, but are not limited to, rating agency actions in respect of the securities, defaults by, or other adverse events affecting the issuer or with respect to the underlying securities, and changes in market interest rates and continued instability in the capital markets.

### s0011
Context (previous sentence): Products developed and manufactured in our foreign locations are subject to export controls of the applicable foreign nation.
SENTENCE: Obtaining export licenses can be difficult, costly and time-consuming and we may not always be successful in obtaining necessary export licenses, and our failure to obtain required import or export approval for our products or limitations on our ability to export or sell our products imposed by these laws may harm our international and domestic revenues.

### s0012
Context (previous sentence): In addition, we are required to pay a quarterly commitment fee with respect to the unused portion of the revolving credit facility at an applicable rate per annum ranging from 0.125% to 0.300% depending on our credit rating.
SENTENCE: We may issue standby letters of credit of up to $250.0 million in the aggregate under the revolving credit facility.

### s0013
Context (previous sentence): These risks and uncertainties include the following: ● The U.S.
SENTENCE: Patent and Trademark Office and various foreign governmental patent agencies require compliance with a number of procedural, documentary, fee payment and other provisions during the patent process.

### s0014
Context (previous sentence): We attempt to monitor and mitigate our exposure and modify our systems when warranted and we have implemented certain business continuity items including data backups at alternative sites.
SENTENCE: Nevertheless, these systems are vulnerable to, and at times have suffered from, among other things, damage from power loss or natural disasters, computer system and network failures, loss of telecommunication services, physical and electronic loss of data, terrorist attacks, security breaches and computer viruses.

### s0015
Context (previous sentence): Ongoing International Conflicts and Tensions The conflict in Ukraine, the Israel-Hamas war and related price volatility and geopolitical instability could negatively impact our business.
SENTENCE: In late February 2022, Russia launched significant military action against Ukraine, and in October 2023, Israel launched a military response against Hamas in Gaza.

### s0016
Context (previous sentence): During the quarter ended December 31, 2020, such a short-seller publication was issued with respect to our company and certain members of the management team, and was referenced by the plaintiffs in the litigation described in “Item 3.
SENTENCE: Legal Proceedings.” General Our production facilities could be damaged or disrupted by a natural disaster, war, terrorist attacks or other catastrophic events.

### s0017
Context (previous sentence): We are subject to the regular examination of our income tax returns by various tax authorities.
SENTENCE: Examinations in material jurisdictions or changes in laws, rules, regulations or interpretations by local taxing authorities could result in impacts to tax years open under statute or to foreign operating structures currently in place.

### s0018
Context (previous sentence): In an attempt to combat inflation, countries and regions have used monetary policy, through increasing central bank interest rates, and such actions have caused, and may continue to cause, volatility in currency exchange rates.
SENTENCE: External events such as Brexit have caused, and may in the future cause, significant volatility in currency exchange rates, especially among the U.S. dollar, the British pound sterling and the euro.

### s0019
Context (previous sentence): Factors beyond our control can significantly influence the fair value of securities in our portfolio and can cause potential adverse changes to the fair value of these securities.
SENTENCE: These factors include, but are not limited to, rating agency actions in respect of the securities, defaults by the issuer or with respect to the underlying securities, and changes in market interest rates or instability in the capital markets.

### s0020
Context (previous sentence): New Accounting Pronouncements See Note 16 to the consolidated financial statements for a discussion of new accounting pronouncements. 31 Item 7A.
SENTENCE: Quantitative and Qualitative Disclosures About Market Risk Market risk is the potential loss arising from adverse changes in market rates and prices such as commodity prices, foreign currency exchange rates and interest rates.

### s0021
Context (previous sentence): ACM Shanghai utilizes certain items subject to export controls under the U.S.
SENTENCE: Export Administration Regulations (EAR) in manufacturing and supplying its products.

### s0022
Context (previous sentence): There have been no material changes to our significant accounting policies during the year ended December 31, 2023.
SENTENCE: We are in the process of reviewing the remaining estimated useful lives of our towers and intangible assets and are considering, for U.S.

### s0023
Context (previous sentence): If we are unable to make our mortgage-related debt payments as required, a lender could foreclose on the property or properties securing its debt.
SENTENCE: Additionally, lenders for our international mortgage loan transactions typically incorporated various covenants and other provisions (including loan to value ratio, debt service coverage ratio, and material adverse changes in the borrower’s or tenant’s business) that can cause a technical loan default.

### s0024
Context (previous sentence): Embecta is subject to complex and frequently changing laws in the United States and elsewhere regarding privacy and the processing, collection, use, storage and protection of personal information, and noncompliance with these laws could result in substantial fines or litigation.
SENTENCE: For instance, the EU has also adopted the General Data Protection Regulation (“GDPR”), which applies to personal data involved in Embecta’s operations in the EU or products and services that Embecta offers to EU users involving personal data.

### s0025
Context (previous sentence): As of December 31, 2018 , 3.6% and 30.5% of our total ABR was from the United Kingdom and other European Union countries, respectively.
SENTENCE: Given the ongoing political uncertainty surrounding the form of Brexit (including a potential “hard Brexit” in which the United Kingdom would also give up full access to the European Union single market and customs union), we cannot predict how the Brexit process will finally be implemented and are continuing to assess the potential impact, if any, of these events on our operations, financial condition, and results of operations.

### s0026
Context (previous sentence): The decrease in value-added sales was due to the same factors driving the decrease in net sales.
SENTENCE: EBITDA for the Precision Optics segment was a loss of $73.3 million in 2024 compared to income of $9.9 million in 2023.

### s0027
Context (previous sentence): In addition, competitors might avoid infringement by designing around our intellectual property rights or by developing non-infringing competing technologies.
SENTENCE: Intellectual property rights and our ability to enforce them may be unavailable or limited in some countries, which could make it easier for competitors to capture market share and could result in lost revenue. 25 Financial Market Risks Our retirement and post-retirement pension plans are subject to financial market risks that could adversely affect our future results of operations and cash flows.

### s0028
Context (previous sentence): Foreign or U.S. laws and regulations may cause us to incur substantial costs or subject us to potential liabilities.
SENTENCE: We are subject to certain compliance costs and potential liabilities under various foreign and U.S. federal, state and local environmental, health and safety laws and regulations.

### s0029
Context (previous sentence): In addition, actions by a regulatory agency in a country or region with respect to a product candidate may have an impact on the approval process for that product candidate in another country or region.
SENTENCE: Foreign regulatory authorities often also have the authority to require post-approval studies, such as a PASS and/or PAES, which involve various risks similar to those described above, and may ask for additional data in order to begin a clinical study including phase 3 clinical trials required to submit a MAA in the EU.

### s0030
Context (previous sentence): In the past, companies that have experienced volatility in the market price of their stock have been subject to securities class action litigation.
SENTENCE: We may be the target of this type of litigation in the future.

### s0031
Context (previous sentence): You should also refer to the other information set forth in this Annual Report on Form 10-K, including Item 7 “Management’s Discussion and Analysis of Financial Condition and Results of Operations” and Item 8 “Financial Statements and Supplementary Data.” The following risks could materially and adversely affect our business, financial condition and results of operations, and cause the trading pri
SENTENCE: These risk factors do not identify all risks that we face; our operations could also be affected by factors that are not presently known to us or that we currently consider to be immaterial to our operations.

### s0032
Context (previous sentence): As we pursue our international expansion initiatives, we are subject to certain laws, including the Foreign Corrupt Practices Act, as well as the laws of the foreign countries in which we operate, which may impose new or changing regulatory restrictions and requirements, including in the areas of data privacy, sustainability and responses to climate change.
SENTENCE: Violations of these laws could subject us to actions of government regulatory authorities, including sanctions, import restrictions, and tariffs, or other penalties that could have an adverse effect on our reputation, operating results and financial condition.

### s0033
Context (previous sentence): Our Commercial Real Estate segment offers commercial real estate information and analytics , online marketplaces, and 3D digital twin technology and its principal brands are CoStar, including CoStar Real Estate Manager and CoStar with STR benchmarking, LoopNet, Matterport, BizBuySell, and Ten-X.
SENTENCE: Our Residential Real Estate segment hosts marketplaces which aggregate consumer demand for homes that they can rent or buy and we sell marketing and leads to the agents, owners, landlords, and property management companies that need to reach those consumers with their offerings.

### s0034
Context (previous sentence): In fiscal year 2020, approximately 38% of our sales were generated in countries other than the U.S.
SENTENCE: Our international operations are subject to additional risks, including fluctuations in currency values, foreign currency exchange controls, discriminatory fiscal policies, compliance with U.S. and foreign laws, enforcement of remedies in foreign jurisdictions and other economic or political uncertainties.

### s0035
Context (previous sentence): Additional risks from our multinational business include transportation delays and interruptions, war, terrorist activities, epidemics, pandemics, political instability, import and export controls, local regulation, changes in governmental policies, labor unrest and current and changing regulatory environments.
SENTENCE: In addition, government policies on international trade and investment such as import quotas, tariffs, and capital controls, whether adopted by individual governments or addressed by regional trade blocs, can affect the demand for our customers’ products and services.

### s0036
Context (previous sentence): Any such changes may reduce margins and could adversely affect our operating results.
SENTENCE: Any broad-based change to our prices and pricing policies could cause our revenues to decline or be delayed as our sales force implements and our customers adjust to the new pricing policies.

### s0037
Context (previous sentence): Bribery Act; and corrupt or unethical practices in foreign jurisdictions that may subject us to exposure under applicable anti-corruption and anti-bribery laws such as the U.S.
SENTENCE: Foreign Corrupt Practices Act of 1977, as amended, or FCPA, and the United Kingdom Bribery Act of 2010, or U.K.

### s0038
Context (previous sentence): While the expanded export controls apply to exports to any jurisdiction, exports to certain jurisdictions, such as the United States, are expected to be permitted by certain types of broad general licenses.
SENTENCE: However, it remains to be seen whether the Japanese government will authorize any exports of these items to mainland China by a limited general license or specific license, if at all.

### s0039
Context (previous sentence): Conflict Minerals Regulation, also apply to us.
SENTENCE: All of these regulations and these types of changes in our regulatory environment, particularly in, but not limited to, the U.S., the E.U. and China, may require us to re-design our products or supply chain to ensure compliance with the applicable standards.

### s0040
Context (previous sentence): Certain of our products are subject to EAR and some products, including certain products developed with government funding, are subject to ITAR.
SENTENCE: Products developed and manufactured in our foreign locations are subject to export controls of the applicable foreign nation.

### s0041
Context (previous sentence): We are subject to export restrictions that may limit our ability to sell to certain customers and the U.S.-China trade war could adversely affect our business.
SENTENCE: The U.S. and several other countries levy tariffs on certain goods and impose other trade restrictions that may impact our customers’ investment in manufacturing equipment, reduce the competitiveness of our products, or inhibit our ability to sell products or purchase necessary equipment and supplies.

### s0042
Context (previous sentence): There is global scientific consensus that greenhouse gas (GHG) emissions continue to alter the composition of Earth’s atmosphere in ways that are affecting and are expected to continue to affect the global climate.
SENTENCE: These considerations have led to new international, national, regional, and local legislative and regulatory responses.

### s0043
Context (previous sentence): In addition, we have secured the naming rights to facilities controlled by third parties, such as office towers and a transit center, and any negative events or publicity arising in connection with these facilities could adversely impact our brand.
SENTENCE: Further, entry into markets with weaker protection of brands or changes in the legal systems in countries we operate may impact our ability to protect our brands.

### s0044
Context (previous sentence): In addition, the terminal modernization programs may not result in improved operational productivity or generate expected returns.
SENTENCE: Heightened security measures, war, actual or threatened terrorist attacks, efforts to combat terrorism and other acts of violence may adversely impact the Company’s operations and profitability.

### s0045
Context (previous sentence): To assess the discount rates, we reviewed the methodology used by the Company and considered each input relative to current economic factors.
SENTENCE: We performed sensitivity analyses of significant assumptions to evaluate the changes in the fair value of the indefinite-lived intangible asset that would result from changes in the assumptions.

### s0046
Context (previous sentence): Although our use of distributed systems enables us to provide rapid content delivery to our customers and is intended to mitigate the risks associated with supporting business continuity in the event of an emergency, a system disruption at a third-party hosting service provider could result in a noticeable disruption and performance degradation to our websites.
SENTENCE: Further, our technology infrastructure may be vulnerable to damage or interruption from natural disasters, power loss, telecommunication failures, terrorist attacks, computer intrusions, vulnerabilities and malware (including viruses and malicious software), software errors, computer denial-of-service attacks and other events.

### s0047
Context (previous sentence): In addition, we may become subject to exchange control regulations that restrict or prohibit the conversion of our foreign revenue currencies into United States dollars.
SENTENCE: Any of these factors could decrease the value of revenues and earnings we derive from our international operations and have a material adverse effect on our business.

### s0048
Context (previous sentence): In such event, we could be required to seek licenses from third parties in order to continue offering our products, to re-engineer our products or to discontinue the sale of our products in the event re-engineering cannot be accomplished on a timely basis, any of which could materially and adversely affect our operating results, financial condition and cash flows.
SENTENCE: We are subject to import and export control and trade and economic sanction laws and regulations that could subject us to liability or impair our ability to compete in international markets.

### s0049
Context (previous sentence): At the inception of a contract, the Company determines if the contract contains a lease.
SENTENCE: A contract contains a lease if it conveys the right to control the u se of an identified asset for a period of time in exchange for consideration.

### s0050
Context (previous sentence): This could also create adverse publicity that may have a material adverse effect on our ability to sell our products successfully and on our financial condition and results of operations.
SENTENCE: In addition, outbreaks of disease carried by animals may reduce regional or global sales of particular animal-derived food products or result in reduced exports of such products, either due to heightened export restrictions or import prohibitions, which may reduce demand for our products due to reduced herd or flock sizes.