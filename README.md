# Building a Data Center: Intel Energy Site Analysis

Where should Intel build its next data center? This project answers that question with U.S. regional energy data. It compares how much power each region produces, how much of it comes from renewable sources, and how steady that supply stays hour to hour.

**[View the live dashboard](file:///Users/rosarylamb/Downloads/IntelDataCenterProject%20(1).html)**

## The recommendation

**The Northwest.** It produces about 22 million MWh more energy than it uses, the second-largest surplus in the country. It also leads the nation with roughly 52% of its power coming from renewable sources. Most of that is hydropower, which runs steadily around the clock instead of rising and falling with the sun or wind. A data center needs reliable, clean power 24/7, and the Northwest delivers both.

## What's in the project

**Tableau dashboard** ([Tableau Public link](YOUR-TABLEAU-PUBLIC-LINK))

- Net production by region (NetProduction calculated field)
- Supply vs. demand dual-axis chart with a Day / Week / Month parameter (SelectPeriod and DATETRUNC)
- Renewable energy share by region (RenewableEnergy and RenewablePercentage calculated fields)
- Treemap of energy sources by region and balancing authority
- Hourly percent difference in generation
- Energy source by region over time
- Renewable energy by hour of day, comparing California and the Northwest

**Interactive web dashboard** (`index.html`)

- Click any region on the hex map or ranking chart and every card updates
- Toggles for surplus vs. renewable views, Day / Week / Month periods, and sorting the power mix
- Legend buttons that show or hide each line
- A Site Fit Score that checks three criteria: net producer, top 5 in renewables, and steady supply around the clock
- A "My Notes" panel with my findings for each question
- Light and dark mode, plus a phone layout

## About the data

The project uses two datasets of hourly U.S. grid data from 2022: `energy_dataset` and `energy_data_by_source`. Both include demand, net generation and output by source (wind, solar, hydro, natural gas, coal, nuclear, petroleum and other) for 13 regions.

The web dashboard opens with demo data. The net production and renewable percentages come from my Tableau results. The power mix, monthly trends and hourly curves are sample values. To see the real numbers, click **Load energy_dataset.csv** and choose the file. It's processed in your browser and never uploaded.

## Tools

Tableau · HTML · CSS · JavaScript · D3.js · PapaParse

## Key findings

1. Five regions are net producers. Mid-Atlantic has the largest surplus at about 31M MWh, and the Northwest is second at about 22M.
2. Mid-Atlantic's biggest monthly surplus came in July 2022.
3. The Northwest, Central and California lead in renewable share, helped by river systems, a wind corridor and year-round sunshine.
4. Only the Northwest and Central are both net producers and top 5 in renewables.
5. California's wind generation picks up from about 10 AM to 10 PM and grows fastest around 3 PM.
6. California's renewable output spikes at midday and drops at night, while the Northwest's stays nearly flat.

## Author

Stephanie Ceja · B.B.A. in Information Systems, The University of Texas Rio Grande Valley
