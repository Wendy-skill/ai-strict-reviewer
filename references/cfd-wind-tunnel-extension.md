# CFD and Wind-Tunnel Review Extension

## Contents

- When to use
- CFD review checks
- Particle/DPM review checks
- Wind-tunnel review checks
- Verification and validation
- Scale and similarity
- Reporting boundaries

## When to Use

Use this extension only for studies that materially involve CFD, particle
transport, wind-tunnel experiments, or coupled numerical/experimental validation.

Do not assume every listed check is required. Apply only those relevant to the
actual methodology.

## CFD Review Checks

Consider:

- governing equations and modelling assumptions
- turbulence-model selection and justification
- steady versus unsteady formulation
- near-wall treatment
- y+ strategy where relevant
- wall functions or low-Re treatment where relevant
- inlet and outlet boundary conditions
- domain size and blockage effects
- mesh topology and refinement strategy
- local refinement around critical regions
- mesh independence or grid convergence
- GCI or other numerical-uncertainty assessment where appropriate
- residual convergence
- monitored physical quantities
- iterative stability
- numerical schemes
- solver settings
- sensitivity to influential modelling choices
- benchmark or experimental validation

Do not demand GCI mechanically if another defensible grid-convergence or numerical
uncertainty strategy is used.

## Particle / DPM Review Checks

Where relevant, consider:

- particle-size distribution
- particle density and material properties
- injection location and distribution
- injection velocity
- number of tracked particles
- particle-number independence
- stochastic tracking
- turbulent dispersion model
- gravity
- drag model
- one-way versus two-way coupling
- particle-particle interactions
- wall collision model
- restitution/rebound assumptions
- capture, trap, stick, or deposition criterion
- re-entrainment assumptions
- residence time and escape criteria
- sensitivity to random seed where stochastic tracking is used
- distinction between first-contact capture and retained deposition

Do not assume first contact is equivalent to experimentally retained mass unless a
retention model or supporting evidence justifies that equivalence.

## Wind-Tunnel Review Checks

Where relevant, consider:

- model scale
- blockage ratio
- test-section dimensions
- inflow profile
- atmospheric boundary-layer matching
- turbulence intensity
- integral length scale where relevant
- roughness representation
- reference velocity and height
- Reynolds-number effects
- Reynolds-number independence
- Froude similarity where gravity matters
- Stokes similarity where particle inertia matters
- particle-size scaling
- particle-density scaling
- instrumentation
- sampling frequency
- sampling duration
- repeatability
- uncertainty
- model mounting and edge effects
- facility limitations

## Verification and Validation

Keep these distinct:

### Numerical verification

Examples:

- mesh/grid convergence
- particle-number convergence
- iterative convergence
- timestep independence
- sensitivity to stochastic sampling
- numerical consistency

### Physical validation

Examples:

- pressure measurements
- velocity measurements
- concentration measurements
- deposition measurements
- benchmark data

A model may reproduce some observables well and others poorly.

Do not convert partial validation into universal model validity.

## Scale and Similarity

For scaled particle experiments, examine whether the thesis addresses the
dimensionless groups that materially affect the process.

Possible examples include:

- Reynolds number
- Froude number
- Stokes number

Do not require simultaneous similarity of all groups if that is physically
impossible.

Instead ask:

1. Which similarities are prioritised?
2. Which are not matched?
3. What physical consequences follow?
4. Does the thesis bound the resulting limitation?

## Reporting Boundaries

Distinguish carefully between:

- model-internal mechanism
- experimentally observed behaviour
- cross-facility agreement
- qualitative trend agreement
- quantitative validation
- design extrapolation

Do not allow agreement in one category to be silently presented as evidence for another.
