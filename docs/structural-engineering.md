# Structural engineering and calculations

Status: concept basis; all values require site-specific verification.

## Load path and VCG
Permanent and variable actions travel from equipment/decks through secondary steel, primary beams, grillage, jacket legs/diagonals, piles and soil. For masses m_i at elevations z_i, VCG z_G = Σ(m_i z_i)/Σm_i. Shift of a subsystem Δm from z_1 to z_2 changes VCG by Δz_G = Δm(z_2-z_1)/M_total. Keep dense BESS, transformers and process vessels low; reserve upper decks for lighter weather-sensitive equipment. Check intact, damaged, installation, transport and accidental conditions.

## Overturning
With reference at seabed or foundation datum, the first-moment equilibrium gives M_overturning ≈ W e + F_wind h_wind + F_wave h_wave + F_current h_current, where W is vertical resultant, e its eccentricity, and F/h are horizontal force and lever arm. Include inertia, hydrodynamic added mass, slamming, crane loads, vessel impact, seismic where applicable, and directional combinations. Foundation resistance must satisfy factored sliding, overturning, uplift and bearing checks; report utilization and reserve.

## Dynamics and resonance
For a reduced SDOF check, T_n = 2π√(m/k), ω_n=√(k/m), and dynamic amplification for harmonic force is |X/F| = 1/k / √((1-r²)²+(2ζr)²), r=ω/ω_n. Build a 3-D mass/stiffness model; solve [K−ω²M]φ=0, normalize modes, include hydrodynamic added mass and soil springs, and combine modal responses (SRSS/CQC as appropriate). Screen platform modes away from dominant wave periods Tp=14–22 s and rotating machinery frequencies; assess fatigue spectral response, vortex shedding and nonlinear coupling.

## Air gap
Required crest elevation: z_crest ≥ z_tide + z_surge,100 + z_wave,100 + z_runup/shoaling + margin. Air gap = z_deck − (still water level + crest elevation above SWL); target concept range 15–25 m, but verify with joint-probability metocean data, green-water, spray, subsidence and construction tolerance. Do not treat average Hs as an extreme design value.

## Foundations and geotechnics
Characterize stratigraphy, cyclic degradation, liquefaction, scour and installation effects. For driven tubular pin piles, derive axial compression/tension from shaft friction and end bearing and lateral response with API/DNV p–y curves: soil reaction p(y), pile equilibrium EI y'''' + N y'' + p(y)=q(z). Include nonlinear springs, cyclic reduction, group effects, pile drivability, fatigue and buckling. Compare skirt piles for load sharing and scour protection against pin piles for installation flexibility. Check axial/lateral capacity, global stability, differential settlement, pile-soil stiffness, corrosion allowance and cathodic protection. Model scour depth and remedial rock/mat systems explicitly.

## Verification checklist
Freeze environmental contours; document load cases and factors; reconcile FE reactions to hand sums; sensitivity-test VCG, stiffness, scour and damping; independently review model, units and combination logic; issue calculation workbook with input/output traceability.