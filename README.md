# Zohran Mamdani Political Rise: Comprehensive Research Dataset (v2)

## Status and scope
This package is a substantially expanded, source-linked political analytics dataset. It includes populated historical election records, primary ranked-choice rounds, polling observations, campaign finance metrics, reported campaign-mechanism indicators, a research timeline, testable hypotheses, source register, and structured templates for future row-level data collection.

It is **not** a fully exhaustive scrape of every precinct, poll, post, ad, contribution, expenditure, endorsement, news story, or canvassing contact. Those require downloading and processing underlying source files. Blank templates are intentional and must not be mistaken for collected observations.

## Files
- `timeline.csv`: documented political and campaign milestones.
- `primary_results.csv`: candidate citywide first-choice and final-round primary totals.
- `rcv_rounds.csv`: round-level RCV counts and transfers.
- `polling_observations.csv`: a documented starter time series from Emerson releases and secondary reporting.
- `campaign_finance.csv`: candidate-specific CFB snapshot plus clearly labeled citywide/race-wide figures.
- `campaign_mechanism_indicators.csv`: reported campaign field, digital, and message-analysis metrics with caveats.
- `research_hypotheses.csv`: research questions, variables, and validity limitations.
- `message_coding_template.csv`: blank post/ad/speech coding schema.
- `geographic_election_template.csv`: blank election-district results joined to contextual measures.
- `polling_template_full.csv`: full poll-record schema.
- `sources.csv`: source register.
- `data_dictionary.csv`: field definitions and caveats.

## Key research questions
1. How did measured polling support change between early 2025 and the Democratic primary?
2. How much did ranked-choice tabulation change the primary outcome relative to first-choice voting?
3. What patterns appear between campaign message themes and polling/issue salience?
4. How did candidate-controlled campaign finance compare with independent expenditures and public matching funds?
5. Did turnout and vote shares vary geographically, and how do those patterns compare with prior elections?
6. How did online attention and field-organizing claims change around campaign milestones?

## Selected quantitative observations
- 2020 NYS Assembly Democratic primary: 8,410 votes for Mamdani; 2020 Assembly general: 38,221 votes, listed as unopposed; 2024 Assembly general: 37,911 votes, listed as unopposed (NYS Board of Elections candidate history).
- 2025 Democratic mayoral primary: 469,642 first-choice votes (43.8%); final RCV round 573,169 (56.4%) vs Andrew Cuomo 443,229 (43.6%) (NYC BOE).
- Emerson reported Mamdani at 10% in March, 23% in a May 23–26 poll, and 32% in a June poll; these are distinct poll observations, not a perfectly comparable panel.
- CFB's 2025 post-election report: $123.5m campaign spending across races, $72.2m mayoral campaign spending, $86.8m public funds distributed, and $83.2m independent spending citywide. It reports $31m in independent support for Cuomo and $21.9m in independent opposition spending against Mamdani.
- Candidate finance summary snapshot reports $17.2m total receipts and $16.5m disbursements for Mamdani's 2025 mayoral committee; values may vary as reports update.
- Campaign mechanism figures from reporting/analysis (e.g., volunteer totals, social engagement comparisons, ad-content shares) are labeled as reported claims or analyst-generated measures, not audited causal evidence.

## Primary sources and data acquisition plan
1. Election returns: NYC BOE's 2025 results summary provides citywide and election-district CSV links. Download both mayoral recap and ED-level files; preserve original files and retrieval date.
2. Earlier election history: NYS BOE candidate election history.
3. Finance: NYC CFB candidate summaries and Data Library bulk CSVs for contributions, expenditures, intermediaries, public funds, and financial analysis.
4. Polling: Emerson College Polling releases; add full field dates, sample population, mode, sample size, uncertainty, and exact question wording before doing formal trend analysis.
5. Demographics: Census ACS tables from data.census.gov; use a documented ACS vintage and official geography crosswalk.
6. Campaign content: collect publicly accessible posts/videos/ads and code a sample using a pre-registered codebook; retain post URL, date, platform, metrics capture date, and coding confidence.

## Research integrity
- Do not infer individual votes from neighborhood-level demographics.
- Do not claim causal effects from correlations or event timelines alone.
- Distinguish actual results from polls and RCV simulations.
- Distinguish campaign-controlled receipts/expenditures from independent spending.
- Report missing data explicitly; never fill blanks with invented observations.
- Retain source URLs and retrieval dates; check all time-sensitive figures against the latest official records.
