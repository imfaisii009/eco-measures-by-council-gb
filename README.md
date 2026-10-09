# ECO measures by council: Great Britain local authority data (to end of March 2026)

A clean, machine-readable copy of the official DESNZ statistics on Energy Company Obligation (ECO) home energy upgrades, covering all **350** single-tier and district councils in England, Wales and Scotland.

Between January 2013 and the end of March 2026, **4,453,004** ECO measures were installed in **2,595,218** households across Great Britain (156.7 measures per 1,000 households). The 350 council rows in this file add up exactly to those published GB totals.

Interactive table and methodology: https://applyfreeboiler.uk/data/eco-measures-by-council

## Files

| File | Rows | Contents |
|---|---|---|
| `eco_measures_by_council_gb.csv` | 350 | One row per council |
| `eco_totals_by_region_gb.csv` | 11 | Published totals for the 9 English regions, Wales and Scotland |

## Source

Department for Energy Security and Net Zero (DESNZ), *Household Energy Efficiency Statistics*, headline release June 2026, published **25 June 2026**:

- Table 3.4: ECO measures by administrative area
- Table 3.5: ECO Affordable Warmth measures installed via Flexible Eligibility, by administrative area
- Table 4.4: Households in receipt of ECO measures by administrative area

DESNZ marks each of these tables as last updated on 28 May 2026. The figures are provisional. Values were copied as published; nothing was adjusted or estimated. County and Inner/Outer London sub-totals in the source were dropped to avoid double counting. The county is kept in its own column instead.

## Column dictionary

| Column | Type | Description |
|---|---|---|
| `council` | text | Local authority name as published by DESNZ (Welsh councils include the Welsh name after " / ") |
| `area_code` | text | ONS/GSS area code (E06, E07, E08, E09, W06, S12) |
| `county_or_met_county` | text | Two-tier county, metropolitan county or Inner/Outer London that the council sits in. Blank for unitary authorities |
| `region_or_nation` | text | English region, Wales or Scotland |
| `eco_measures_jan2013_mar2026` | integer | ECO measures installed, all phases (ECO1 to ECO4), Jan 2013 to end Mar 2026 (Table 3.4) |
| `measures_per_1000_households` | decimal | DESNZ published rate per 1,000 households (2022-based household projections for mid-2025) |
| `households_helped_jan2013_mar2026` | integer | Households receiving at least one ECO measure, Jan 2013 to end Mar 2026 (Table 4.4) |
| `eco3_interim_eco4_flex_measures` | integer, may be blank | Affordable Warmth measures where the household qualified through flexible eligibility (for example a council LA Flex declaration). The ECO3 Interim / ECO4 Flex figures start in April 2022 (Table 3.5). Blank where DESNZ withheld the value |
| `flex_suppressed_flag` | text | `#` = value of 1 to 4 withheld by DESNZ; `^` = value of 5 or more withheld to protect household privacy. Blank if the value is published |

## Notes for users

- Compare councils with `measures_per_1000_households`, not raw totals, because large cities have more homes.
- One household can receive several measures (for example a boiler and loft insulation), so measures are higher than households helped.
- The measures column covers every ECO phase since 2013. DESNZ does not publish an ECO4-only total by council.

## About ECO4

ECO4 is the current phase of the Energy Company Obligation: larger energy suppliers must fund insulation and heating upgrades for low-income and vulnerable households, with Ofgem administering it on behalf of DESNZ. Households qualify through certain benefits or through their council's flexible eligibility (LA Flex) route.

## Licence and attribution

Contains public sector information licensed under the Open Government Licence v3.0.
Underlying data © Crown copyright, published by DESNZ: https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/

Questions about the statistics themselves go to DESNZ at energyefficiency.stats@energysecurity.gov.uk.

## Citation

ApplyFreeBoiler.uk, "ECO measures by council: Great Britain local authority data", https://applyfreeboiler.uk/data/eco-measures-by-council. Data: DESNZ, Household Energy Efficiency Statistics, headline release June 2026, Tables 3.4, 3.5 and 4.4, published 25 June 2026.

Maintained by [ApplyFreeBoiler.uk](https://applyfreeboiler.uk), run by Reliant Energy Solutions Ltd, an ECO4 installer based in Bury, Greater Manchester.
