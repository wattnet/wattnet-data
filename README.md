<div align="left">
  <picture>
    <source media="(prefers-color-scheme: dark)"
            srcset="https://github.com/wattnet/.github/raw/main/images/wattnet-logo-full-dark-transparent-cropped.png" />
    <source media="(prefers-color-scheme: light)"
            srcset="https://github.com/wattnet/.github/raw/main/images/wattnet-logo-full-light-transparent-cropped.png" />
    <img src="https://github.com/wattnet/.github/raw/main/images/wattnet-logo-full-light-transparent-cropped.png"
         alt="Wattnet Logo"
         width="300" />
  </picture>
</div>
# Data Repository
 
This repository contains data files for wattnet, including zone definitions, crossborder data, environmental factors, and GeoJSON of zones.
 
This is used as a **shared Git submodule** included in
[`wattnet-core`](https://github.com/wattnet/wattnet-core),
[`wattnet-forecast`](https://github.com/wattnet/wattnet-forecast),
[`wattnet-api`](https://github.com/wattnet/wattnet-api),
[`wattnet-dashboard`](https://github.com/wattnet/wattnet-dashboard) and
[`wattnet-tools`](https://github.com/wattnet/wattnet-tools).
 
It centralizes shared data constants to avoid duplication across projects.
 
## Architecture
 
The following diagrams show how this repository's data is consumed across the wattnet modules:
 
<div align="left">
  <img src="https://github.com/wattnet/wattnet-architecture/blob/main/diagrams/png/structurizr-1-wattnet_zone_data.png?raw=true" alt="Zone data dependencies" width="48%"/>
  <img src="https://github.com/wattnet/wattnet-architecture/blob/main/diagrams/png/structurizr-1-wattnet_environmental_data.png?raw=true" alt="Environmental data dependencies" width="48%"/>
</div>
 
## Repository Structure
 
- `zones/`: Contains zone definition files in YAML format.
- `footprint/`: Contains files with the factors for footprint calculations.
- `impact/`: Contains files with the factors for impact calculations.
- `geojson/`: Contains GeoJSON files representing the geographical boundaries of individual zones.
  - `fullmap/`: Contains a unified GeoJSON file with all zones.
## License
 
This repository is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
See the [LICENSE](LICENSE) file for more details.
 
## Funding and Acknowledgments
 
This work is funded by the European Union's Horizon Europe research and innovation programme through the **[GreenDIGIT](https://greendigit-project.eu/)** project, under grant agreement **[101131207](https://cordis.europa.eu/project/id/101131207)**.
 
<div align="left">
  <img src="https://github.com/wattnet/.github/raw/main/images/EN_FundedbytheEU_RGB_POS.png" alt="EU Funded Logo" width="260"/>
  <img src="https://github.com/wattnet/.github/raw/main/images/GreenDIGIT%20logo%20color%20horizontal2.png" alt="GreenDIGIT Logo" width="230"/>
</div>


##### © 2026 Spanish National Research Council (CSIC). All rights reserved.
