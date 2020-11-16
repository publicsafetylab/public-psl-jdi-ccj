# Analysis of NYU Public Safety Lab's Jail Data Initiative for the National Commission on COVID-19 and Criminal Justice
### NYU <a href="https://publicsafetylab.org/"><b>Public Safety Lab</b></a>

In September 2020 we reported to the National Commission on COVID-19 and Criminal Justice on trends in daily individual-level jail data collected by New York University's Public Safety Lab between January 1, 2020 and July 20, 2020 (report available <a href="https://cdn.ymaws.com/counciloncj.org/resource/resmgr/covid_commission/covid-19,_jails,_and_public_.pdf">here</a>).

This repository makes publicly available the data used for an updated Impact Report released in November 2020 (daily aggregated jail data collected between January 1, 2020 and October 22, 2020).

<br>

### Features

Data appears in individual CSV files subsetted by feature types. For example, of the 325 jail facilities available in this set, different subsets report detainee age vs. detainee gender. All CSVs contain the following fields:

<ul>
  <li>date</li>
  <li>state (two-character abbreviation)</li>
  <li>county_identifier (these may not map perfectly to county names because multiple rosters may exist within the county, e.g., WA-Thurston for the Thurston Co. Sheriffs Office Corr. Fac. and WA-Thurson_Olympia for Olympia City Jail)</li>
  <li>facility_name (these may not map perfectly to the Bureau of Justice Statistics 2013 Census of Jails, e.g., when one roster contains data on detainees in multiple facilities; when this occurs, facility names are separated by semicolons)</li>
  <li>jail_id (a unique numeric identifier for each jail roster for internal use)</li>
  <li>est_pop_2019 (estimated surrounding county population from the 2019 Census)</li>
  <li>primary_fips (the county FIPS identifier associated with the primary jurisdiction of the roster</li>
  <li>bjs_juris_id (the Bureau of Justice Statistics identifier for the corresponding facility or facilities</li>
  <li>missing_date_ind (an indicator for facility-days for which data was not scraped; no gaps of 7+ days exist per facility)</li>
</ul>
