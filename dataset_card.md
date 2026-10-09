---
license: other
license_name: ogl-3.0
license_link: https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/
language:
- en
pretty_name: ECO measures by council (Great Britain, to March 2026)
size_categories:
- n<1K
tags:
- energy-efficiency
- energy-company-obligation
- eco4
- uk
- local-government
- open-government-data
- tabular
configs:
- config_name: councils
  data_files: eco_measures_by_council_gb.csv
- config_name: regions
  data_files: eco_totals_by_region_gb.csv
---

# ECO measures by council (Great Britain)

Official DESNZ figures on Energy Company Obligation (ECO) home energy upgrades for all 350 councils in England, Wales and Scotland, January 2013 to end of March 2026: measures installed, households helped, measures per 1,000 households, and ECO3 Interim / ECO4 Flex (LA Flex) measures.

- **Rows:** 350 councils (`councils`) and 11 region/nation totals (`regions`)
- **GB totals:** 4,453,004 measures in 2,595,218 households (156.7 per 1,000 households)
- **Source:** DESNZ, Household Energy Efficiency Statistics, headline release June 2026, Tables 3.4, 3.5 and 4.4, published 25 June 2026. Figures are provisional.
- **Licence:** Open Government Licence v3.0 (OGL-3.0). Contains public sector information licensed under the Open Government Licence v3.0.

See README.md for the column dictionary and caveats. Suppressed flex values (`#` = 1 to 4, `^` = 5 or more) are blank in the numeric column and flagged in `flex_suppressed_flag`.

Interactive table and methodology: https://applyfreeboiler.uk/data/eco-measures-by-council

Maintained by ApplyFreeBoiler.uk.
