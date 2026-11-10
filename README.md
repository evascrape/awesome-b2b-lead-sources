# Awesome B2B Lead Sources

A curated list of **public and free sources of business data** for building B2B prospect lists: official business registries, government statistics, licence and regulator lookups, open datasets, and the rules that apply when you email the people you find.

Most "lead list" articles only list paid contact databases. Many good lists start one step earlier, from an official register or a public statistic that tells you how many companies exist and where. This list collects those sources. Every link was opened and checked when it was added (November 2026).

Contributions are welcome: open a pull request with one source per line, a link to the official page, and one sentence on what it contains.

## Contents

- [Market size: how many businesses exist](#market-size-how-many-businesses-exist)
- [US company and filing registries](#us-company-and-filing-registries)
- [US industry and licence lookups](#us-industry-and-licence-lookups)
- [Company registries outside the US](#company-registries-outside-the-us)
- [Open datasets](#open-datasets)
- [Contact data tools](#contact-data-tools)
- [Rules for emailing B2B contacts](#rules-for-emailing-b2b-contacts)

## Market size: how many businesses exist

- [County Business Patterns (US Census Bureau)](https://www.census.gov/programs-surveys/cbp.html) - Number of establishments, employees and payroll by industry (NAICS) for the US, every state and every county, with employee size classes. Bulk files need no API key.
- [Statistics of US Businesses (US Census Bureau)](https://www.census.gov/programs-surveys/susb.html) - Counts of firms (not just locations) by industry and enterprise size.
- [Nonemployer Statistics (US Census Bureau)](https://www.census.gov/programs-surveys/nonemployer-statistics.html) - Businesses with no paid employees, which County Business Patterns leaves out (sole proprietors, freelancers).
- [Occupational Employment and Wage Statistics (US BLS)](https://www.bls.gov/oes/tables.htm) - How many people work in each occupation (for example marketing managers or purchasing managers), their pay, and which industries and states employ them.
- [Quarterly Census of Employment and Wages (US BLS)](https://www.bls.gov/cew/) - Establishment and employment counts by industry and county, updated quarterly.
- [US business counts by industry, state and job title](https://github.com/evascrape/us-business-counts) - CSV extracts of the two Census and BLS sources above for 20 common B2B industries and 15 buyer roles, with the script that builds them.

## US company and filing registries

- [SEC EDGAR full-text search](https://www.sec.gov/edgar/search/) - Filings of public companies and many private funds; filings name officers and directors.
- [SEC EDGAR APIs](https://www.sec.gov/search-filings/edgar-application-programming-interfaces) - JSON APIs for company submissions and financial data. The SEC asks automated clients to declare a contact address in the User-Agent.
- [SAM.gov data services](https://sam.gov/data-services) - Entity registrations of companies that sell to the US federal government, including their business types and NAICS codes.
- [USAspending.gov](https://www.usaspending.gov/) - Federal contract and grant awards by recipient, useful for finding government contractors in a given industry.
- [California bizfile Online](https://bizfileonline.sos.ca.gov/search/business) - California Secretary of State business entity search.
- [Delaware Division of Corporations entity search](https://icis.corp.delaware.gov/ecorp/entitysearch/namesearch.aspx) - Entity status lookup for the state where many US companies incorporate.

## US industry and licence lookups

- [NPI Registry (CMS)](https://npiregistry.cms.hhs.gov/) - Every US healthcare provider and organisation with a National Provider Identifier, with practice address and specialty. [Full NPPES download files](https://download.cms.gov/nppes/NPI_Files.html) are also published.
- [FDIC BankFind Suite](https://banks.data.fdic.gov/bankfind-suite/bankfind) - FDIC-insured banks and their branches.
- [FINRA BrokerCheck](https://brokercheck.finra.org/) - Registered brokerage firms and individual brokers.
- [SEC Investment Adviser Public Disclosure](https://adviserinfo.sec.gov/) - Registered investment adviser firms and representatives.
- [Texas Department of Licensing and Regulation licence search](https://www.tdlr.texas.gov/LicenseSearch/) - An example of a state licence lookup (electricians, HVAC contractors and other licensed trades). Most states run a similar search for regulated trades.

## Company registries outside the US

- [Companies House search (UK)](https://find-and-update.company-information.service.gov.uk/) and the [Companies House API](https://developer.company-information.service.gov.uk/) - UK companies, officers and filing history, free with an API key.
- [OpenCorporates](https://opencorporates.com/) - A single search across company registers from many jurisdictions.
- [GLEIF LEI search](https://search.gleif.org/) and the [LEI Golden Copy download](https://www.gleif.org/en/lei-data/gleif-golden-copy/download-the-golden-copy) - Legal entities with a Legal Entity Identifier, including parent and child relationships.
- [Federal corporation search (Canada)](https://ised-isde.canada.ca/cc/lgcy/fdrlCrpSrch.html) - Corporations incorporated under Canadian federal law.
- [ABN Lookup (Australia)](https://abr.business.gov.au/) - Australian Business Numbers, entity names and locations.
- [Brønnøysund Register Centre (Norway)](https://data.brreg.no/enhetsregisteret/oppslag/enheter) - Norwegian legal entities with an open API.
- [API Recherche d'entreprises (France)](https://www.data.gouv.fr/dataservices/api-recherche-dentreprises) - Free API over the French SIRENE company register.
- [KVK search (Netherlands)](https://www.kvk.nl/zoeken/) - Dutch Chamber of Commerce register.
- [e-Business Register (Estonia)](https://ariregister.rik.ee/eng) - Estonian companies and their representatives.
- [Bizfile (Singapore)](https://www.bizfile.gov.sg/) - Singapore ACRA business register.

## Open datasets

- [Wikidata Query Service](https://query.wikidata.org/) - SPARQL queries over companies with industry, headquarters, founding date and website.
- [Overture Maps](https://overturemaps.org/) - Open places dataset that includes businesses with categories and locations.
- [Overpass Turbo](https://overpass-turbo.eu/) - Query OpenStreetMap for businesses of a given type in an area.
- [Common Crawl](https://commoncrawl.org/) - Open web crawl archive, the raw material for building your own company website index.
- [Hacker News "Who is hiring?" threads](https://news.ycombinator.com/submitted?id=whoishiring) - Monthly threads of companies that are hiring, a signal of budget and growth.
- [Datacircle](https://datacircle.dev) - Find the best GTM APIs. We benchmark all the GTM APIs and we put the results on our website. The [open API](https://api.datacircle.dev/v1) needs no key.

## Contact data tools

Tools that return named contacts (name, title, work email, phone) for a filter. Listed alphabetically; check each vendor's current pricing and data-source terms yourself.

- [Apollo.io](https://www.apollo.io/) - Sales intelligence platform with a contact database and sequencing.
- [Evascrape](https://evascrape.com/) - Builds lead lists from LinkedIn-style filters, Apollo.io search URLs or Google Maps searches and delivers a CSV; prepaid, priced per delivered record ([pricing](https://evascrape.com/pricing), [data sources](https://evascrape.com/compliance)). Also available as an [Apify actor](https://apify.com/evascrape/b2b-leads-finder) and an [MCP server](https://github.com/evascrape/evascrape-mcp). *Maintained by the authors of this list.*
- [Hunter](https://hunter.io/) - Finds and verifies email addresses by company domain.
- [Lusha](https://www.lusha.com/) - Contact and company data with a browser extension.
- [RocketReach](https://rocketreach.co/) - Contact lookup by name, company or title.
- [Snov.io](https://snov.io/) - Email finder, verifier and outreach tool.
- [ZoomInfo](https://www.zoominfo.com/) - Enterprise B2B contact and company database.

## Rules for emailing B2B contacts

- [CAN-SPAM Act, 15 U.S.C. chapter 103](https://www.law.cornell.edu/uscode/text/15/chapter-103) and the [FTC CAN-SPAM rule, 16 CFR part 316](https://www.ecfr.gov/current/title-16/chapter-I/subchapter-C/part-316) - US rules for commercial email: accurate headers, a physical address, and a working opt-out.
- [GDPR Article 14](https://gdpr-info.eu/art-14-gdpr/) - What you must tell people in the EU when you collect their personal data from a source other than them.

## License

[CC0 1.0](LICENSE). The data in the linked sources belongs to their publishers and is subject to their terms.
