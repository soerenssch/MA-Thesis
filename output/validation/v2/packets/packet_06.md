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

### s0251
Context (previous sentence): Past terrorism attacks in the U.S. and in other locations worldwide and the potential for future attacks have caused commercial insurance for such threats to become extremely difficult to obtain.
SENTENCE: In the event that we are found liable following an act of terrorism, the insurance we currently have in place would not fully cover the claims for damages.

### s0252
Context (previous sentence): The exportation, re-exportation, transfers within foreign countries and importation of our products, including by our partners, must comply with these laws and regulations, and any violations may result in reputational harm, government investigations and penalties, and a denial or curtailment of exporting.
SENTENCE: Complying with export control and sanctions laws for a particular sale may be time consuming, may increase our costs, and may result in the delay or loss of sales opportunities.

### s0253
Context (previous sentence): In addition, the Company holds a 30% investment in a credit rating agency licensed in China.
SENTENCE: China has laws applicable to domestic credit rating agencies as well as foreign investment in such entities and entities in general (including national security review).

### s0254
Context (previous sentence): Additionally, there may be substantial capital and other costs to comply with regulations and/or increased security costs or insurance premiums, any of which could negatively impact our operating results.
SENTENCE: Our international operations continue to expand, exposing us to additional risks.

### s0255
Context (previous sentence): In the event of a major earthquake, cyclone, monsoon or other natural or man-made disaster, we could experience business interruptions, destruction of facilities and/or loss of life, any of which could materially adversely affect our business.
SENTENCE: In addition, the outbreak of war, political unrest or terrorist activity, diseases, epidemics or pandemics in any of the locations in which we conduct business could severely disrupt our business or the business of our customers and suppliers, which could in turn materially adversely affect our business.

### s0256
Context (previous sentence): For example, an investment in real estate cannot generally be quickly sold, and we cannot predict whether we will be able to sell any hotel we desire to for the price or on the terms set by us or acceptable to us, or the length of time needed to find a willing purchaser and to close the sale of the hotel.
SENTENCE: Moreover, the Code imposes restrictions on a REIT’s ability to dispose of properties that are not applicable to other types of real estate companies.

### s0257
Context (previous sentence): The risks noted above could negatively impact us or require us to: • Contribute additional capital if our partners fail to fund their share of any required capital contributions or are unable to access capital as a result of disruptions in the banking sector; • Contribute additional capital if our partners fail to fund their share of any required capital contributions or are unable to access capit
SENTENCE: We generally seek to maintain control of our partnerships, limited liability companies, and joint venture investments in a manner sufficient to permit us to achieve our business objectives.

### s0258
Context (previous sentence): State regulators have also been increasingly active in implementing privacy and cybersecurity laws, regulations, rules and standards.
SENTENCE: Several states, including states where the Company currently conducts, or may in the future conduct, business, such as California, Nebraska, Virginia and Colorado, have implemented, or are considering implementing, comprehensive data privacy and cybersecurity laws and regulations, including regulations requiring certain financial institutions to implement cybersecurity programs.

### s0259
Context (previous sentence): State Department International Traffic in Arms Regulations (“ITAR”) and U.S. and other foreign country laws such as the Foreign Corrupt Practices Act (“FCPA”), and local laws prohibiting corrupt payments to governmental officials.
SENTENCE: Violations of these laws and regulations could result in fines, criminal sanctions against us, our officers or our employees, prohibitions on the conduct of our business and damage to our reputation.

### s0260
Context (previous sentence): We derive revenue through rental activities of our brands under franchise and license arrangements.
SENTENCE: These arrangements are subject to various international, federal and state laws and regulations that impose limitations on our interactions with counterparties.

### s0261
Context (previous sentence): We may not be able to compete by differentiating ourselves based on the quality, availability and delivery of our pr oducts or our customer service.
SENTENCE: Addit ionally, we may not be able to reduce our cost structure and our selling prices to be competitive with others, and tariffs introduced to protect manufacturers in the United States and Canada from foreign price competition may not be fully effective.

### s0262
Context (previous sentence): Many of these factors and risks are present and may be exacerbated within our business operations in China.
SENTENCE: For example, changes in U.S.-China relations, the political environment or international trade policies could result in further revisions to laws or regulations or their interpretation and enforcement, increased taxation, trade sanctions, the imposition of 11 additional import or export duties and tariffs, restrictions on imports or exports, currency revaluations or retaliatory actions, which have had and may continue to have an adverse effect on our business plans and operating results.

### s0263
Context (previous sentence): An obligation to make contributions to pension plans could reduce the cash available for working capital and other corporate uses, and may have an adverse impact on our operations, financial condition and liquidity.
SENTENCE: Climate change, or legal, regulatory or market measures to address climate change, may negatively affect our business, financial condition and results of operations.

### s0264
Context (previous sentence): The Standing Committee of the National People’s Congress, or the Standing Committee, has promulgated the Cyber Security Law, which imposes requirements on entities who build and operate mainland China’s internet architecture or provide services in mainland China over the internet, and the Data Security Law, which imposes data security and privacy obligations on entities and individuals carrying ou
SENTENCE: The Data Security Law also provides for a national security review procedure for data activities that may affect national security and imposes export restrictions on certain data an information.

### s0265
Context (previous sentence): Our business could be adversely affected if we are unable to maintain or obtain alliance and marketing relationships with other air carriers in desired markets. 42 Table of Contents American has established a transatlantic joint business with British Airways, Aer Lingus, Iberia and Finnair, a transpacific joint business with Japan Airlines and a joint business relating to Australia and New Zealand
SENTENCE: The transatlantic joint business benefits from a grant of antitrust immunity from the DOT and was reviewed by the EC in July 2010.

### s0266
Context (previous sentence): For example, the Artificial Intelligence Act (“EU AI Act”) recently came into effect in August 2024 and gives companies one to three years to comply with its various requirements which are principally focused on creating transparency with respect to generative AI systems and AI-generated content.
SENTENCE: Penalties for non-compliance with the EU AI Act include fines as high as 7% of a company’s global annual revenue.

### s0267
Context (previous sentence): In addition, many of our manufacturing facilities and suppliers are located outside of the U.S. and we intend to continue our expansion into emerging and/or faster-growing international markets.
SENTENCE: The functional currency for most of our foreign operations is the applicable local currency.

### s0268
Context (previous sentence): West Coast in sufficient amounts to fuel its vessels or at a reasonable cost, as increased demand for LNG could decrease available supply of LNG and increase prices.
SENTENCE: Governments have in the past and may again in the future impose tariffs on LNG that also may increase supply costs.

### s0269
Context (previous sentence): We face exposure to foreign currency exchange rate fluctuations, and such fluctuations could adversely affect our business, results of operations and financial condition.
SENTENCE: As our international operations expand, our exposure to the effects of fluctuations in currency exchange rates grows.

### s0270
Context (previous sentence): Any such difficulties could have an adverse effect on our business, results of operations and financial condition.
SENTENCE: Threats of cyber-attacks or terrorism could affect our business.

### s0271
Context (previous sentence): We have also audited, in accordance with the standards of the Public Company Accounting Oversight Board (United States) (PCAOB), the Company's internal control over financial reporting as of January 31, 2025, based on criteria established in lnternal Control - lntegrated Framework (2013) issued by the Committee of Sponsoring Organizations of the Treadway Commission and our report dated April 1, 20
SENTENCE: Opinion on the Financial Statements We have audited the accompanying consolidated balance sheets of Urban Outfitters, Inc. and subsidiaries (the "Company") as of January 31, 2025 and 2024, the related consolidated statements of income, comprehensive income, shareholders' equity, and cash flows for each of the three years in the period ended January 31, 2025, and the related notes (collectively referred to as the "financial statements").

### s0272
Context (previous sentence): Further, the United States has imposed economic sanctions, and could impose further sanctions in the future, that affect transactions with designated countries, including Cuba, Iran, Crimea region, North Korea and Syria, and nationals and others of those countries, and certain specifically targeted individuals and entities engaged in conduct detrimental to U.S. national security interests.
SENTENCE: These sanctions are administered by the OFAC and are typically known as the OFAC regulations.

### s0273
Context (previous sentence): Trade disputes and protectionist measures, or continued uncertainty about such matters, could result in declining consumer confidence and slowing economic growth or recession, and could cause our customers to reduce, cancel, or alter the timing of their purchases with us.
SENTENCE: Sustained trade tensions could lead to long-term changes in global trade and technology supply chains, which could adversely affect our business and growth prospects.

### s0274
Context (previous sentence): From time to time, terrorist attacks worldwide have caused instability in global financial markets.
SENTENCE: The Company continues to monitor the ongoing conflict between Russia and Ukraine, as well as other conflicts, including the ongoing conflicts in the Middle East, for any potential disruptions to the Company's operations.

### s0275
Context (previous sentence): Our success, growth, and financial results depend in part on our continuing ability to attract, retain, and motivate highly qualified people at all levels, including management, technical, compliance, and sales personnel.
SENTENCE: Competition for these individuals can be intense, and we may not be able to retain our key people, or attract, assimilate, or retain other highly-qualified individuals in the future, which could harm our future success.

### s0276
Context (previous sentence): Accordingly, stockholders may need to sell their shares of our common stock to realize a return on their investment, and stockholders may not be able to sell their shares at or above the price they paid for them.
SENTENCE: Future sales of our common stock or other securities convertible into our common stock could cause the market value of our common stock to decline and could result in dilution of stockholders’ shares.

### s0277
Context (previous sentence): In addition, changes in our products or services, or changes in applicable export or economic sanctions regulations may create delays in the introduction and deployment of our products and services in international markets, or, in some cases, prevent the export of our products or provision of our services to certain countries or end users.
SENTENCE: Any change in export or economic sanctions regulations, shift in the enforcement or scope of existing regulations, or change in the countries, governments, persons or technologies targeted by such regulations, could also result in decreased use of our products and services, or in our decreased ability to export our products or provide our services to existing or prospective customers with international operations.

### s0278
Context (previous sentence): The Company’s intrastate NGL transportation services are subject to the TRRC regulations and must be provided in a manner that is just, reasonable and non-discriminatory.
SENTENCE: Such operations could be subject to additional regulation if the NGLs and crude oil are transported in interstate or through foreign commerce, whether by the Company’s pipelines or other means of transportation.

### s0279
Context (previous sentence): Debt Our outstanding debt consisted of floating- and fixed-rate unsecured term loans, convertible senior notes, senior unsecured notes and mortgage loans with varying maturities.
SENTENCE: Our total debt had an aggregate face value of $2.3 billion as of December 31, 2024, as summarized below: December 31, 2024 (in thousands) Revolving credit facilities $ — Term loans 916,652 Convertible senior notes 750,000 Senior unsecured notes 402,400 Mortgage loans 195,413 Total debt at face value $ 2,264,465 December 31, 2024 (in thousands) Revolving credit facilities $ — Revolving credit facilities $ — Term loans 916,652 Term loans 916,652 Convertible senior notes 750,000 Convertible senior notes 750,000 Senior unsecured notes 402,400 Senior unsecured notes 402,400 Mortgage loans 195,413 Mortgage loans 195,413 Total debt at face value $ 2,264,465 Total debt at face value $ 2,264,465 For further discussion on the components of our debt, see Note 5.

### s0280
Context (previous sentence): If we cannot make scheduled payments on our debt, we will be in default and, as a result: • our debt holders could declare all outstanding principal and interest to be due and payable; • our debt holders could declare all outstanding principal and interest to be due and payable; • the lenders under our credit agreements could terminate their commitments to lend us money; and • the lenders under ou
SENTENCE: The terms of our credit agreements restrict our operations, particularly our ability to respond to changes or to take certain actions.

### s0281
Context (previous sentence): While we do not rely on any single supplier or vendor for the majority of our materials and skilled labor, we may experience difficulties obtaining necessary materials from suppliers or vendors whose supply chains might become impacted by economic or political changes, shortages of shipping containers and/or means of transportation, or difficulties obtaining adequate skilled labor from third-party
SENTENCE: It is uncertain whether we would be able to source the essential commodities, supplies, materials and skilled labor timely or at all without incurring significant costs or delays, particularly during times of economic uncertainty resulting from events outside of our control, including, but not limited to, federal policies and the ongoing or future geopolitical conflicts.

### s0282
Context (previous sentence): Our business is subject to risk based on customer exposure to rising costs and reduced customer income.
SENTENCE: Livestock producers may experience increased feed, fuel, transportation and other key costs or may experience decreased animal protein prices or sales, inflationary pressures as a result of interest rate increases or otherwise and including as a result of the uncertainties and potential economic downturn relating to a resurgence of the COVID-19 pandemic or similar public health crises, or relating to armed conflicts, including the armed conflicts between Israel and Hamas (and potential broader military conflict in the region) and between Russia and Ukraine.

### s0283
Context (previous sentence): Regulation related to the provision of services on the internet is increasing, as federal, state, and foreign governments continue to adopt new laws and regulations addressing data privacy and the collection, processing, storage and use of personal information.
SENTENCE: In some cases, foreign data privacy laws and regulations, such as the European Union’s General Data Protection Regulation, also governs the processing of personal information.

### s0284
Context (previous sentence): The U.S.
SENTENCE: Act to Prevent Pollution from vessels, which implements the International Maritime Pollution (MARPOL) treaty, and the Oil Pollution Act of 1990, among many other laws, treaties and regulations, provides for severe civil and criminal penalties related to vessel-generated pollution for incidents in U.S. waters within three nautical miles and in some cases within the 200-mile exclusive economic zone.

### s0285
Context (previous sentence): Our success will depend on industry chip manufacturers adopting our SAPS, TEBO, Tahoe, ECP, furnace and other technologies.
SENTENCE: To date our strategy for commercializing our tools has been to place them with selected industry leaders in the manufacturing of memory and logic chips, the two largest chip categories, to enable those leading manufacturers to evaluate our technologies, and then leverage our reputation to gain broader market acceptance.

### s0286
Context (previous sentence): These signals include, but are not limited to, GPS signals, other GPS-like satellite signals, augmented GPS services, and other RF technologies that link equipment, operations, owners, dealers, and technicians.
SENTENCE: These radio services depend on frequency allocations governed by international and national government agencies.

### s0287
Context (previous sentence): Our products are subject to import and export controls in jurisdictions in which we distribute or sell our products.
SENTENCE: Import and export controls and economic sanctions laws and regulations include restrictions and prohibitions on the sale or supply of certain products and on our transfer of parts, components, and related technical information and know-how to certain countries, regions, governments, persons and entities.

### s0288
Context (previous sentence): In addition to economic and political risk, a risk associated with our European manufacturing operations is the higher relative expense and length of time required to adjust manufacturing employment capacity.
SENTENCE: We also face political risks in the U.S., including tax or regulatory risks or potential adverse impacts from legislative impasses over, or significant legislative, regulatory or executive changes in fiscal or monetary policy and other foreign and domestic government policies, including, but not limited to, trade policies and import/export policies.

### s0289
Context (previous sentence): If ED or other regulator determines that statements made by us or on our university partner’s behalf are in violation of the regulations, we could be subject to sanctions and other liability, which could have a material adverse effect on our business.
SENTENCE: To the extent we are performing return to Title IV calculations for our university partner institutions, we are subject to sanctions if we fail to correctly calculate and timely return Title IV program funds for students who withdraw before completing their educational program.

### s0290
Context (previous sentence): Under this mechanism, NW Natural recovers CCA costs and will defer any difference between forecasted and actual costs in the following year.
SENTENCE: Additionally, under the approved tariff, proceeds from the sale of allowances, which is required under the CCA, would be used to offset CCA compliance costs for low-income customers.

### s0291
Context (previous sentence): In accordance with the FASB’s guidance, the ESPP is non-compensatory. 5.
SENTENCE: Segments and Nature of the Business Our segments include the VITAS segment and the Roto-Rooter segment.

### s0292
Context (previous sentence): In particular, since we have significant operations in China, our business development plans, results of operations and financial condition may be materially and adversely affected by significant political, social and economic developments in China.
SENTENCE: A slowdown in economic growth in China could adversely impact our customers, prospective customers, suppliers, distributors and partners in China, which could have a material adverse effect on our results of the operations and financial condition.

### s0293
Context (previous sentence): Further, the interruption or curtailment of trade between Israel and its trading partners, as a result of terrorist attacks or hostilities, conflicts between Israel and any other Middle Eastern country or organization, or any other cause, could significantly harm our business.
SENTENCE: Additionally, current or future tensions or conflicts in the Middle East could materially and adversely affect our business, operating results, financial condition and cash flows.

### s0294
Context (previous sentence): Our failure to comply with the laws, regulations, and supervisory actions to which we are subject, even if the failure is inadvertent or reflects a difference in interpretation, could subject us to fines, other penalties, and restrictions on our business activities, any of which could adversely affect our business, financial condition, cash flows, results of operations, capital base, and/or the pr
SENTENCE: Failure to comply with consumer protection, privacy, data protection, or cybersecurity laws and requirements could subject us to civil and criminal penalties or litigation, including class actions, and have a material adverse effect on our business.

### s0295
Context (previous sentence): In addition, there are risks associated with large scale manufacturing for clinical trials or commercial scale including, among others, cost overruns, potential problems with process scale-up, process reproducibility, stability issues, compliance with good manufacturing practices, lot consistency and timely availability of raw materials.
SENTENCE: Even if we obtain marketing approval for any of our investigational products, there is no assurance that our manufacturers will be able to manufacture the approved product to specifications acceptable to the FDA or other comparable foreign regulatory authorities, to produce it in sufficient quantities to meet the requirements for the potential commercial launch of the product or to meet potential future demand.

### s0296
Context (previous sentence): In addition, we own four hotels located in seismically active areas of California and five hotels located in areas that have an increased potential to experience hurricanes (Florida, Hawaii, and Louisiana).
SENTENCE: We have acquired and intend to maintain comprehensive insurance on each of our hotels, including liability, terrorism, fire, and extended coverage, of the type and amount that we believe are customarily obtained for or by hotel owners.

### s0297
Context (previous sentence): Our ability to accurately predict consumer and/or customer demand well in advance of the selling season for our products is impacted by these risks, as well as our reliance on manual processes and judgments that are subject to human error.
SENTENCE: These risks are heightened during periods of macroeconomic and geopolitical volatility, such as we are currently experiencing.

### s0298
Context (previous sentence): The increase was primarily due to increases in service charges on deposit accounts, insurance commissions and fees and interchange and debit card transactions fees partly offset by decreases in other non-interest income and other charges, commissions and fees.
SENTENCE: The increase in service charges on deposit accounts was primarily related to increases in overdraft/insufficient funds charges on consumer and commercial accounts and, to a lesser extent, commercial service charges partly offset by a decrease in consumer service charges.

### s0299
Context (previous sentence): These gains and losses have been recorded in selling and administrative expense in the consolidated statements of comprehensive income.
SENTENCE: We also enter into forward contracts to exchange foreign currencies for United States dollars in order to hedge our currency transaction exposures on intercompany receivables denominated in foreign currencies.

### s0300
Context (previous sentence): Ultimately, the COVID-19 pandemic could have a material adverse impact on the Company’s business, financial positions, results of operations and cash flows.
SENTENCE: RISKS RELATED TO MACROECONOMIC CONDITIONS The Company’s international operations may be negatively affected by political events, wars or terrorism and regulatory changes, related to either a specific country or a larger region.