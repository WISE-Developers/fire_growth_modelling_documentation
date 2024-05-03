# Agenda

## 1. Franco update

nest.js - using in GNWT intended to be used for CWFMF in the future.

## 2. Neal on Foundation

No go, looking for a way to get money out of CIFFC and useful. 

Working with Canada Wildfire on getting things attached with them through WRFI project.

More freedom with money used from Canada Wildfire and WRFI. 

## 3. Development Priorities

** Must Do **

Actually opening source, AGPL 3 compliant
End of Life Prometheus - Actually do this.
Actual example that is deployable and runnable.
Median - we need real statistical outputs

** Nice to have **

Training
Dataset - Sam reached out to Matt and said the 30m, 100m, 250m fuel grid is coming their way
Expand wx service for all models US - EU etc
Keep wx as a grid
Cutter for ingesting data
Automatic tuning of the tool (wx etc)

## Remaining CIFFC Funds
- BC did not provide approval for Neal to be part of a not-for-profit foundation.
- Canada Wildfire may be an option for CIFFC to transfer remaining WISE funds to.
- Canada Wildfire is a now a not-for-profit.
- GNWT is a member of Canada Wildfire. Franco will investigate is this option is acceptable for GNWT.

## Wildfire Resilient Futures Initiative (WRFI)
Initiative within the Government of Canada Adaptation Action Plan, in support of the National Adaptation Strategy, launched on June 27, 2023. Building and mobilizing foundational wildland fire knowledge is one of three interrelated activities. With $48 Million to invest over 4 years starting in April 2024, the Build and Mobilize Foundational Wildland Fire Knowledge Program aims to encourage collaborative research and demonstration projects focused on innovation in wildfire risk assessment, risk mitigation, and adaptive forest management as per the Blueprint for Wildland Fire Science in Canada. Neal is scrammbling to put together a proposal with Mike Flannigan and TRU under Theme 1: Wildfire risk assessment. This theme includes a focus on leveraging new technologies, and integration of research into predictive models and decision-making tools.

## Development priorities to include in WRFI proposal
- End-of-Life Prometheus.
- Open source WISE.
- Developer documentation and unit testing for WISE.
- National fuel dataset for WISE implementation.
- A working example of WISE implementation.
- Abstraction API for all models in the CWFMF (FireSTARR, Cell2Fire, WISE, Burn-P3?).
- New modern interface for guided automation or human-in-the-loop modelling by a fire behaviour specialist. Interface should provide option to use all fire simulation engines in the CWFMF.
- Integration of CWFMF weather forecast service for WISE implementation.
- Expand CWFMF weather service to include all numerical weather model sources used by wildfire management agencies (Canada, US, European).
- Enhance fire growth models to use raw numerical weather model outputs (rasters) instead of extracting weather streams for point locations.
- Median fire behaviour statistics (tabular and raster).
- Spotting module.
- Wind gusting.
- Next generation CFFDRS implementation.
- Self-tuning weather models based on observation network (auto-tune).
- Machine learning for fire growth modelling (auto-tuning fire spread models).
