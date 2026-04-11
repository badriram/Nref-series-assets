# N_ref Paper Series — Code and Figures

[Time doesn't slow down, You do](https://badriram.github.io/Nref-series-assets) | [Graph Explorer](https://badriram.github.io/Nref-series-assets/explorer.html)

> Companion assets for a three-paper physics series on surplus structure in the temporal parameter.

📄 **Paper 1** — *Surplus Structure in the Temporal Parameter: Consequences of the Mass-Shell Constraint and the N_ref Substitution* — [Zenodo: 10.5281/zenodo.19386819](https://doi.org/10.5281/zenodo.19386819) | [Research Square](https://doi.org/10.21203/rs.3.rs-9285775/v1)

📄 **Paper 2** — *Counting Axioms for the Temporal Parameter: Axiomatic and Categorical Foundations of the N_ref Framework* — [Zenodo: 10.5281/zenodo.19462910](https://doi.org/10.5281/zenodo.19462910)

📄 **Paper 3** — *The Bondi k-Factor as Quantum Operator: A Two-Sector Decomposition of the Lorentz Transformation* — [Zenodo: 10.5281/zenodo.19387399](https://doi.org/10.5281/zenodo.19387399)

-----

## Repository Contents

### Code

**`computation.py`** — generates all figures for Paper 1.

```bash
pip install numpy scipy matplotlib
python computation.py
```

Produces:

- `fig1_two_arrows.png` — two-arrows independence diagram (process-accumulation vs thermodynamic)
- `fig2_four_qubit.png` — four-qubit clock illustration
- `fig3_wdw_minisuperspace.png` — Wheeler-DeWitt minisuperspace constraint surface

### Figures — Paper 1 (`paper1/`)

|File                         |Description                                                                  |
|-----------------------------|------------------------------------------------------------------------------|
|`fig1_two_arrows.png`        |Process-accumulation and thermodynamic arrows are independent                 |
|`fig2_four_qubit.png`        |Four-qubit internal clock illustration                                        |
|`fig3_wdw_minisuperspace.png`|WDW constraint surface; domain restriction to N_ref ≥ 0                       |
|`fig1_train.svg`             |Einstein train dual-ledger: P's simultaneous reception vs T's split receptions (§8 Bondi closure)|

### Figures — Paper 2

Paper 2 is the axiomatic/categorical foundations paper and contains no figures.

### Figures — Paper 3 (`paper3/`)

|File                    |Description                                                                                       |
|------------------------|--------------------------------------------------------------------------------------------------|
|`fig2_koperator.tex`    |TikZ source — k-factor operator decomposition: time dilation sector (nonlinear) vs simultaneity sector (linear)|
|`fig5_blurred_radar.svg`|Blurred radar diagram — sharp counts (classical) vs probability clouds (quantum k̂)                |

-----

## The Papers

### Paper 1 — Surplus Structure in the Temporal Parameter: Consequences of the Mass-Shell Constraint and the N_ref Substitution

The temporal parameter t ∈ ℝ carries three properties that no experiment has confirmed as features of physical reality: negative extension, loop-admitting topology, and reversal symmetry. These are identified as surplus structure (Weatherall, Gisin). Its operational content is N_ref: the accumulated state-transition count of a reference system, non-negative and monotonically non-decreasing — the caesium-133 hyperfine oscillator is one realisation. Two theorems are established. *Theorem 1*: restricting the Wheeler–DeWitt scalar-field clock to its operationally grounded domain φ ∈ [0,∞) halves the minisuperspace solution space, excluding independently contracting universes. *Theorem 2*: within the Page–Wootters framework, the process-accumulation arrow and the thermodynamic arrow are formally independent. The Bondi k-calculus then derives the full Lorentz transformation — including the relativity of simultaneity — from transition-count ratios between inertial observers, the relativity principle, and a finite signal speed c. No prior notion of time, metric, or spacetime is assumed; 1/γ is a theorem rather than an input.

📄 [10.5281/zenodo.19386819](https://doi.org/10.5281/zenodo.19386819) | [Research Square](https://doi.org/10.21203/rs.3.rs-9285775/v1)

### Paper 2 — Counting Axioms for the Temporal Parameter: Axiomatic and Categorical Foundations of the N_ref Framework

Four axioms (N1–N4) define N_ref as the accumulated state-transition count of a physical reference system; the definition is realisation-independent and structurally excludes the Pauli obstruction. The mass-shell constraint yields the Pikovski Hamiltonian Ĥ_phys = Ĥ₀/γ within the expansion regime, and the exact budget equation (dτ/dt)² + v²/c² = 1. A forgetful functor F: Math_t → Phys_N identifies surplus automorphisms of the mathematical temporal category that have no counterpart in the physical category. The computational gauge characterisation (CG1–CG3) shows that the surplus is mathematically necessary (Stone's theorem), informationally determined for KMS states (modular analyticity), and physically vacuous (axiom N1). The signature theorem proves that Minkowski (1,1) is forced by the non-compactness of the boost group — itself a theorem of counting and the relativity principle — and the extension to the full (1,3) signature follows from spatial isotropy via Schur's lemma. A universality proposition establishes that every physical clock satisfying N1–N4 dilates by 1/γ.

### Paper 3 — The Bondi k-Factor as Quantum Operator: A Two-Sector Decomposition of the Lorentz Transformation

This paper extends the derivation to the quantum level. The Bondi k-factor is promoted to an operator k̂ = (Ĥ_cm + p̂c)/(mc²), revealing a two-sector decomposition of the Lorentz transformation with structurally distinct quantum behaviour: a time dilation sector (k̂ + k̂⁻¹ = 2Ê/(mc²), nonlinear in momentum) and a simultaneity sector (k̂ − k̂⁻¹ = 2p̂c/(mc²), linear in momentum). The asymmetry is proved via Jensen's inequality: rest mass m > 0 bounds the energy spectrum below, making E(p) strictly convex, and convexity simultaneously produces Jensen corrections, Pikovski decoherence, and the Pauli obstruction — all confined to the time dilation sector. The simultaneity sector is protected exactly by linearity. The decomposition is universal across physically distinct clock types (light-bounce, radioactive decay, gravitational pendulum): which sector produces corrections and which is protected is independent of the clock mechanism. The framework provides a structural explanation for the angular separation of the quantum corrections computed by Grochowski et al. (2021), whose "quantum time dilation" and "quantum Doppler shift" contributions map onto the two sectors — separable by angular detection geometry. All corrections vanish in the classical limit σ_p → 0, recovering Paper 1's Bondi derivation exactly.

📄 [10.5281/zenodo.19387399](https://doi.org/10.5281/zenodo.19387399)

-----

## License

**Code** (`computation.py`): [MIT](LICENSE)

**Papers**: [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) — you may reuse and redistribute with appropriate credit to the author (Badriram Rajagopalan) and a link to the Zenodo record.
