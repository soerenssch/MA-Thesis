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

### s0051
Context (previous sentence): A business continuity plan is necessary for our global business.
SENTENCE: We have a business continuity plan designed to (i) identify key assets, operations and underlying threats, (ii) define and assess relevant threats (e.g., natural disasters, pandemics, terrorism, etc.) on business operations, (iii) develop and categorize action plans to minimize the impact of the identified threats and (iv) test the adequacy of our action plans.

### s0052
Context (previous sentence): Income from operations for fiscal 2024 was 7.2% of net sales, or $369.8 million, compared to 4.7% of net sales, or $226.6 million, for fiscal 2023.
SENTENCE: The increase in operating income dollars was primarily driven by the increase in gross profit.

### s0053
Context (previous sentence): Some of these tariffs have been paused or reduced, but we cannot predict whether any of these reductions will remain in place or pauses will lapse or be extended, or whether any tariffs will be increased or decreased.
SENTENCE: These additional tariffs, including pauses, reductions or additional increases, as well as a government’s adoption of “buy national” policies or retaliation by another government against such tariffs or policies, have introduced significant uncertainty into the market and may affect the cost to manufacture 17 Table of Contents our products and the prices of and demand for our products, which could have a material and adverse effect on our business, financial condition and results of operations.

### s0054
Context (previous sentence): Further, we may not always be able to develop tools that effectively and efficiently meet the needs of advertisers.
SENTENCE: Advertisers will not do business with us if they do not believe that advertisements on our platform are effective in meeting their campaign goals, if we cannot measure the effectiveness of our advertising products or if they do not believe that their investment in advertising with us will generate a competitive return relative to other alternatives.

### s0055
Context (previous sentence): We are also subject to ongoing reviews of our products, manufacturing processes and facilities by government authorities, and must also produce product data and comply with detailed regulatory requirements.
SENTENCE: In order to obtain regulatory approval of certain new products we must, among other things, demonstrate that the product is appropriate and effective for its intended uses, and that we are capable of manufacturing the product in accordance with applicable regulations.

### s0056
Context (previous sentence): Our sales originating outside the United States represented the majority of our total revenue in fiscal year 2024.
SENTENCE: We anticipate that sales from international operations will continue to represent a substantial portion of our total revenue.

### s0057
Context (previous sentence): The U.S. government may also negotiate reductions or eliminations of Section 232 duties with other trading partners.
SENTENCE: If these or other tariffs or duties expire or if others are relaxed or repealed, or if relatively higher U.S. metal prices make it attractive for foreign metal producers to export their products to the U.S., despite the presence of duties or tariffs, the resurgence of substantial imports of foreign metal could create downward pressure on U.S. metal prices which could have a material adverse effect on our earnings and future results of operations.

### s0058
Context (previous sentence): Worldwide political conditions and threats of terrorist attacks may adversely affect our operations and demand for our products.
SENTENCE: Armed conflicts around the world, including those in Ukraine and Israel, could have an impact on our sales, our supply chain and our ability to deliver products to our customers.

### s0059
Context (previous sentence): Our business could be affected during this period of uncertainty, and perhaps longer, by the impact of the UK's exit from the EU.
SENTENCE: In addition, our business could be negatively affected by new trade agreements between the UK and other countries, including the United States, and by the possible imposition of trade or other regulatory barriers in the UK.

### s0060
Context (previous sentence): For example, our net revenue for the year ended December 31, 2022 was in part negatively impacted by the strengthening of the U.S. dollar against the Euro and the British Pound.
SENTENCE: In addition, we generally pay our employees located outside the United States in the local currency, with a significant portion of those payments being made in Taiwan dollars and Euros, and such expenses were positively impacted in 2022 by the strengthening of the U.S. dollar against these currencies.

### s0061
Context (previous sentence): These industries are characterized by the concentration of a few large participants.
SENTENCE: This concentration of customers affects our overall risk profile, since our customers will be similarly affected by changes in economic, geopolitical, and industry conditions.

### s0062
Context (previous sentence): Congress or U.S. regulatory authorities may take administrative, legislative or regulatory action that could materially interfere with our ability to make sales to certain of our customers, particularly in China.
SENTENCE: We could experience unanticipated restrictions on our ability to sell to certain foreign customers where sales of products and the provision of services may require export licenses or are prohibited by government action.

### s0063
Context (previous sentence): Investor sentiment recovered significantly in the fourth quarter to end 2023 with a solid bullish viewpoint.
SENTENCE: Through an uneven environment in 2023, with shifting views on the trajectory of the U.S. economy, persistent geopolitical unrest, and turmoil beginning early in the year within the banking sector, our “no trade-offs” value proposition continued to resonate with investors.

### s0064
Context (previous sentence): The following graph (“Performance Graph”) compares our cumulative total stockholder return since March 31, 2013 , with the cumulative total stockholder return for the Standard & Poor's MidCap 400 Index, the Russell 2000 Index and our peer group index.
SENTENCE: The Company is included in each of the Standard & Poor's MidCap 400 Index and the Russell 2000 Index.

### s0065
Context (previous sentence): In addition, current economic challenges in China, including any global economic ramifications of these challenges, may continue to put negative pressure on global economic conditions.
SENTENCE: If conditions in the global economy, including Europe, China, Australia and the United States, or other key vertical or geographic markets deteriorate, such conditions could materially adversely 31 Table of Contents affect our business, results of operations, and financial condition.

### s0066
Context (previous sentence): Bribery Act 2010 and the Foreign Corrupt Practices Act.
SENTENCE: We also incur costs in currencies other than our functional currencies in some of the countries in which we operate.

### s0067
Context (previous sentence): VIE contractual relationships are not as effective in providing control over the affiliated Chinese companies as direct ownership, and Ctrip would have to rely on the PRC legal system to enforce those contracts in the event of a breach by one of these entities.
SENTENCE: Further, conflicts of interest could arise to the extent Ctrip's officers or directors are also shareholders, officers or directors of the affiliated Chinese entities.

### s0068
Context (previous sentence): Also, as European countries respond to an increased flow of migrants from the Middle East, travel between countries within the European Union and to and from the region could be subject to increased restrictions or the closing of borders, which could negatively impact travel to, from or within the European Union and adversely affect our business and results of operations.
SENTENCE: Certain jurisdictions, particularly in Europe, are considering regulations intended to address the issue of "overtourism," including by restricting access to city centers or popular tourist destinations or limiting accommodation offerings in surrounding areas, such as by restricting construction of new hotels or the renting of homes or apartments.

### s0069
Context (previous sentence): Supply chain disruptions could continue to impact our ability to timely source necessary components and inputs.
SENTENCE: Import tariffs, including recent U.S. tariffs imposed or threatened to be imposed on China, Canada and Mexico and other countries and any retaliatory actions taken by such countries, could potentially lead to further increases in prices of raw materials or components which are critical to our business.

### s0070
Context (previous sentence): Our results of operations are reported in U.S. dollars.
SENTENCE: While the majority of our revenue is denominated in U.S. dollars, a significant portion of our revenue and costs is denominated in other currencies, such as the Euro, the British pound, the Japanese yen, the Canadian dollar, the Chinese yuan and the Australian dollar.

### s0071
Context (previous sentence): In addition, when we dispose of or sell assets, we may not be able to reinvest the sales proceeds and earn returns similar to those generated by the assets that were sold.
SENTENCE: From time to time we have made, and in the future we may seek to make, investments in companies over which we do not have sole control.

### s0072
Context (previous sentence): Substantially all of our sales in 2023, 2022, and 2021 were made to customers outside the United States.
SENTENCE: Our manufacturing center has been located in Shanghai since 2006 and substantially all of our operations are located in mainland China.

### s0073
Context (previous sentence): Changes in government trade policies could limit the demand for our tools and increase the cost of our tools.
SENTENCE: General trade tensions between the United States and mainland China escalated be ginning in 2018, and have continued to escalate.

### s0074
Context (previous sentence): Weak economic conditions, such as high unemployment, low labor force participation, lower family income, a weak real estate market, lower business investment and lower consumer spending may adversely affect the demand for insurance and financial products and lower the Company’s profitability in some cases.
SENTENCE: In addition, political instability, politically motivated violence or civil unrest, may increase the frequency and severity of insured losses.

### s0075
Context (previous sentence): Our future income, cash flows and fair values of financial instruments are dependent upon prevailing market interest rates.
SENTENCE: Interest Rate Risk Interest rate risk is highly sensitive to many factors, including governmental monetary and tax policies, domestic and international economic and political considerations and other factors beyond our control.

### s0076
Context (previous sentence): In the event our controls should fail or are found to be out of compliance for other reasons, we could be subject to monetary damages, civil and criminal money penalties, litigation and damage to our reputation and the value of our brands.
SENTENCE: We also have been subject, and we will likely be subject in the future, to inquiries or legal proceedings from time to time from regulatory bodies concerning compliance with economic sanctions, consumer protection, competition, tax and travel industry-specific laws and regulations, including but not limited to investigations and legal proceedings relating to the travel industry and, in particular, parity provisions in contracts between hotels and online travel companies, including Expedia Group, and the presentation of information to consumers, as described in Part I, Item 3, Legal Proceedings - Competition and Consumer Matters.

### s0077
Context (previous sentence): An inability to receive products after quality control, shortages of products or difficulties in procuring Signet’s products, or a disruption or shutdown of its digital banner websites, among others, may adversely impact its ability to commercialize, manufacture or market its products in a timely manner, any of which could have an adverse effect on Signet’s results of operations.
SENTENCE: Furthermore, there have been travel advisories imposed related to travel to Israel, and restriction on travel, or delays and disruptions as related to imports and exports may be imposed in the future.

### s0078
Context (previous sentence): The Company also maintains secondary regional headquarters at leased office facilities in Eysins, Switzerland, Shanghai, China and Singapore.
SENTENCE: The Company has a global research and development center in a leased office/lab facility located in Andover, Massachusetts, USA.

### s0079
Context (previous sentence): In addition, insurance companies may no longer offer coverage against certain types of losses such as environmental liabilities or other catastrophic events or, if offered, the expense of obtaining such coverage may not be justified.
SENTENCE: Some of our insurance policies, such as those covering losses due to terrorism and floods, are insured subject to limitations, and in the future, we may be unable to renew our current insurance coverage or initiate new coverage at adequate levels or at reasonable prices.

### s0080
Context (previous sentence): However, there can be no assurance that we will be able to fully mitigate the impact of such tariffs or trade restrictions.
SENTENCE: At this time, the overall impact on our business related to these tariffs remains uncertain and depends on multiple factors, including the duration and potential expansion of current tariffs, future changes to tariff rates, scope, or enforcement, retaliatory measures by impacted trade partners, inflationary effects and broader macroeconomic responses, changes to consumer purchasing behavior, and the effectiveness of our responses in managing these challenges.

### s0081
Context (previous sentence): Our products require transportation from our facilities to the site where they are used, which consumes energy.
SENTENCE: Concern over climate change, including the impact of global warming, has led to federal, state, and international efforts to limit GHG emissions.

### s0082
Context (previous sentence): Like other companies operating or selling internationally, we face risks of non-compliance with the U.S.
SENTENCE: Foreign Corrupt Practices Act (the “FCPA”) and other laws which generally prohibit direct and indirect improper payments to foreign government officials and political parties for the purpose of securing an unfair business advantage.

### s0083
Context (previous sentence): Our federal business includes the maintenance of global networks and the provision of special operations services (e.g., counterterrorism training) that require us to dispatch employees to various countries around the world.
SENTENCE: These countries may be experiencing political upheaval or unrest, and in some cases war or terrorism.

### s0084
Context (previous sentence): If a merchant were to go out of business during the billing period, we may be unable to collect such fees, which could negatively affect our business, financial condition, results of operations and cash flows.
SENTENCE: In addition, our business, growth, financial condition or results of operations could be materially adversely affected by public health emergencies, such as the COVID-19 pandemic, political and economic instability or changes in a country’s or region’s economic conditions, changes in laws or regulations or in the interpretation of existing laws or regulations, whether caused by a change in government or otherwise, increased difficulty of conducting business in a country or region due to actual or potential political or military conflict or action by the United States or foreign governments that may restrict our ability to transact business in a foreign country or with certain foreign individuals or entities.

### s0085
Context (previous sentence): In addition, on January 26, 2017, we acquired Fleet, which has operations in Singapore.
SENTENCE: We generally rely on brokers and distributors for the sale of our products in foreign countries.

### s0086
Context (previous sentence): In addition, the protection afforded under the patent laws of one country may not be the same as that in other countries.
SENTENCE: This means, for example, that our right to exclusively commercialize a product in those countries where we have patent rights for that product can vary on a country-by-country basis.

### s0087
Context (previous sentence): The United States has implemented or proposed, or is considering, various travel restrictions and actions that could affect U.S. trade policy or practices, which could also adversely affect travel to or from the United States.
SENTENCE: Future terrorist attacks, natural disasters, travel advisories or restrictions, health concerns, civil or political unrest or other events outside our control could disrupt our business and operations and adversely affect our results of operations.

### s0088
Context (previous sentence): If, in any taxable year, we fail to qualify for taxation as a REIT and are not entitled to relief under the Code: • we will not be allowed a deduction for distributions to stockholders and would be subject to federal and state income tax on our taxable income at regular corporate income tax rates, which could be substantial in amount, and may require us to borrow additional funds or liquidate some
SENTENCE: We are subject to certain federal, state, local and foreign taxes on our income and assets, including taxes on any undistributed income and state, local or foreign income, franchise, property and transfer taxes.

### s0089
Context (previous sentence): We currently interconnect with network service providers around the world to enable the use by our customers of our products over their networks.
SENTENCE: Although we are in the process of acquiring authorization in many countries for direct access to phone numbers, we expect that we will continue to rely on network service providers for these services.

### s0090
Context (previous sentence): Committee on Foreign Investment in the U.S., or CFIUS.
SENTENCE: In the event that CFIUS reviews one or more of the our investments, there can be no assurances that we will be able to maintain or proceed with such investments on terms acceptable to us.

### s0091
Context (previous sentence): However, economic growth and business spending appear to be slowing, financial market volatility has increased, and opinions vary on whether the U.S. economy can continue to keep growing after more than a decade of growth and recovery following the Great Recession.
SENTENCE: Uncertainties also have arisen as a result of increased tariffs and other changes to U.S. trade policies and reactions to such changes by China and other U.S. trading partners as further discussed below, as well as impact from the recent coronavirus outbreak originating in Wuhan, China.

### s0092
Context (previous sentence): Interruptions in these systems, whether due to system failures, computer viruses, software errors, physical or electronic break-ins, or malicious hacks or attacks on our systems (such as denial of service attacks or use of malware such as ransomware) could affect the security and availability of our services on our mobile applications and our websites and prevent or inhibit users’ access to our se
SENTENCE: Our operations also depend on our ability to protect our databases, computers, and software, telecommunications equipment, and facilities against damage from potential dangers such as fire, flood, power loss, security breaches, computer viruses, telecommunications failures, terrorist attacks, acts of war, electronic and physical break-ins, computer viruses, earthquakes, and similar events.

### s0093
Context (previous sentence): The Chinese government has broad discretion and authority to regulate the technology industry in China.
SENTENCE: Additionally, China’s government has implemented policies from time to time to regulate economic expansion in China.

### s0094
Context (previous sentence): The on-going effects of the decision by British voters to exit the European Union may negatively impact our operations.
SENTENCE: On December 24, 2020, the U.K. and the European Union announced an agreement on the EU-UK Trade and Cooperation Agreement (the EU-UK trade deal) that took effect on January 1, 2021.The trade deal was formally approved by the U.K.

### s0095
Context (previous sentence): These new restrictions have impacted the procurement by ACM Shanghai of certain items from the United States, and of certain items subject to U.S. export controls from outside the United States, for use in manufacturing its products.
SENTENCE: In October 2023, BIS further expanded export controls on semiconductors, semiconductor manufacturing items and items for use in manufacturing designated types of semiconductor manufacturing equipment, including through new licensing requirements covering a broader variety of items, and an expansion in the geographical scope of the controls.

### s0096
Context (previous sentence): Supply chain disruptions could adversely affect our results of operations and financial condition.
SENTENCE: Our supply chain, including transportation availability, staffing, and cost, could be disrupted by natural or human-induced events or conditions, such as power or telecommunications outage, security incident, terrorist attack, war, other geopolitical events, public health crisis, earthquake, extreme weather events, fire, flood, other natural disasters, transportation disruption, labor actions, including strikes, raw materials shortages, financial problems or insolvency, trade regulations or actions, inadequate manufacturing capacity or utilization to meet demand, or other reasons Supply chain disruptions could adversely affect our results of operations and financial condition.

### s0097
Context (previous sentence): Consumer demand for credit (i.e., rates of spending and levels of indebtedness) also tends to grow more slowly or decline during periods of economic contraction or slow economic growth.
SENTENCE: Our customer base suffers when financial markets experience volatility, illiquidity and disruption, and the potential for increased and continuing disruptions going forward presents considerable risks to our business and revenue.

### s0098
Context (previous sentence): Brexit is likely to lead to legal uncertainty and potentially divergent national laws and regulations as the UK determines which European Union laws to replace or replicate.
SENTENCE: Any of these effects of Brexit, and any other effects we cannot anticipate, could adversely affect our business, business opportunities, results of operations, financial condition and cash flows.

### s0099
Context (previous sentence): We also take affirmative steps to prevent and detect fraud and report, to appropriate authorities, any known or suspected acts of fraud in accordance with existing laws and requirements.
SENTENCE: Schwab also faces operational risk when we employ the services of various third parties, including domestic and international outsourcing of certain technology, processing, servicing, and support functions.

### s0100
Context (previous sentence): Houston Electric depends on these REPs to remit payments on a timely basis.
SENTENCE: Houston Electric’s PUCT-approved tariff outlines the remedies available to Houston Electric in the event that a REP defaults on amounts owed.