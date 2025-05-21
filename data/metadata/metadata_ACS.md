
- `Title`: American Community Survey (ACS) five-year estimate (2014-2018)
- `Abstract`: Demographic breakdown of disabled population
- `Spatial Coverage`: USA
- `Spatial Resolution`: County
- `Spatial Representation Type`: vector multipolygon 
- `Spatial Reference System`: EPSG 4269
- `Temporal Coverage`: 2014-2018
- `Temporal Resolution`: 5-year estimate
- `Lineage`: Retrieved values from Census website tables S1810 and C18130 tables using tidyCensus
- `Distribution`: Publicly available
- `Constraints`: Public Data

The American Community Survey (ACS) five-year estimate (2014-2018) variables used in the study are outlined in the table below.
Details on ACS data collection can be found at <https://www.census.gov/topics/health/disability/guidance/data-collection-acs.html> and details on sampling methods and accuracy can be found at <https://www.census.gov/programs-surveys/acs/technical-documentation/code-lists.html>.

|                            Variable Name in Study                            |                                               ACS Variable name                                                |
|:----------------------------------:|:----------------------------------:|
| percent of total civilian non-institutionalized population with a disability |                                                 S1810_C03_001E                                                 |
|                                   **Race**                                   |                                                                                                                |
|                      percent w disability: White alone                       |                                                 S1810_C03_004E                                                 |
|                      percent w disability: Black alone                       |                                                 S1810_C03_005E                                                 |
|                    percent w disability: Native American                     |                                                 S1810_C03_006E                                                 |
|                      percent w disability: Asian alone                       |                                                 S1810_C03_007E                                                 |
|                       percent w disability: Other race                       |                                                 S1810_C03_009E                                                 |
|                                **Ethnicity**                                 |                                                                                                                |
|                   percent w disability: Non-Hispanic White                   |                                                S1810_C03_0011E                                                 |
|                        percent w disability: Hispanic                        |                                                 S1810_C03_012E                                                 |
|                 percent w disability: Non-Hispanic non-White                 | (S1810_C02_001E - S1810_C02_011E - S1810_C02_012E) / (S1810_C01_001E - S1810_C01_011E - S1810_C01_012E) \* 100 |
|                       percent w disability: Other race                       |                                                 S1810_C03_009E                                                 |
|                                 **Poverty**                                  |                                                                                                                |
|                  percent w disability: Below poverty level                   |                         (C18130_004E + C18130_011E + C18130_018E) / C18130_001E \* 100                         |
|                  percent w disability: Above poverty level                   |                         (C18130_005E + C18130_012E + C18130_019E) / C18130_001E \* 100                         |
|                                   **Age**                                    |                                                                                                                |
|                          percent w disability: 5-17                          |                                                 S1810_C03_014E                                                 |
|                         percent w disability: 18-34                          |                                                 S1810_C03_015E                                                 |
|                         percent w disability: 35-64                          |                                                 S1810_C03_016E                                                 |
|                         percent w disability: 65-74                          |                                                 S1810_C03_017E                                                 |
|                          percent w disability: 75+                           |                                                 S1810_C03_018E                                                 |
|                              **Biological sex**                              |                                                                                                                |
|                          percent w disability: male                          |                                                 S1810_C03_001E                                                 |
|                         percent w disability: female                         |                                                 S1810_C03_003E                                                 |

: Disability Subgroup Variables

American Community Survey (ACS) data for sociodemographic subcategories of people with disabilities can be accessed by using the `tidycensus` package to query the Census API. This requires an API key which can be acquired at [api.census.gov/data/key_signup.html](https://api.census.gov/data/key_signup.html).