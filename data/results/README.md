# Annual results

`annual_end_use.csv` contains the values used in Table 7-1 and Figure 7-1. These are calculated from the supplied HIBO_09272026_JB.csv and unchanged IDF; no new EnergyPlus run is included.

Annual duration: 8,760 h; 52,560 ten-minute records. Total modeled floor area: 67.782169468 m². Excludes the duplicate plenum footprint; includes MEP.

Each rate is integrated as sum(W × 600 s) / 3,600,000 to obtain kWh. SI EUI is kWh divided by total floor area. Conversion to the reference unit uses 1 IT Btu = 1055.05585262 J and 1 ft² = 0.09290304 m².

| End use | Calculation basis |
| --- | --- |
| Interior equipment (electric) | Sum of three Zone Electric Equipment Total Heating Rate series plus Lost Heat Rate (zero in this run). |
| Interior lighting (electric) | Reconstructed from Lights Watts/Area, exact modeled zone areas, and ltg_sch_office under the supplied Monday-start annual calendar. |
| Exterior lighting (electric) | Reconstructed from Exterior:Lights design level 88.49 W and Exterior_lighting_schedule_a; schedule-only control. |
| Central heating (electric) | Integrated DXVAV SYS 1 HEATING COIL:Heating Coil Electricity Rate. |
| Terminal reheat (electric) | Sum of three terminal Heating Coil Heating Rate series divided by each entered efficiency (1.0). |
| Cooling (electric) | Integrated DXVAV SYS 1 COOLING COIL:Cooling Coil Electricity Rate, not thermal cooling output. |
| Fans (electric) | Sum of supply- and return-fan Fan Electricity Rate series. |

The seven reconstructed end-use rates sum to the reported facility electrical demand in every timestep (maximum absolute residual < 0.000001 W). This includes the exact scheduled lighting calculation; no unexplained residual has been assigned to a category. Terminal heat is treated as electricity only because its entered electric-coil efficiency is 1.0.

Original annual CSV SHA-256: `9a586bf5835065b55b1bd8bf56e43c02befaaaa3549448d894d27e9225160d34`. The full annual CSV is not duplicated in this compact repository.
