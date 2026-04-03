# N_ref Paper Series — Code and Figures

> Companion assets for two published physics papers on surplus structure in the temporal parameter.

📄 **Paper 1** — [Zenodo: 10.5281/zenodo.19386819](https://doi.org/10.5281/zenodo.19386819)
📄 **Paper 2** — [Zenodo: 10.5281/zenodo.19387399](https://doi.org/10.5281/zenodo.19387399)

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

### Figures — Paper 1

|File                         |Description                                                  |
|-----------------------------|-------------------------------------------------------------|
|`fig1_two_arrows.png`        |Process-accumulation and thermodynamic arrows are independent|
|`fig2_four_qubit.png`        |Four-qubit internal clock illustration                       |
|`fig3_wdw_minisuperspace.png`|WDW constraint surface; domain restriction to N_ref ≥ 0      |

### Figures — Paper 2

|File                    |Description                                                                                       |
|------------------------|--------------------------------------------------------------------------------------------------|
|`fig1_train.svg`        |Einstein train dual-ledger: P’s simultaneous reception vs T’s split receptions                    |
|`fig2_koperator.svg`    |k-factor operator decomposition — time dilation sector (nonlinear) vs simultaneity sector (linear)|
|`fig3_visibility.svg`   |Fringe visibility V(L,T) decay at three cesium temperatures; coherence horizon L_C                |
|`fig4_experiments.svg`  |Experimental baselines vs L_C threshold; current and planned atom interferometers                 |
|`fig5_blurred_radar.svg`|Blurred radar diagram — sharp counts (classical) vs probability clouds (quantum k̂)                |

-----

## The Papers

### Paper 1 — Surplus Structure in the Temporal Parameter

The mass-shell relation E² = p²c² + m²c⁴ is a conserved-total resource constraint: total energy is fixed, and spatial momentum competes with internal dynamics for shares of it. The Pikovski Hamiltonian (H ≈ γmc² + Ĥ₀/γ) formalises this suppression. The Page-Wootters framework derives time from entanglement; Smith & Ahmadi (2020) proved PaW conditioning recovers Pikovski time dilation exactly. The SI second (9,192,631,770 cesium oscillations) grounds time operationally in internal state-transition counts — a domain mismatch with t ∈ ℝ. The relational observable N_ref replaces t. Three surplus properties of ℝ are audited and found unconfirmed by any experiment: negative extension (closed timelike curves), loop topology (closed timelike curves), and reversal symmetry (T-symmetry parameter reversal). The full Lorentz transformation including the simultaneity sector is derived from N_ref and the Bondi k-calculus with no manifold or synchronisation convention imported.

📄 [10.5281/zenodo.19386819](https://doi.org/10.5281/zenodo.19386819)

### Paper 2 — Quantum Corrections to the Lorentz Transformation

The k-factor is promoted to the operator k̂ = (Ĥ_cm + p̂c)/(mc²). For a detector in a momentum superposition, the Lorentz transformation acquires quantum corrections that are asymmetric: the time-dilation sector (which depends on energy, nonlinear in momentum) receives corrections at order (σ_p/mc)², while the simultaneity sector (linear in momentum) is protected to leading order. Fringe visibility in an atom interferometer decays as V(L) = exp(−(ω₀σ_pL/(mc²))²/2), with coherence horizon L_C ≈ 7.3 km for cold cesium at 1 μK. The primary experimental discriminator is the temperature dependence: the effect tracks σ_p = √(mk_BT), a property of the detector atom that no environmental noise source can mimic.

📄 [10.5281/zenodo.19387399](https://doi.org/10.5281/zenodo.19387399)

-----

## License

**Code** (`computation.py`): [MIT](LICENSE)

**Papers**: [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) — you may reuse and redistribute with appropriate credit to the author (Badriram Rajagopalan) and a link to the Zenodo record.
