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

### s0501
Context (previous sentence): Labor strikes or other labor activities, labor shortages to meet demand for Company products, including the staffing of seasonal labor needs might also disrupt our supply chain.
SENTENCE: Although precautions are taken to mitigate the impact of possible disruptions, if the Company is unable to effectively mitigate the likelihood or potential impact of such disruptive events, the Company’s results of operations and financial condition could be negatively impacted. ● Disruption to the Company’s supply chain could impair the Company’s ability to produce or deliver its finished products, resulting in a negative impact on operating results - Disruptions to the manufacturing operations or supply chain, some of which are discussed above, could result from, but are not limited to, unpredictable events such as natural disasters, pandemics, weather, fire or explosion, earthquakes, terrorism or other acts of violence.

### s0502
Context (previous sentence): While we believe we are in compliance with local laws, we cannot assure that tax and customs authorities will agree with our reporting positions and upon audit such tax and customs authorities may assess additional taxes, duties, interest, and penalties against us.
SENTENCE: Additionally, some of our products are subject to U.S. export controls, including the Export Administration Regulations and economic sanctions administered by the Office of Foreign Assets Control.

### s0503
Context (previous sentence): Certain of our products are subject to the Export Administration Regulations, administered by the BIS, which require that we obtain an export license before we can export products or technology to specified countries.
SENTENCE: Other products are subject to the International Traffic in Arms Regulations, which restrict the export of information and material that may be used for military or intelligence applications by a foreign person.

### s0504
Context (previous sentence): To the extent that any capital investment or other assistance from the PRC government is not provided to us, it could be used to promote the products and technologies of our competitors, which could adversely affect our business, operating results and financial condition. 35 Table of Contents 35 Table of Contents Changes in political and economic policies with respect to the PRC may make it diffic
SENTENCE: On November 12, 2020, then-President Trump issued an executive order, or the Order, establishing a new sanctions program designed to prohibit U.S. persons from entering into transactions in certain publicly traded securities, as well as derivatives and securities designed to provide investment exposure to such securities, of any “Communist Chinese military company,” or CCMC, as designated by the U.S.

### s0505
Context (previous sentence): Bulk drug materials are currently manufactured at our manufacturing facilities in Rensselaer, New York and Limerick, Ireland, as well as at our collaborators' facilities.
SENTENCE: We and our collaborators would be unable to manufacture these materials if the relevant facility were to cease production due to regulatory requirements or actions, business interruptions, labor shortages or disputes, contaminations, fire, natural disasters, acts of war or terrorism, or other problems.

### s0506
Context (previous sentence): We depend on multiple forms of transportation and transportation routes.
SENTENCE: Logistics can be disrupted by weather, strikes or lockouts, inadequate infrastructure or port capacity, hostilities, terrorism, or other events, and transportation costs can be volatile.

### s0507
Context (previous sentence): There can be no assurance that we will be able to obtain or maintain the required regulatory approvals in these countries.
SENTENCE: Our products are currently regulated in the European Union (EU) and the United Kingdom under the European Medical Devices Directive (93/42/EC as amended by 2007/47/EC) (MDD) and the European Medical Device Regulation (2017/745) (MDR).

### s0508
Context (previous sentence): Bitcoin is an alternative to fiat currencies that are backed by central governments, but its value is highly dependent on supply and demand.
SENTENCE: It is unclear how global geopolitical and economic crises will affect the adoption and valuation of digital assets.

### s0509
Context (previous sentence): These systems and operations are vulnerable to damage or interruption from human error, computer viruses, floods, fires, power loss, telecommunication failures and similar events.
SENTENCE: They are also subject to break-ins, sabotage, intentional acts of vandalism, terrorism and similar misconduct.

### s0510
Context (previous sentence): Such projects expose us to certain professional liability risks that are inherent in performing security inspection services for the purpose of detecting contraband items, including items that could be used in performing terrorist acts or other crimes.
SENTENCE: If a contraband item were to pass through our operations and be used to perform a terrorist act or other crime, we would be subject to risk of significant professional liability claims.

### s0511
Context (previous sentence): Despite our system of controls over our intellectual property, it may be possible for our current or future competitors to obtain, copy, use, or disclose, illegally or otherwise, our product and process technology or other proprietary information.
SENTENCE: The laws of some foreign countries may not protect our intellectual property to the same degree as do U.S. laws and our confidentiality, non-disclosure, and non-compete agreements may be unenforceable or difficult and costly to enforce.

### s0512
Context (previous sentence): These constraints impose compliance costs and risks on our operations and may negatively affect the financial or operating performance of such business activities.
SENTENCE: Our efforts to comply with U.S. and other applicable sanction and embargo laws may not be effective, and as a consequence we may face enforcement or other actions if our compliance efforts are not or are perceived as not being wholly effective.

### s0513
Context (previous sentence): Also, our current facilities in Mexico operate under the Mexican Maquiladora (IMMEX) program.
SENTENCE: This program provides for reduced tariffs and eased import regulations.

### s0514
Context (previous sentence): In the U.S. , these laws include, among others, the U.S.
SENTENCE: Export Administration Regulations (EAR), administered by the U.S.

### s0515
Context (previous sentence): Risk Factors".
SENTENCE: The United Kingdom (U.K.) formally left the European Union (E.U.) on January 31, 2020 (“Brexit”) and the transition period, during which E.U. laws continued to apply to the U.K., expired on December 31, 2020.

### s0516
Context (previous sentence): Consequently, management relies on third-party sources of capital to fund our capital needs.
SENTENCE: We may not be able to obtain financing on favorable terms or at all.

### s0517
Context (previous sentence): Application of the provisions of Section 280E to our tenants would result in the disallowance of certain tax deductions, including for depreciation or interest expense, which could have an adverse impact on their respective financial condition and ability to make lease payments to us.
SENTENCE: Any lease payment defaults by a tenant could adversely affect our results of operations and cash flows, and cause us to reduce the amount of distributions to our stockholders. ● unexpected changes in regulatory requirements and other laws; ● unexpected changes in regulatory requirements and other laws; ● the impact of national, regional or state specific business cycles and economic instability; and ● the impact of national, regional or state specific business cycles and economic instability; and ● potentially adverse tax consequences. ● potentially adverse tax consequences.

### s0518
Context (previous sentence): We cannot assure you that we will be able to protect the Company against such fluctuations in the future.
SENTENCE: Further, we cannot assure you that the countries in which we currently operate will not adopt policies limiting repatriation of earnings in the future.

### s0519
Context (previous sentence): We strive to have a “zero-defect” quality culture focused on meeting or exceeding demanding high-temperature automotive quality standards.
SENTENCE: We strive to comply with industry standards such as IATF 16949:2016 (the automotive sector-specific quality management system standard) and ISO 14001 (a voluntary standard for environmental management published by the International Standards Organization), and we also strive to comply with ISO 26262 ASIL product development standards, RoHS (an EU standard relating to use of certain hazardous substances in products) and similar environmental product requirements.

### s0520
Context (previous sentence): The imposition of tariffs, duties, border adjustment taxes or other trade restrictions by the United States could also result in the adoption of new or increased tariffs or other trade restrictions by other countries.
SENTENCE: Tariffs may in the future increase our cost of materials and may cause us to increase prices to our customers which we believe may reduce demand for our products.

### s0521
Context (previous sentence): If the U.S.
SENTENCE: Government is uncertain about whether such items were not subject to U.S. export controls, it could conduct an investigation and, if it is determined that some of the items were subject to U.S. export control jurisdiction, result in costs, fines or penalties that could have a material impact on our business.

### s0522
Context (previous sentence): The effect of the regulations could be detrimental to our financial condition.
SENTENCE: In addition, we and our sponsor financial institutions are subject to the laws and regulations enforced by the Office of Foreign Assets Control, which prohibit U.S. persons from engaging in transactions with certain prohibited persons or entities.

### s0523
Context (previous sentence): Failure to comply with these laws could harm our business by subjecting us to sanctions by the U.S. government, including substantial monetary penalties, denial of export privileges and debarment from U.S. government contracts.
SENTENCE: For example, from 2016 through 2020, one of our foreign subsidiaries engaged in certain transactions, a limited number of which included U.S. origin goods, either directly or indirectly through distributors, involving sales to specially designated nationals and/or to the Crimea region of Ukraine, which may have been made in violation of relevant trade sanctions or export control laws.

### s0524
Context (previous sentence): If we or our customers fail to comply with such laws and regulations, we could incur liabilities and fines and our operations could be suspended.
SENTENCE: In addition, as climate change concerns become more prevalent, the U.S. and foreign governments have sought to limit the effects of any such changes.

### s0525
Context (previous sentence): Several states have sought to assert jurisdiction over educational institutions offering online degree programs that have no physical location in the state but that have some 42 Table of Contents severally liable to ED, along with the relevant client, for return of those funds.
SENTENCE: Further, we could be fined or otherwise sanctioned by ED, which could increase our cost of regulatory compliance and materially adversely affect us.

### s0526
Context (previous sentence): Weak economic conditions, such as high unemployment, low labor force participation, lower family income, a weak real estate market, lower business investment and lower consumer spending may adversely affect the demand for insurance and financial products and lower the Company’s profitability in some cases.
SENTENCE: In addition, political instability, politically motivated violence or civil unrest, may increase the frequency and severity of insured losses.

### s0527
Context (previous sentence): We may experience increased costs for, or significant impact to, our Chinese operations in the event of changes in Chinese government policies or political unrest or unstable economic conditions in China.
SENTENCE: The nationalization or other expropriation of private enterprises by the Chinese government could result in total loss of our China investment.

### s0528
Context (previous sentence): We sell our products to distributors, end-users, installers, and directly to OEMs.
SENTENCE: We have manufacturing and other operating facilities in the U.S., Canada, China, India, Mexico, Tunisia, and various countries in Europe.

### s0529
Context (previous sentence): Our ability to manage inventory and meet delivery requirements may be constrained by our suppliers’ inability to scale production and adjust delivery of long-lead time products during times of volatile demand.
SENTENCE: In addition, current or future global economic uncertainty, including inflation and high interest rates, supply chain and labor disruptions, tariffs and other trade barriers and restrictions, unemployment rates, banking instability, any U.S. government shutdown, any downgrades in the U.S. government's sovereign credit rating, public health crises, volatile financial markets, geopolitical instability and regional conflicts, and potential recession may affect the financial stability of our key suppliers or their access to financing, which may in turn affect their ability to perform their obligations to us.

### s0530
Context (previous sentence): However, to the extent we are unable to finance our operating expenditures, capital expenditures, scheduled interest and debt repayments and any future dividends with net cash provided by operating activities and borrowings under the Credit Facility, we may require additional capital.
SENTENCE: Periods of instability in the capital and credit markets (both generally and in the oil and gas industry in particular) could limit our ability to access these markets to raise debt or equity capital on affordable terms or to obtain additional financing.

### s0531
Context (previous sentence): We have done and may continue to do business in countries subject to U.S. sanctions and embargoes, and we may have limited managerial oversight over those activities.
SENTENCE: Failure to comply with various sanction and embargo laws may result in enforcement or other regulatory actions.

### s0532
Context (previous sentence): We work on an ongoing basis to identify customer trends and preferences, and to obtain merchandise inventory to meet anticipated customer needs.
SENTENCE: It is very challenging to successfully do this well and consistently across our diverse merchandise categories and in the multiple markets in which we operate throughout the United States and its territories.

### s0533
Context (previous sentence): Customers may also not deploy a security release, or decide not to upgrade to the latest versions of our products, services or cloud-based solutions containing the release, leaving them vulnerable.
SENTENCE: Vulnerabilities and critical security defects, prioritization errors in remedying vulnerabilities or security defects, failure of third-party providers to remedy vulnerabilities or security defects, or customers not deploying security releases or deciding not to upgrade products, services or solutions could result in claims of liability against us, damage our reputation or otherwise harm our business.

### s0534
Context (previous sentence): Domestic or international natural disasters or terrorist attacks may disrupt our operations, decrease the demand for our products or otherwise have an adverse impact on our business.
SENTENCE: Chemical related assets, and U.S. corporations such as us, may be at greater risk of future terrorist attacks than other possible targets in the U.S., the United Kingdom and throughout the world.

### s0535
Context (previous sentence): NEM is a tariffed utility rate program that permits a consumer to sell the excess solar energy that the consumer’s solar panels produce to the electric utility company at a predetermined price.
SENTENCE: The most basic type of NEM tariff pays consumers the retail rate for electricity that their solar panels export to the grid, less certain “non-bypassable” fees paid by the consumer.

### s0536
Context (previous sentence): As has been widely reported, we are currently operating in a period of macroeconomic uncertainty and capital markets disruption, which has been significantly impacted by domestic and global monetary and fiscal policy, trade regulations, including changes in trade policies, tariffs or other trade restrictions or the threat of such actions, 46 Table of Contents geopolitical instability, including on
SENTENCE: In particular, the conflict in Ukraine has exacerbated market disruptions, including significant volatility in commodity prices, as well as supply chain interruptions, and has contributed to record inflation globally.

### s0537
Context (previous sentence): These conditions could ultimately dampen demand for our goods and services by increasing the possibility of a recession.
SENTENCE: In addition, the conflict could lead to increased cyberattacks or could aggravate other risk factors that we identify in our public filings.

### s0538
Context (previous sentence): These conditions, as well as any further delays, devaluations or imposition of more stringent repatriation restrictions, may materially adversely affect our business, results of operations and financial condition.
SENTENCE: We may be adversely affected by conflicts overseas or terrorist attacks; the travel industry continues to face ongoing security concerns.

### s0539
Context (previous sentence): Since March 2025, President Trump has announced new tariffs on foreign imported goods from countries worldwide, including additional tariffs on substantially all products imported from China.
SENTENCE: Some of these tariffs have been paused or reduced, but we cannot predict whether any of these reductions will remain in place or pauses will lapse or be extended, or whether any tariffs will be increased or decreased.

### s0540
Context (previous sentence): Accordingly, if our effective tax rate were to increase, it may have a material adverse effect on our business, financial condition and results of operations.
SENTENCE: Finally, because we have substantial operations in a number of locations worldwide, tax authorities in various jurisdictions may raise questions concerning matters such as transfer pricing, whether revenues or expenses should be attributed to particular countries, the presence or absence of permanent establishments in particular countries and similar matters.

### s0541
Context (previous sentence): If the Company were to incur a significant liability for which its as not fully insured or that its insurers disputed, the Company’s business, financial condition or results of operations could be materially adversely affected.
SENTENCE: Future terror attacks, war, natural disasters or other catastrophic events or public health crises beyond the Company's control could negatively impact the Company's business, results of operations, and cash flows.

### s0542
Context (previous sentence): Bribery Act 2010; • compliance with U.S. laws and regulations pertaining to the sale and distribution of products to customers in foreign countries, including anti-corruption laws such as the Foreign Corrupt Practices Act and the U.K.
SENTENCE: Bribery Act 2010; • difficulty in conducting due diligence with respect to business partners in certain international markets; • difficulty in conducting due diligence with respect to business partners in certain international markets; • political and economic turbulence or uncertainty; • political and economic turbulence or uncertainty; • terrorism, war or other armed conflict; and • terrorism, war or other armed conflict; and • natural disasters, epidemics, and pandemics. • natural disasters, epidemics, and pandemics.

### s0543
Context (previous sentence): In fiscal 2018, Astute was acquired by a third party and we realized a $16.2 million loss on our investment.
SENTENCE: Significant developments or uncertainties stemming from the U.S. administration or resulting in potential changes resulting from the elections in the U.S. this fall, including changes in U.S. trade policies, tariffs, healthcare, taxes or other matters and the reaction of other countries thereto, could have an adverse effect on our business.

### s0544
Context (previous sentence): On the fourth business day of each month, factors drop and lower the market value of our Agency Securities.
SENTENCE: This reflects both scheduled and unscheduled principal paydowns, which are guaranteed by GSEs.

### s0545
Context (previous sentence): Artificial Intelligence is an emerging area of technology that has the potential to impact various aspects of our business operations and customer interactions.
SENTENCE: AI, including Generative AI and Post-Quantum Cryptography, has the potential to change the way we operate by creating efficiencies and improving processes and customer experiences.

### s0546
Context (previous sentence): We are from time to time subject to audits and investigations relating to our government contracts, and any violations could result in various civil and criminal penalties and administrative sanctions, including termination of contracts, refunding or suspending of payments, forfeiture of profits, payment of fines and suspension or debarment from future government business.
SENTENCE: In addition, such contracts may provide for termination by the government at any time, without cause.

### s0547
Context (previous sentence): We maintain policies designed to comply with anti-money laundering and sanctions laws and acquire bitcoin only from regulated entities.
SENTENCE: However, if we are found to have unknowingly purchased bitcoin from bad actors or sanctioned individuals, we could face regulatory proceedings, and our ability to engage in future bitcoin transactions may be restricted or prohibited.

### s0548
Context (previous sentence): This additional regulation of encryption technology could delay or prevent the acceptance and use of encryption products and public networks for secure communications, resulting in decreased demand for our products and services.
SENTENCE: In addition, some foreign competitors are subject to less stringent controls on exporting their encryption technologies.

### s0549
Context (previous sentence): Our international research and development teams play a critical role in these efforts.
SENTENCE: We must attract, train, motivate and retain our international research and development team members.

### s0550
Context (previous sentence): If we fail to comply with the requirements of the ADA, we could be subject to fines, penalties, injunctive action, reputational harm and other business effects which could materially and negatively affect our performance and results of operations.
SENTENCE: Terrorist attacks, military conflicts and the availability of terrorism insurance may adversely affect the lodging industry.