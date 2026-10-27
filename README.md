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

| Category   | Links                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Stack      | [![YAML](https://img.shields.io/badge/YAML-475569?logo=yaml&logoColor=white)](https://yaml.org/) [![GeoJSON](https://img.shields.io/badge/GeoJSON-475569)](https://geojson.org/)                                                                                                                                                                                                                                                         |
| Repository | [![Contributors](https://img.shields.io/github/contributors/wattnet/wattnet-data?label=Contributors&color=1E293B&logo=github&logoColor=white&labelColor=1E293B)](https://github.com/wattnet/wattnet-data/graphs/contributors) [![Stars](https://img.shields.io/github/stars/wattnet/wattnet-data?style=flat&label=Stars&color=1E293B&logo=github&logoColor=white&labelColor=1E293B)](https://github.com/wattnet/wattnet-data/stargazers) |
| License    | [![License](https://img.shields.io/github/license/wattnet/wattnet-data?label=License&color=64748B&logo=opensourceinitiative&logoColor=white&labelColor=1E293B)](https://github.com/wattnet/wattnet-data/blob/main/LICENSE)                                                                                                                                                                                                               |

This repository contains data files for Wattnet, including zone definitions, crossborder data, environmental factors, and GeoJSON of zones.

This is used as a **shared Git submodule** included in
[`wattnet-core`](https://github.com/wattnet/wattnet-core),
[`wattnet-forecast`](https://github.com/wattnet/wattnet-forecast) and
[`wattnet-api`](https://github.com/wattnet/wattnet-api).

It centralizes shared data constants to avoid duplication across projects. [`wattnet-dashboard`](https://github.com/wattnet/wattnet-dashboard) and [`wattnet-tools`](https://github.com/wattnet/wattnet-tools) do not use the submodule: they keep their own copies of the files they need, so those copies are not updated when this repository changes.

## Architecture

The following diagrams show how this repository's data is consumed across the Wattnet modules:

<div style="display: flex; width: 100%;">
  <img
    src="https://github.com/wattnet/wattnet-software-architecture/blob/main/diagrams/png/structurizr-1-wattnet_zone_data.png?raw=true"
    style="flex: 1; width: 0; height: 340px; object-fit: contain;"
  />
  <img
    src="https://github.com/wattnet/wattnet-software-architecture/blob/main/diagrams/png/structurizr-1-wattnet_environmental_data.png?raw=true"
    style="flex: 1; width: 0; height: 340px; object-fit: contain;"
  />
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

This work was developed within the [GreenDIGIT](https://greendigit-project.eu/) project, funded by the European Union's Horizon Europe research and innovation programme under grant agreement No. [101131207](https://cordis.europa.eu/project/id/101131207), and by the Swiss State Secretariat for Education, Research and Innovation (SERI).

<img src="https://github.com/wattnet/.github/raw/main/images/GreenDIGIT logo color horizontal2.png" alt="GreenDIGIT Logo" width="230" align="right"/>
<img src="https://github.com/wattnet/.github/raw/main/images/EN_FundedbytheEU_RGB_POS.png" alt="EU Funded Logo" width="260" align="left"/>
<img src="https://github.com/wattnet/.github/raw/main/images/Flag_of_Switzerland.svg" alt="Swiss State Secretariat for Education, Research and Innovation (SERI)" height="50" align="left"/>
<br clear="all"/>

##### © 2026 Spanish National Research Council (CSIC). All rights reserved.
