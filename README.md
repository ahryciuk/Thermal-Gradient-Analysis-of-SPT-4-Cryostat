# Thermal-Gradient-Analysis-of-SPT-4-Cryostat
Assessment of thermal gradient across conductive pathways from Pulse Tube Cryo-cooler to key internal subassemblies

## My Role:
- performed both analytic and finite element analyses to evaluate thermal gradients across the 50 Kelvin and 4 Kelvin subassemblies
- developed Python code bases to perform analytic calculations with varying design geometry and material properties

## Notes and Assumptions:
- material properties from [NIST database](https://trc.nist.gov/cryogenics/materials/materialproperties.htm)
- contact resistance of OFHC copper: Siddappa, P., & Tariq, A. 2023, Applied Thermal Engineering, 219, 119412, doi: https://doi.org/10.1016/j.applthermaleng.2022.119412
- SPT-3G empirically showed braided OFHC copper heat straps have a load-dependent temperature drop of ~0.12 K/W for 2"x2" footprints
- PT420 cold head temperatures (see [Thermal Budget](https://github.com/ahryciuk/Thermal-Budgeting-of-SPT-4-Cryostat)): https://cdn.bluefors.com/wp-content/uploads/2023/09/22145601/PT420-RM-Capacity-Curve.pdf
- heat generation from optics tubes based on lens absorption is ~30 mW per tube
- heat generation from alumina filters is ~1.2 W per tube (see [Thermal Budget](https://github.com/ahryciuk/Thermal-Budgeting-of-SPT-4-Cryostat)) 


## Summary of Results:

Thermal Gradients by Subassembly (units in Kelvin)
| 50 Kelvin (1D) | 50 Kelvin (FEA) | 4 Kelvin (1D) | 4 Kelvin (FEA) | Optics Tube Spread (Al1100) | Optics Tube Spread (OFHC Cu) |
|:-------:|:-------:|:-------:|:-------:|:-------:|:-------:|
| 19.7 | 18.12 | 4.14 | 4.61 | 1.88 | 0.24 |

## Files:
- Summary plots: /summary_plots/
- Analysis document: SPT4_Cryostat_Temperature_Gradient_Characterization.pdf
- Python code: /python_code/
