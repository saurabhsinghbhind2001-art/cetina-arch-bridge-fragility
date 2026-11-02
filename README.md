# Seismic fragility of a long-span RC deck arch bridge: data and scripts

Data and analysis scripts for the paper "Seismic fragility of a long-span RC deck arch bridge under three-component and spatially varying ground motion" by Saurab Singh, Juned Raheem and Dheeraj Kaurav (Department of Civil Engineering, MANIT Bhopal, India).

| File | Content |
|---|---|
| S1_ground_motion_records.csv | The 35 FEMA P695 records (NGA-West2 RSN, event, station, magnitude, distance), the scale factors at the 14 intensity levels and the multi-support subset |
| S2_all_runs_peak_responses.csv | One row per nonlinear time-history analysis: case, record, Sa(T1) level, damping model, element formulation, completion and collapse flags, peak drifts, shears, springing curvatures, crown displacements, residual drift and device responses. Drifts are ratios. `C5C6_ddrift_long`/`_trans`: deformation drift (chord drift minus base rotation), the largest of legs 5L, 5R, 6L, 6R; this is the quantity used in the limit states and figures of the paper. `C5C6_drift_*_chord` and `max_col_drift_*_chord`: chord drift. `crown_rel_vert_m` / `deck_crown_rel_vert_m`: peak vertical displacement of the arch / deck crown relative to the springings (used in the paper); `*_max_component_m`: the largest of the three components. |
| S3_fragility_parameters.csv | Lognormal fragility medians and dispersions for every case and damage state, with the exceedance counts behind each fit |
| S4_analysis_scripts.zip | OpenSeesPy model and drivers, ground-motion processing and spatially varying motion simulation, limit-state, fragility, bootstrap, hazard and figure scripts |

The NGA-West2 acceleration files are not redistributed; download them from the PEER database by the RSNs in S1.

Licence: CC BY 4.0.
