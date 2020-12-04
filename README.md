# COVID-19, Jails, and Public Safety: A Report to the National Commission on COVID-19 and Criminal Justice
### Report Summary 

In September 2020 New York University's <a href="https://publicsafetylab.org/"><b>Public Safety Lab</b></a> reported to the National Commission on COVID-19 and Criminal Justice on trends in daily individual-level jail data being collected by its <a href="https://publicsafetylab.org/jail-data-initiative"><b>Jail Data Initiative</b></a>. The report, which analyzed a sample of over 14 million daily individual-level jail records collected between January 1, 2020 and July 20, 2020, is available <a href="https://cdn.ymaws.com/counciloncj.org/resource/resmgr/covid_commission/covid-19,_jails,_and_public_.pdf">here</a>.

This repository makes publicly available the data used for an updated report released in December 2020, which drew upon a sample of approximately 19 million daily individual-level daily jail records collected between January 1, 2020 and October 22, 2020. The data in this repository are aggregated to the roster/day level.

### Features

Data appears in individual CSV files subsetted by feature types. All CSVs contain the following fields:

<ul>
  <li>date</li>
  <li>state (two-character abbreviation)</li>
  <li>county_identifier (more precisely, state_county_roster_identifier; multiple jail rosters that exist within a single county are reported as e.g., WA-Thurston for the Thurston County Sheriff's Office Correctional Facility and WA-Thurston_Olympia for the Olympia City Jail)</li>
  <li>facility_name (multiple facilities may be reported by a single jail roster; when this occurs, facility names are separated by semicolons)</li>
  <li>jail_id (a unique numeric identifier for each jail roster for internal use)</li>
  <li>est_pop_2019 (estimated county population from the 2019 American Community Survey)</li>
  <li>primary_fips (the county FIPS identifier associated with the primary jurisdiction of the roster)</li>
  <li>bjs_juris_id (the Bureau of Justice Statistics identifier for the corresponding facility or facilities)</li>
  <li>missing_date_ind (an indicator for roster/days for which data were not scraped; no data are reported for rosters with gaps of 7+ days in data collection)</li>
</ul>

Additional notes:

<ul>
  <li>missing values are different from zero counts (e.g., if a roster does not report a feature, that feature will report null values; if a roster reports a feature, but there are no records of that feature for a given date, the feature will report zero counts)</li>
  <li>"traffic" in a CSV title refers to the presence of counts grouped by bookings and releases, in addition to total daily counts per roster/day</li>
  <li>"recidivism" in a CSV title refers to the presence of data on rebooking by group, in addition to total daily counts by group per roster/day</li>
  <li>charge class refers to classification as felony, misdemeanor, or other</li>
  <li>charge type refers to specific subsets of charges (e.g., failure to appear, cannabis posession, etc.)</li>
  </ul>
  
 ### Contact Information

Please contact us at publicsafetylab@nyu.edu with questions or comments.

