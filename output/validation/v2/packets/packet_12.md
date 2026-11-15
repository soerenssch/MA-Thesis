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

### s0551
Context (previous sentence): Under this mandate, domestic technology vendors are explicitly favored over foreign vendors such as Vicor.
SENTENCE: We believe we experienced reduced demand in certain segments (e.g., rail), notably in 2019, reflecting the significant role of state-owned enterprises in those segments.

### s0552
Context (previous sentence): The recent changes in U.S. trade policy involving the application or increase of tariffs and the subsequent retaliatory measures against the U.S. have created a dynamic environment that may have a material adverse impact on our business.
SENTENCE: While we have deployed strategies to mitigate the impact of these dynamic trade policies, there is no assurance that we will be able to mitigate the full impact of all such tariffs, retaliatory tariffs or other trade policies that have or may develop in this rapidly changing environment.

### s0553
Context (previous sentence): Other potential sources of liquidity include the sale of loans, the utilization of available government and regulatory assistance programs, the ability to acquire brokered deposits, the issuance of additional collateralized borrowings such as Federal Home Loan Bank advances, the issuance of debt or equity securities, and borrowings through the Federal Reserve’s discount window.
SENTENCE: Without sufficient liquidity from these potential sources, we may not be able to meet the cash flow requirements of our depositors and borrowers. 18 Table of Contents Additionally, our access to funding sources in amounts adequate to finance our activities or on terms that are acceptable to us could be impaired by factors specific to us, the financial services industry, or the economy in general.

### s0554
Context (previous sentence): The Organisation for Economic Co-operation and Development ("OECD") initiated the "base erosion and profit shifting" ("BEPS") project to ensure international tax standards keep pace with changes in global business practices and to address situations where multinational businesses may pay little or no tax in certain jurisdictions by shifting profits away from jurisdictions in which the profit gener
SENTENCE: In connection with the BEPS project, the OECD issued "final reports" that propose 15 actions the OECD determined are needed to address base erosion and profit shifting, including: (a) enhancing transparency through the sharing of tax information between countries; (b) prescribing standardized country-by-country reporting and other documentation requirements aimed at identifying where profits, tax and economic activities occur; (c) preventing harmful tax practices including the use of preferential tax regimes; (d) modernizing the OECD's transfer pricing rules related to intangibles; (e) changing the definition of permanent establishment to prevent artificial avoidance of tax nexus; and (f) limiting tax base erosion through interest deductions and other financial payments.

### s0555
Context (previous sentence): We maintain defined benefit pension plans for most U.S. employees, which provide for defined benefit payments after retirement for those employees.
SENTENCE: Canadian and Mexican employees participate in public retirement systems for those countries and are not eligible to participate in the defined benefit pension plans that we maintain for U.S. employees.

### s0556
Context (previous sentence): If delinquencies or defaults on the Company’s loans or investment securities increase, their value and the income derived from them could be adversely affected, and the Company could incur administrative and other costs in seeking a recovery on its claims and any collateral.
SENTENCE: Weak or deteriorating economic conditions also may negatively impact the market value and liquidity of the Company’s investment securities, and the Company may be required to record additional impairment charges if investment securities suffer a decline in value that is determined to have resulted from a credit loss.

### s0557
Context (previous sentence): More recently, in April 2018, the BIS again blocked exports of U.S. products to ZTE, which were lifted in July 2018.
SENTENCE: ZTE is under a court-ordered monitorship, which means that if it does not comply with certain requirements similar export control prohibitions could be imposed again.

### s0558
Context (previous sentence): Safe Harbor Framework, which facilitated personal data transfers to the United States in compliance with applicable EU data-protection laws.
SENTENCE: EU and U.S. political authorities then adopted the EU-U.S.

### s0559
Context (previous sentence): It is possible that we will not generate taxable income in time to use our net operating loss carryforwards before their expiration or at all.
SENTENCE: As of September 28, 2019 , we had gross U.S. federal net operating loss carryforwards of $60.6 million , which expire beginning in 2035 , and gross state net operating loss carryforwards of $36.2 million , which expire beginning in 2025 , as well as $16.1 million in foreign net operating loss carryforwards, of which $1.4 million have an indefinite life.

### s0560
Context (previous sentence): Even if we do find acceptable alternative suppliers, the process of locating and securing these alternatives may be disruptive to our business, which could have an adverse impact on our ability to meet our customers’ needs and reduce our profitability and cash flows.
SENTENCE: In addition, if a significant domestic supply source is discontinued and we cannot find acceptable domestic alternatives, we may need to find foreign sources of supply.

### s0561
Context (previous sentence): The risk factors described below are not our only salient risks.
SENTENCE: Political events, war, terrorism, civil unrest, weather or other natural/environmental disasters, and other risks that are currently unknown or seen as immaterial, could also have a material adverse impact on our business, consolidated financial statements and/or common stock’s market price.

### s0562
Context (previous sentence): Our operations require us to comply with various domestic and international regulations, violations of which could have a material adverse effect on our results of operations, financial condition and cash flows.
SENTENCE: We are exposed to a variety of federal, state, local and international laws and regulations relating to matters such as environmental, workplace, health and safety, labor and employment, customs and tariffs, export and re-export controls, economic sanctions, currency exchange, bribery and corruption and taxation.

### s0563
Context (previous sentence): We maintain property, business interruption, product, general liability, casualty and other types of insurance that we believe are appropriate for our business and operations as well as in line with industry practices.
SENTENCE: However, we are not fully insured against all potential hazards incident to our business, including losses resulting from natural disasters or climate-related exposures, wars, terrorist acts, or cybersecurity incidents.

### s0564
Context (previous sentence): Since inception, we have conducted a substantial majority of our manufacturing operations in San Jose, California.
SENTENCE: We continue to increase our manufacturing capacity in Taiwan and in the Netherlands.

### s0565
Context (previous sentence): Adverse global economic conditions could have a negative impact on our business, results of operations and financial condition and liquidity.
SENTENCE: A general slowdown in the global economy, including a recession, or in a particular region or industry, an increase in trade tensions with U.S. trading partners, inflation or a tightening of the credit markets could negatively impact our business, financial condition and liquidity.

### s0566
Context (previous sentence): In addition, some foreign competitors are subject to less stringent controls on exporting their encryption technologies.
SENTENCE: As a result, they may be able to compete more effectively than we can in the United States and the international internet security market.

### s0567
Context (previous sentence): If one of our suppliers, subcontractors, distributors, resellers, or TPSRs violates labor or other laws or implements labor or other business practices that are regarded as unethical, the shipment of finished products to us could be interrupted, orders could be canceled, relationships could be terminated, and our reputation could be damaged.
SENTENCE: If one of our suppliers or subcontractors fails to procure necessary license rights to trademarks, copyrights, or patents, legal action could be taken against us that could impact the salability of the Company’s products and expose us to financial obligations to a third-party.

### s0568
Context (previous sentence): Bribery Act; • Local business practices which may be in conflict with the U.S.
SENTENCE: Foreign Corrupt Practices Act and U.K.

### s0569
Context (previous sentence): For example, in some countries, we are not considered a regulated telecommunications business subject to regulations surrounding payment into universal service funds and provision of emergency services but in other countries the provision of VoIP services may be a regulated telecommunications business.
SENTENCE: Certain of our products may be used by customers located in countries where voice and other forms of IP communications may be illegal or require special licensing or in countries on a U.S. embargo list.

### s0570
Context (previous sentence): These efforts could influence global supply/demand in the short term.
SENTENCE: China is a significant cigarette market.

### s0571
Context (previous sentence): Changes to or the interpretation and/or application of laws and regulations applicable to cross-border trade and foreign exchange could further impose additional requirements and restrictions, increase costs, and present conflicting obligations.
SENTENCE: Any factors that increase the costs of cross-border trade for us or our customers or that restrict, delay, or make cross-border trade more difficult or impractical, such as trade policies or higher tariffs (as recently threatened or imposed by certain countries, including the U.S.), and general macroeconomic trends and global economic conditions, could reduce our cross-border transactions and volume, materially and negatively impact our revenues and profits and materially harm our business.

### s0572
Context (previous sentence): The Company's raw material supply contracts vary as to terms and duration, with aluminum contracts typically multi-year in duration with fluctuating prices based on aluminum ingot costs and steel contracts typically one year in duration with fixed prices.
SENTENCE: The availability of various raw materials and their prices depends on global and local supply and demand forces, governmental regulations (including tariffs and duties), level of production, resource availability, transportation, and other factors, including natural disasters such as floods and earthquakes, and the COVID-19 pandemic.

### s0573
Context (previous sentence): For example, the World Trade Organization’s resolution on the Large Civil Aircraft Dispute between the United States and the European Union resulted in both bodies imposing tariffs on a variety of products, including leaf tobacco.
SENTENCE: While these tariffs have been temporarily lifted and negotiations continue, drastic changes in global trade remains a risk to our results of operations.

### s0574
Context (previous sentence): The current U.S. administration has imposed tariffs on certain materials imported into the U.S. from China and announced additional tariffs on other goods from China and other countries.
SENTENCE: Moreover, counter-measures have been taken by other countries in retaliation for the U.S.-imposed tariffs.

### s0575
Context (previous sentence): All of these factors and others could disrupt our business directly and could disrupt the business of our customers thereby reducing or delaying orders of our goods and services.
SENTENCE: Prolonged civil unrest, political instability or uncertainty, military activities, or broad-based sanctions could have an adverse effect on our operations and business outlook.

### s0576
Context (previous sentence): Although there is no statutory enforcement in the Cayman Islands of judgments obtained in the United States, the courts of the Cayman Islands will recognize and enforce a foreign money judgment of a foreign court of competent jurisdiction without retrial on the merits based on the principle that a judgment of a competent foreign court imposes upon the judgment debtor an obligation to pay the sum f
SENTENCE: For a foreign judgment to be enforced in the Cayman Islands, such judgment must be final and conclusive and for a liquidated sum, and must not be in respect of taxes or a fine or penalty, inconsistent with a Cayman Islands judgment in respect of the same matter, impeachable on the grounds of fraud or obtained in a manner, and/or be of a kind the enforcement of which is, contrary to natural justice or the public policy of the Cayman Islands (awards of punitive or multiple damages may well be held to be contrary to public policy).

### s0577
Context (previous sentence): General Our production facilities could be damaged or disrupted by a natural disaster, war, terrorist attacks or other catastrophic events.
SENTENCE: Our manufacturing facilities are subject to risks associated with natural disasters, such as earthquakes, fires, floods tsunami, typhoons and volcanic activity, environmental disasters, health epidemics, and other events beyond our control such as power loss, telecommunications failures, and uncertainties arising out of armed conflicts or terrorist attacks.

### s0578
Context (previous sentence): Changes in currency exchange rates affect the U.S. dollar value of the foreign currency-denominated amounts at which our international businesses purchase products, incur costs or sell products.
SENTENCE: In addition, for our U.S.-based businesses, the majority of products are sourced from independent contractors or our manufacturing facilities located in foreign countries.

### s0579
Context (previous sentence): Risk Factors" of this filing and discussion of risks included in the company's SEC filings. 27 COVID-19 Update The global coronavirus ("COVID-19") pandemic and associated counteracting measures implemented by governments and businesses around the world, as well as subsequent accelerated recovery in global business activity, have increased uncertainty in the global business environment and led to s
SENTENCE: More recently, the war in Ukraine has further contributed to some of the disruptive factors.

### s0580
Context (previous sentence): Furthermore, the concentration of our revenues in a limited number of large customers is likely to cause significant fluctuations in our future annual and quarterly operating results.
SENTENCE: A majority of our revenues are generated from exports to foreign countries, primarily in Asia, that are subject to economic and political instability and we compete against a number of Asia-based test contactor, test handler and automated test equipment suppliers.

### s0581
Context (previous sentence): Foreign Corrupt Practices Act, the U.K.
SENTENCE: Bribery Act and local laws which also prohibit corrupt payments to governmental officials or third parties, data privacy requirements, labor relations laws, tax laws, anti-trust or competition laws, U.S., E.U. or U.N. sanctioned country or sanctioned persons mandates, and consumer protection laws.

### s0582
Context (previous sentence): Our ability to enforce our patents also depends on the laws of individual countries and each country’s practice with respect to enforcement of intellectual property rights.
SENTENCE: In addition, if we are unable to maintain our existing license agreements or 45 Table of Contents other agreements pursuant to which third parties grant us rights to intellectual property, including because such agreements expire or are terminated, our financial condition and results of operations could be materially adversely affected.

### s0583
Context (previous sentence): This increase was primarily related to an increase in the North American OTC Healthcare segment, which accounted for $63.0 million , and the International OTC Healthcare segment, which accounted for $15.6 million , largely due to the acquisitions of DenTek and Fleet.
SENTENCE: The DenTek brands, acquired in February 2016, accounted for approximately $56.9 million of revenues in the North American OTC Healthcare and International OTC Healthcare segments not included in the comparable period in the prior year.

### s0584
Context (previous sentence): Foreign Corrupt Practices Act (the “FCPA”), the U.K.
SENTENCE: Bribery Act and/or similar anti-corruption and anti-bribery laws, particularly in emerging market countries; • compliance with the U.S.

### s0585
Context (previous sentence): Changing demand patterns from economic volatility and uncertainty could have a significant negative impact on our results of operations. 22 Additionally, increased operating costs resulting from recent inflationary pressures, including increases in compensation and other expenses for our employees, have adversely affected our profitability and could continue to do so.
SENTENCE: Broad-based inflation will also continue to increase the costs of operating our delivery centers, including, in particular, due to rising or volatile energy prices, which have been and may continue to be amplified by the ongoing conflict between Russia and Ukraine and other geopolitical tensions.

### s0586
Context (previous sentence): The level of uncertainty concerning economic conditions may adversely affect the accuracy of our estimates which may, in turn, impact the reliability of the process. ● The process we use to estimate losses inherent in our credit exposure requires difficult, subjective, and complex judgments, including qualitative factors that pertain to economic conditions and how these economic conditions might i
SENTENCE: The level of uncertainty concerning economic conditions may adversely affect the accuracy of our estimates which may, in turn, impact the reliability of the process. ● The value of the portfolio of investment securities that we hold may be adversely affected by increasing interest rates and defaults by debtors. ● The value of the portfolio of investment securities that we hold may be adversely affected by increasing interest rates and defaults by debtors. ● There have been changes and discussions with respect to U.S. trade policies, legislation, treaties and tariffs, including trade policies and tariffs affecting other countries, including China, the European Union, Canada and Mexico and retaliatory tariffs by such countries.

### s0587
Context (previous sentence): In December 2023, PJM awarded us an approximately $424 million project to address increasing load and reliability issues in Maryland and northern Virginia as part of its 2022 Window 3 competitive solicitation.
SENTENCE: PJM has directed that the project be placed in service in 2027.

### s0588
Context (previous sentence): This environment could lead to further proposals by political candidates and state and federal legislators and regulators, and to the enactment of laws and regulations, applicable to, or limiting, our business.
SENTENCE: For instance, over the last several years, numerous proposals for new federal spending have been discussed by political candidates and/or introduced by legislators to make higher education “free” or substantially so.

### s0589
Context (previous sentence): We manage, utilize, and store sensitive or confidential client or employee data, including personal data and protected health information.
SENTENCE: As a result, we are subject to numerous laws and regulations designed to protect this information, such as the U.S. federal and state laws governing the protection of health or other personally identifiable information, including the Health Insurance Portability and Accountability Act, and international laws such as the European Union General Data Protection Regulation.

### s0590
Context (previous sentence): The safety profile of upadacitinib was consistent with previously reported clinical trials and no new safety signals were detected. • In July 2018, AbbVie initiated two Phase 3 clinical trials to evaluate the efficacy and safety of upadacitinib in subjects with moderate to severe atopic dermatitis. • In July 2018, AbbVie initiated two Phase 3 clinical trials to evaluate the efficacy and safety of 
SENTENCE: Risankizumab • In January 2018, AbbVie initiated two Phase 3 clinical trials to evaluate the efficacy and safety of risankizumab, an investigational interleukin-23 (IL-23) inhibitor, versus placebo during induction therapy in subjects with moderately to severely active Crohn’s disease. • In January 2018, AbbVie initiated two Phase 3 clinical trials to evaluate the efficacy and safety of risankizumab, an investigational interleukin-23 (IL-23) inhibitor, versus placebo during induction therapy in subjects with moderately to severely active Crohn’s disease. • In February 2018, AbbVie announced that top-line results from two Phase 3 clinical trials evaluating risankizumab with 12-week dosing compared to ustekinumab met ranked additional secondary endpoints for the treatment of patients with moderate to severe chronic plaque psoriasis.

### s0591
Context (previous sentence): This transaction resulted in the acquisition of $2.0 billion of assets, including $1.49 billion of loans and $370.6 million of investment securities, as well as $1.45 billion of deposits and $189.0 million in goodwill.
SENTENCE: The effects of the acquired assets and liabilities have been included in the consolidated financial statements since that date.

### s0592
Context (previous sentence): Non-compliance could also result in fines, damages, criminal sanctions, prohibited business conduct, and damage to our reputation.
SENTENCE: We incur additional legal compliance costs associated with our global operations and could become subject to legal penalties in foreign countries if we do not comply with local laws and regulations, which may be substantially different from those in the U.S.

### s0593
Context (previous sentence): Although inflation generally decreased in 2024 and central banks began modest reductions in interest rates, there remains uncertainty regarding, and volatility in, the inflation rate.
SENTENCE: Higher inflation levels could return, however, due to, among other things, potential tax cuts or tariffs, which could reduce the appetite for continued interest rate cuts and even necessitate interest rate increases in 2025, which could have a negative impact on our business.

### s0594
Context (previous sentence): As the sole general partner of the Operating Partnership, AMH has a fiduciary duty to the other limited partners in the Operating Partnership, which may conflict with the interests of the Company’s shareholders.
SENTENCE: The limited partners of the Operating Partnership have agreed that, in the event of a conflict in the fiduciary duties owed by AMH to the Company’s shareholders and in AMH’s capacity as the general partner of the Operating Partnership to such limited partner, AMH is under no obligation to give priority to the interests of such limited partner.

### s0595
Context (previous sentence): Our financial, accounting, data processing, backup or other operating or security systems and infrastructure may fail to operate properly or become disabled or damaged as a result of a number of factors, including events that are wholly or partially beyond our ability to control, which could adversely affect our ability to process transactions or provide services.
SENTENCE: Such events may include: sudden increases in customer transaction volume; electrical, telecommunications or other major physical infrastructure outages; natural disasters such as earthquakes, tornadoes, hurricanes and floods; disease pandemics; and events arising from local or larger scale political or social matters, including wars and terrorist acts.

### s0596
Context (previous sentence): Any such suspension or debarment or other sanction could have an adverse effect on our business and reputation.
SENTENCE: Under some of our government subcontracts, we are required to maintain secure facilities and to obtain security clearances for personnel involved in performance of the contract, which can be time-consuming and costly.

### s0597
Context (previous sentence): We have historically granted equity awards under an equity compensation plan, which includes granting performance share units and restricted stock awards or restricted stock units, to key management personnel as part of a competitive compensation package.
SENTENCE: Our ability to grant these awards has been vital to attracting, retaining and aligning shareholder interest with a talented management team in a highly competitive marketplace.

### s0598
Context (previous sentence): As of October 2, 2021, our remaining share repurchase authorization under the Program was approximately $132.0 million.
SENTENCE: Dividends On August 26, 2021, May 28, 2021, March 5, 2021 and December 10, 2020, the Board of Directors declared a quarterly dividend $0.14 per share of common stock.

### s0599
Context (previous sentence): Our stores are located in public areas where large numbers of people typically gather.
SENTENCE: Terrorist attacks, threats of terrorist attacks or civil unrest involving public areas could cause people not to visit areas where our stores are located.

### s0600
Context (previous sentence): Further, prior to COVID-19, events in Hong Kong impacted profitability of our Hong Kong operations and may continue to do so, and past hurricanes have impacted the profitability of Walt Disney World Resort in Florida and future hurricanes may also do so.
SENTENCE: The negative economic consequences of COVID-19 may be particularly challenging in markets where individuals and local businesses have limited access to government supported “safety nets”, which could lead to political instability and unrest, and further depress demand for our products and services over a longer timeframe.