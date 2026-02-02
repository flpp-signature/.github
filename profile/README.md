# SignAture

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Multi-functional modelling tool for the significantly altering future electricity markets and their development**

This organization hosts open-source tools and models developed during the SignAture research project (2022–2025), funded by the Latvian Council of Science (project No. lzp-2021/1-0227).

## Overview

The SignAture project addresses key challenges in evolving electricity markets through three complementary research streams:

| Repository | Focus | Framework |
|------------|-------|-----------|
| [Baltic-Model](https://github.com/flpp-signature/Baltic-Model) | Power system operational optimization | SpineOpt (Julia) |
| [BESS-Simulation](https://github.com/flpp-signature/BESS-Simulation) | Battery storage reserve provision | Python |
| [Market-Impact](https://github.com/flpp-signature/Market-Impact) | Wholesale market welfare analysis | Python |

## Repositories

### 🔋 [Baltic-Model](https://github.com/flpp-signature/Baltic-Model)

Operational optimization models of the Baltic power system (Estonia, Latvia, Lithuania) using the [SpineOpt](https://github.com/spine-tools/SpineOpt.jl) framework and Spine Toolbox.

**Features:**
- 2020 calibration/validation model with historical data
- 2050 future scenarios with high renewable penetration (6 GW wind, 2 GW solar)
- Detailed Daugava hydropower cascade modeling with reservoir dynamics
- Heat-electricity coupling for CHP plants
- Sensitivity analyses for demand, RES capacity, storage, and hydrological conditions

**Publications:**
- Baltputnis & Broka (2023). *Future scenarios of the Baltic power system with large penetration of renewables.* [doi:10.1109/EEM58374.2023.10161795](https://doi.org/10.1109/EEM58374.2023.10161795)
- Baltputnis et al. (2024). *Refinement and Calibration of Optimization Models for Baltic Region Energy System Development.* [doi:10.1109/RTUCON62997.2024.10830801](https://doi.org/10.1109/RTUCON62997.2024.10830801)

---

### ⚡ [BESS-Simulation](https://github.com/flpp-signature/BESS-Simulation)

Simulation tool for Battery Energy Storage System (BESS) reserve provision, implementing a robust market-based management strategy for European balancing markets.

**Features:**
- Simultaneous FCR and aFRR market participation
- Market-based SOC restoration via intraday trading
- Full EU System Operation Guideline compliance for Limited Energy Reservoirs (LERs)
- Conservative and active SOC management strategies
- Voluntary FRR bidding with exhaustive worst-case validation

**Publication:**
- Baltputnis et al. (2024). *Robust market-based battery energy storage management strategy for operation in European balancing markets.* Journal of Energy Storage, 102, 114082. [doi:10.1016/j.est.2024.114082](https://doi.org/10.1016/j.est.2024.114082)

---

### 📊 [Market-Impact](https://github.com/flpp-signature/Market-Impact)

Market simulation framework for assessing price changes and welfare impacts from new market participants in electricity wholesale markets, with focus on independent aggregator (IA) participation in the Nordic day-ahead market.

**Features:**
- Simulations using historical Nord Pool bid/offer curves
- Welfare impact analysis (producer surplus, consumer surplus, DR consumer welfare)
- Compensation payment socialization scenarios
- Generalizable to any pay-as-cleared auction market
- Extensible to various market participants (storage, EVs, prosumers, etc.)

**Publication:**
- Baltputnis et al. (2025). *Independent Aggregation in the Nordic Day-Ahead Market: What is the Welfare Impact of Socializing Supplier Compensation Payments?* Heliyon, 11(1), e41619. [doi:10.1016/j.heliyon.2024.e41619](https://doi.org/10.1016/j.heliyon.2024.e41619)

---

## Data availability

Simulation inputs, intermediary results, and final outputs are available on Zenodo:

| Dataset | DOI |
|---------|-----|
| Baltic Model data | [10.5281/zenodo.18442640](https://doi.org/10.5281/zenodo.18442640) |
| BESS Simulation data | [10.5281/zenodo.18199324](https://doi.org/10.5281/zenodo.18199324) |
| Market Impact data | [10.5281/zenodo.18434501](https://doi.org/10.5281/zenodo.18434501) |

## Getting started

Each repository contains detailed installation and usage instructions. General requirements:

| Repository | Requirements |
|------------|--------------|
| Baltic-Model | [Spine Toolbox](https://github.com/spine-tools/Spine-Toolbox), Julia 1.8+, SpineOpt.jl |
| BESS-Simulation | Python 3.8+, NumPy, Pandas, Matplotlib |
| Market-Impact | Python 3.8+, NumPy, Pandas, Matplotlib |

## Acknowledgments

<table>
  <tr>
    <td><img src="https://www.lzp.gov.lv/sites/lzp/files/gallery_images/rtu_flpp_logo_purple1.jpg" alt="Logo" width="200"></td>
    <td>This research is funded by the Latvian Council of Science, project "Multi-functional modelling tool for the significantly altering future electricity markets and their development (SignAture)", project No. lzp-2021/1-0227.</td>
  </tr>
</table>

## License

All repositories in this organization are licensed under the MIT License.

## Contact

For questions about the SignAture project or these tools, please open an issue in the relevant repository.
