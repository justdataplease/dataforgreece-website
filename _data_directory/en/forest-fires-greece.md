---
title: Forest Fires in Greece
slug: forest-fires-greece
description: Forest Fires in Greece
category: Environment
date: 2024-10-14
download_url: https://github.com/justdataplease/dataforgreece/raw/refs/heads/main/data/fires-greece/forest-fires-combined-greece_2023.csv.zip
---

| **Published by**     | Hellenic Fire Service                                 |
|----------------------|------------------------------------------------------|
| **Last Update**       | 2024-10-14                                                 |
| **Date Added**        | 2024-10-14                                           |
| **Category**          | Environment              |
| **Data Dates**        | 2000/01 - 2023/12                                    |
| **Source**               | [Hellenic Fire Service Dataset](https://www.fireservice.gr/el_GR/synola-dedomenon) |

### Data Description
The dataset provides information on forest and urban fire incidents where the Hellenic Fire Service (HFS) intervened. The data is available in a machine-readable format, and is governed by the terms of Annex C of the related circular (ADA: ΩΩΡΜΧ-ΜΒΛ). The terms include attribution to the creator, non-commercial use, and sharing alike.

### Data Preprocessing
The individual files are merged into a single dataset and cleaned to ensure consistency. Additionally, several helper columns are added to facilitate the analysis.

### Related Charts
<div class="pt-2">
<iframe width="800" height="446" src="https://lookerstudio.google.com/embed/reporting/513f28b7-eb4d-46ec-9322-e66476a0b86d/" frameborder="0" style="border:0" allowfullscreen sandbox="allow-storage-access-by-user-activation allow-scripts allow-same-origin allow-popups allow-popups-to-escape-sandbox"></iframe>
</div>

### Data Accessibility
1. You can download and analyze the data in Excel by clicking the "Download" button.
2. Alternatively, you can analyze the data online using the public dataset directly in [Google BigQuery](https://console.cloud.google.com/bigquery) with the following query:
   ```sql
   SELECT * FROM dataforgreece.public_data.forest_fires_greece_v
   ```


### Definitions for Dataset

| **Column**                        | **Description**                                                        |
|------------------------------------|------------------------------------------------------------------------|
| burned_forest_area                 | Forested areas that were affected by fire (stremma)                       |
| burned_groves                      | Small forested areas or groves affected by fire (stremma)                 |
| burned_grassland_areas             | Grasslands that were affected by fire (stremma)                           |
| burned_reeds_marshes               | Marshlands and reed-covered areas burned (stremma)                        |
| burned_agricultural_areas          | Agricultural lands that were affected by fire (stremma)                   |
| burned_crops_residues              | Leftover crops and residues from farming affected by fire (stremma)       |
| burned_landfills                   | Landfill or waste disposal sites affected by fire (stremma)                     |
| personnel_fire_brigade             | Firefighters from the fire brigade involved in firefighting operations |
| personnel_infantry_divisions       | Infantry units involved in fire operations                             |
| personnel_volunteers               | Volunteers assisting in firefighting operations                        |
| personnel_army                     | Army personnel involved in firefighting operations                     |
| personnel_other_forces             | Other forces that contributed to firefighting                          |
| vehicles_fire_vehicles             | Fire trucks and other firefighting vehicles                            |
| vehicles_municipal_vehicles        | Municipal vehicles involved in firefighting operations                 |
| vehicles_tanker_trucks             | Tanker trucks used to transport water for firefighting                 |
| vehicles_machinery                 | Heavy machinery used in fire response                                  |
| airborne_helicopters               | Helicopters used in aerial firefighting                                |
| airborne_aircraft_cl415            | CL-415 aircraft used for water bombing in firefighting                 |
| airborne_aircraft_cl215            | CL-215 aircraft used for aerial firefighting                           |
| airborne_aircraft_pzl              | PZL aircraft used for water bombing in firefighting                    |
| airborne_aircraft_gru              | GRU aircraft used for fire intervention                                |
| airborne_hired_helicopters         | Hired helicopters used for firefighting                                |
| airborne_hired_airplanes           | Hired airplanes used for aerial firefighting                           |

NOTE - 1 stremma = 1,000 m² = 0.1 hectrares. Greece has a total of 1.9 million hectares of forested area.