# Taxonomy, compute sizing, and energy budget

## Taxonomy and naming
Use five levels: sector > base > vertical > market > segment. Example: Energy & Compute > Offshore Hybrid Platform > GPU Compute / Marine Biorefinery / BESS > AI training, inference, HPC, renewable fuels, grid services > named product, customer, duty cycle and geography. Stable IDs should be PLATFORM-CELL-###, DECK-##, HALL-##, BESS-##, BIO-##; maintain a registry with owner, interface, revision and safety classification.

Platform naming should encode site, cluster, cell and function. Networking is layered: bridge-linked mesh between cells; redundant subsea fiber rings to shore/data landing; satellite backhaul for out-of-band control and emergency operations. Microgrids may be off-grid islanded, grid-tied, or grid-forming hybrid; define black-start, protection zones, synchronization and load-shed priorities.

## 50 m x 50 m module footprint
Gross plan area = 2,500 m². After jacket legs, risers, escape routes, fire separation, access, lifting and utilities, use 1,400–1,750 m² usable per deck tier as a planning allowance. At five tiers this is 7,000–8,750 m² gross usable deck area, not a guaranteed IT footprint.

## Compute options and sizing
Air-cooled 40-ft ISO shells are simple but require high airflow, filters, acoustic treatment and larger heat rejection. Single-phase direct-liquid cooling (DLC) serves cold plates; two-phase DLC/immersion uses dielectric tanks and can achieve higher rack density but adds fluid, containment and service complexity. Krampitz-like ISO modules or bespoke marine containers require marine structural, fire, corrosion, lifting and hazardous-area qualification.

Illustrative planning arithmetic: N_containers = ceil(A_IT / A_container_effective); N_racks = N_containers × racks/container; IT MW = racks × rack_kW / 1,000. Use measured vendor values for rack kW and floor area. H100/B200 density depends on server SKU, networking, storage and derating; do not equate GPU count with useful compute without a power and thermal envelope.

Floor loading must be checked from equipment dead load + dynamic/service loads divided by support area, with local point loads and roll paths. No universal limit is assumed: verify deck plate, grillage, primary steel and jacket reactions. Volumetric efficiency increases with liquid cooling, but maintenance clearances and fire compartments reduce theoretical packing.

Planning PUE: air cooling approximately 1.20–1.40; immersion approximately 1.03–1.08, subject to seawater pumps, heat exchangers, controls and ambient conditions. Total facility power = IT power × PUE + non-IT process loads.

## Power budget and heat
A compute module may be screened at 20–50+ MW facility draw; a 10-ha cluster may scale toward 500 MW. These are scenarios, not design capacities. Heat rejected is approximately Q = P_IT × 3.412 MMBtu/h per MW, or Q ≈ P_IT MW thermally. Seawater heat exchanger duty Q = m_dot c_p ΔT; pump parasitics, fouling, biosecurity, discharge temperature and intake/discharge separation must be included in PUE.

Balance resources with offshore wind/solar profiles, biogas/biomethane from sargassum AD, BESS buffering, grid import/export and backup fuel cells. For storage autonomy t hours at load P MW, usable BESS ≈ P × t / (DoD × round-trip efficiency); add reserve and degradation margin. AD gas yield must come from feedstock characterization and measured methane yield; dispatchable generation is limited by collection, digestion, cleanup and engine/fuel-cell efficiency.

## Verification gates
Freeze density/rack/vendor assumptions; calculate deck reactions and VCG; run thermal CFD and HX fouling cases; perform short-circuit/protection and harmonic studies; define islanding and black-start; validate fiber latency/redundancy; reconcile PUE and BESS autonomy with 8760-hour dispatch. Link to [structural engineering](structural-engineering.md), [capex](capex-derivation-model.md), and [metocean](metocean-gulf-of-guinea.md).