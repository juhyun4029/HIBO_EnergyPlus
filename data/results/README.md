# Simulation results

`annual_end_use.csv` supplies Table 7-1 and Figure 7-1 in the model report.

Source: [`HIBO_09282026_JBTable.html`](../../reference/HIBO_09282026_JBTable.html), EnergyPlus 22.2.0-c249759bad, simulation timestamp 28 September 2026, 14:03:43. Annual duration: 8,760 hours. Total modeled floor area: 67.782169468 m², including MEP and excluding the duplicate plenum footprint.

Annual end-use electricity is read from **Annual Building Utility Performance Summary → End Uses**. Total electricity is read from **Electric Loads Satisfied → Total Electricity End Uses**. End-use entries are reported to 0.01 GJ; the facility total is reported to 0.001 GJ. Converted kWh, EUI and percentages are approximate. Independently rounded end uses do not sum exactly to the reported facility total.

Conversions: kWh = GJ / 0.0036; EUI = kWh / floor area. The customary-unit conversion uses 1 IT Btu = 1055.05585262 J and 1 ft² = 0.09290304 m². Heating combines the central electric heater and terminal reheaters; the supplied annual table does not separate their electrical consumption.

The reference folder contains:

| File | Contents |
| --- | --- |
| `HIBO_09282026_JBTable.html` | Annual summary, equipment sizing, and envelope reports |
| `HIBO_09282026_JBZsz.csv` | Zone-sizing design-day profiles; not annual timestep results |
| `HIBO_09282026_JB.redacted.err` | Simulation diagnostics with the local machine path redacted |

These are the supplied simulation outputs. No new EnergyPlus run is included.
