# Capex derivation model

All figures are screening ranges in nominal USD and must be replaced by vendor quotations, market indices, logistics studies and escalation assumptions.

## Cell-level build-up
Substructure/foundation: steel tonnes × fabricated-and-coated $/t + pile material + driving spreads + marine logistics + heavy-lift vessel day rate × campaign days + weather-window contingency + engineering/QA. This produces the concept range $80–250m/cell. Record tonnage, rate, vessel, mobilization, days, standby, fuel and contingency separately.

Topside decks: primary steel tonnes + secondary steel/grillage + blast/firewalls + coating/fireproofing + module supports + fabrication/assembly + commissioning. The concept range is $85–310m; reconcile deck area, steel intensity, module count and lift weights.

BESS: energy capacity × installed marine-grade battery price ($300–700/kWh) + MV collection + marine switchgear + EMS + HVAC/fire suppression + foundations/cabling + installation and spares. For 500 MWh, battery-only arithmetic is $150–350m; package range $200–500m includes balance of plant and offshore execution.

Compute: nitrogen-purged modular shells, GPU/IT fit-out, liquid-cooling distribution, titanium plate heat exchangers, seawater pumps/intake/discharge, UPS, MV/LV distribution, controls, fire protection and commissioning. Aggregate bottom-up quantities to $160–770m; separate IT hardware from civil/marine infrastructure and refresh cycles.

Biorefinery: mechanical intake/handling + dewatering + anaerobic digestion + gas cleanup + HTL pressure vessels/pumps + heat recovery + utilities + tanks + effluent and safety systems. Bottom-up package range $170–800m; pressure boundary, materials, hazardous area and marine corrosion are major sensitivities.

## 10-ha aggregation
Sum cells, bridges, shared utilities, export, accommodation, port/logistics, development, owner’s costs, contingency and escalation; avoid double-counting shared BESS, intake and control systems. Scenario bands: low $2–4B; central $4–8B; high $8–15B+. Create a quantity/rate/schedule for each scenario and Monte Carlo or P50/P90 uncertainty rather than hiding contingency.

## Legacy versus newbuild
A $1 nominal transfer is not the project cost. Add surveys, title/environmental liabilities, structural life extension, fatigue and remaining-life assessment, topsides removal, brownfield tie-ins, hazardous materials, decommissioning security and downtime. Compare NPV, schedule risk, capacity/utilization, certification and residual liability against a purpose-built cell; use an option-gated decision.

## Audit fields
For each line: WBS, quantity, unit, currency/year, source URL or quotation, date, escalation index, location factor, productivity, vessel assumptions, contingency basis, confidence grade, inclusions/exclusions and reviewer. Link engineering quantities to [structural basis](structural-engineering.md) and environmental assumptions to [metocean basis](metocean-gulf-of-guinea.md).