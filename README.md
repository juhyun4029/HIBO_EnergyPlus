# HIBO EnergyPlus building model

EnergyPlus model of the Human-Centered Integrated Building Operation laboratory in Omaha, Nebraska. **Model: 28 September 2026. EnergyPlus: 22.2.0.**

## Model report

[PDF](reports/HIBO_Model_Report.pdf) · [Word](reports/HIBO_Model_Report.docx) · [HTML](reports/HIBO_Model_Report.html)

The report describes the building and its implemented simulation inputs: weather and simulation settings, geometry and zoning, materials and constructions, occupancy and internal gains, schedules, HVAC, controls, and air exchange. Annual end-use energy and EUI follow the input sections. Values, units, and source information are shown together.

Exact schedules are in Appendix A; additional connections, curves, and output requests are in Appendix B. The [complete input register](docs/complete-inputs.html) contains all entered IDF fields and geometry vertices; [input tables](data/inputs/) provide the same model data in tabular form. Download the repository and open `docs/index.html` to read the illustrated report in a browser.

## Run with EP-Launch

Use **EP-Launch from EnergyPlus 22.2.0**. Select `model/HIBO_09282026_JB.idf` and `weather/USA_NE_Omaha-Eppley.Airfield.725500_TMY3.epw`, then click **Simulate**. Both files are included. No programming environment is required.

| Folder | Contents |
| --- | --- |
| `model/` | EnergyPlus IDF |
| `weather/` | Omaha TMY3 EPW |
| `reports/` | Model report in Word, PDF, HTML, and Markdown |
| `docs/` | Browser report, complete input register, and figures |
| `data/` | Input inventories and annual end-use results |
| `reference/` | Annual HTML report, zone-sizing profiles, and path-redacted error log |
| `sources/` | Supporting-source notes |

Only the IDF and EPW are needed to simulate. Folder names are organizational; EP-Launch can select files from other locations. Drawings and the nameplate photograph are supporting evidence, not runtime inputs. The EPW is already included.

The model uses reference properties and operating assumptions as well as drawing/nameplate evidence; it is not a field-calibrated model. The included IDF and weather file are the simulation inputs; the reference folder contains the supplied outputs. See [source notes](sources/README.md) before distributing supporting drawings.
