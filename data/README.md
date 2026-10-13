# Leader age dataset: data note

`leaders-age-data.csv` has one row per country (143 rows), as of **11 October 2026**. All 143 are used in the charts and figures (`included_in_analysis` = 1), but Palestine is left out of the political-regime views (see below). Ages and years in office are calculated to the as-of date and rise a little each day.

## Columns
| Column | Meaning |
|---|---|
| `country`, `region`, `g20` | Country; continent (Russia counted in Europe, Turkey in Asia; North America includes Central America and the Caribbean); 1 if one of the 19 G20 member countries. |
| `leader`, `birth_date` | The leader (see "Who counts as the leader") and their birth date. |
| `leader_age_years` | Age in years on the as-of date. |
| `first_start_date`, `terms`, `number_of_terms` | Dates of each stint in office. Years as prime minister count towards time in office, so Putin (president 1999-2008, prime minister 2008-2012, president since) and Erdogan (prime minister 2003-2014, then president) are each one continuous stretch. |
| `years_in_office_total` | Years in office, adding up all stints. |
| `vdem_regime_2025` | V-Dem Regimes of the World classification for 2025 (blank for Brunei, the Bahamas and Dominica, which V-Dem does not classify, and for Palestine, which V-Dem scores separately for the West Bank and Gaza). |
| `population_median_age_2026` | Median age of the population, UN World Population Prospects 2024 (2026 estimate), via Our World in Data. |
| `age_gap_years` | `leader_age_years` minus `population_median_age_2026`. |
| `population_2023` | Population, UN World Population Prospects 2024 (2023 estimate), via Our World in Data. Used for population-weighted figures. |
| `pew_leader_june_2026`, `pew_age_on_2026_06_14`, `our_age_on_2026_06_14`, `pew_comparison` | Cross-check against Pew Research Center's June 2026 table of 186 leaders (ages as of 14 June 2026). |
| `included_in_analysis` | 1 if used in the charts and figures (all rows). |
| `coding_note` | Judgement calls for individual countries. |

## Who counts as the leader
The person who holds the main executive power: the prime minister in parliamentary systems and in semi-presidential ones where the government is led by the prime minister (for example Portugal, Poland, Moldova, Romania, Lebanon); the president in presidential systems and in semi-presidential ones where the president dominates (for example France); the monarch in Gulf and other executive monarchies. Xi and To Lam are counted from taking the top party post, and coup leaders from the coup. Acting or interim leaders are included.

Judgement calls that differ from Pew Research Center: Saudi Arabia (we count Crown Prince Mohammed bin Salman, Pew counts King Salman), Timor-Leste (prime minister Gusmao, Pew counts the president) and Nicaragua (Daniel Ortega, Pew counts co-president Rosario Murillo). For Moldova, the UK and Peru, Pew's June table pre-dates a change of leader.

## Which countries are covered
The charts cover UN member states for which the leader's birth date could be established reliably, plus **Palestine**, a UN observer state (Mahmoud Abbas, born 1935-11-15). Footnote used on the charts: *Mahmoud Abbas is president of the State of Palestine, but the Palestinian Authority's governing authority is largely limited to parts of the West Bank.* Pew's table omits Palestine. V-Dem scores the West Bank and Gaza separately, so Palestine has no regime value and is left out of the regime views; the median age and population cover the whole territory. He is Asia's oldest leader (90.9) with its widest age gap (+70.6 years). Taiwan, Kosovo and the Holy See are not included.

**Contested control.** Where the recognised government does not control all of its territory (for example Sudan, Somalia, Syria, Ukraine, Myanmar, Burkina Faso, DR Congo, Ethiopia and South Sudan), the country is included and counted under the recognised government's leader, with a note in `coding_note`.

**Not included.** North Korea, Oman and Guinea (sources disagree on the birth year), Afghanistan, Benin, Botswana, Bulgaria, Burundi, Cape Verde, Colombia, Georgia, Grenada, Guinea-Bissau, Haiti, Iraq, Latvia, Lesotho, Libya, Lithuania, Madagascar, Mali, Mongolia, Niger, North Macedonia, Serbia, Seychelles, Suriname, Switzerland, Uruguay, Yemen, and most Pacific and Caribbean microstates. The 143 countries cover 94.5% of the world's population (2023).

## Sources
Wikipedia and Wikidata (birth dates, terms of office); UN World Population Prospects 2024 via Our World in Data (median age, population); V-Dem Democracy Report v16 (March 2026), Regimes of the World, 2025, via Our World in Data. Every birth date was checked against both Wikipedia and Wikidata and, since June, against Pew's table.

## Pew cross-check
133 countries match Pew's table exactly (same leader, birth date within about four days). One more is the same leader with a birth date about 16 days different (Ireland), one has a different birth year (Bangladesh: ours 1968 from the national ID, Pew 1965), six are different people (three definitional, three timing), and two are not in Pew's table (Palestine, Somalia).

## Figures recomputed from the 143 included rows (as of 11 October 2026)
| Figure | Value |
|---|---|
| Median leader age | 64.3 |
| Leaders aged 65 or older | 68 of 143 (47.6%); aged 70 or older 32.2% |
| People living under a leader aged 65 or older | 76.0% of people in these 143 countries; at least 71.8% of the world even if every excluded country's leader were younger. For 70 or older: 67.2% and 63.4%. |
| G20 (19 countries) | over 80: United States, Brazil; aged 70-79: 7; under 50: France, Italy, Saudi Arabia |
| Median leader age by region | Africa 69.5, Asia 67.3, North America 65.4, Oceania 59.9, Europe 56.8, South America 56.0 |
| Median age gap (leader minus population median) | 32.4 years |
| Leaders younger than their population's median age | Montenegro (-1.37), Netherlands (-1.97) |
| African countries classed as autocracies | 31 of 41 (24 electoral, 7 closed); 8 of Africa's 10 oldest leaders |
| Longest-serving leader in a liberal democracy | France, 9.4 years (none of the 25 has 10 or more) |
| Median years in office by regime | liberal democracy 3.3; electoral democracy 4.0; electoral autocracy 7.6; closed autocracy 8.8 |
| Share in office 10 or more years | 0%, 16%, 39%, 48% (same order) |
| Putin and Erdogan, years in office | 26.8 and 23.6 |
