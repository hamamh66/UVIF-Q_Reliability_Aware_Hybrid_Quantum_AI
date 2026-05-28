# UVIF-Q: Reliability-Aware Hybrid Quantum-Classical AI

This repository provides a reproducible implementation of the **Quantum-Classical Unified Variational Intelligence Framework (UVIF-Q)**, a reliability-aware and equilibrium-oriented framework for hybrid quantum-classical artificial intelligence in the NISQ era.

## Overview

UVIF-Q extends the Unified Variational Intelligence Framework into hybrid quantum-classical learning by modeling intelligent behavior as a constrained variational equilibrium among multiple operational pressures:

- task performance,
- uncertainty regulation,
- risk sensitivity,
- circuit and model complexity,
- decision-relevant information utility,
- and quantum decoherence pressure.

The repository supports experimental validation of UVIF-Q as a multi-objective reliability layer for hybrid quantum-classical systems rather than as a claim of quantum computational advantage.

## Main Features

- Hybrid quantum-classical learning prototype.
- Variational quantum circuit implementation.
- UVIF-Q multi-objective loss construction.
- Task-only and UVIF-Q ablation configurations.
- Uncertainty, risk, complexity, information, and decoherence terms.
- Repeated-seed validation.
- Calibration and Expected Calibration Error analysis.
- Adversarial robustness evaluation.
- Noise-sensitivity and decoherence diagnostics.
- Publication-ready figures and tables.
- Google Colab-compatible execution workflow.

## Repository Structure

```text
UVIF-Q_Reliability_Aware_Hybrid_Quantum_AI/
│
├── notebooks/
│   ├── UVIF_Q_Prototype_Validation_Notebook.ipynb
│   └── UVIF_Q_Fast_Upgrade_Notebook.ipynb
│
├── figures/
│   ├── Framework_Overview.png
│   ├── Fig_UVIFQ_Fast_Ablation_Performance_CI.png
│   ├── Fig_UVIFQ_Fast_Calibration_ECE_CI.png
│   ├── Fig_UVIFQ_Fast_Noise_Sweep.png
│   └── Fig_UVIFQ_Fast_Reliability_Robustness_Map.png
│
├── tables/
│   ├── table_uvifq_fast_repeated_results.csv
│   ├── table_uvifq_fast_summary_ci.csv
│   └── table_uvifq_noise_sweep.csv
│
├── outputs/
│   ├── outputs_summary_fast_upgrade.txt
│   ├── manuscript_interpretation_fast_upgrade.txt
│   └── file_index.csv
│
└── README.md
```

## Experimental Design

The repository includes two complementary notebooks:

1. **Full prototype notebook**  
   Provides the main UVIF-Q proof-of-concept validation with multiple ablation settings and publication-ready outputs.

2. **Fast upgraded notebook**  
   Provides a faster reviewer-oriented repeated-run validation with:
   - three independent random seeds,
   - reduced configurations,
   - confidence-interval summaries,
   - focused noise-sensitivity analysis,
   - calibration and robustness diagnostics.

## UVIF-Q Objective

The UVIF-Q functional is formulated as:

```math
J_{UVIF-Q}[\pi]
=
\mathbb{E}
\left[
L_{task}(\pi)
+
\alpha U(\pi)
+
\beta R(\pi)
+
\gamma C(\pi)
-
\delta I(\pi)
+
\epsilon D_Q(\pi)
\right]
```

where:

- `L_task` is the task loss,
- `U` is uncertainty pressure,
- `R` is risk sensitivity,
- `C` is complexity regularization,
- `I` is decision-relevant information utility,
- `D_Q` is decoherence pressure.

## Dataset

The prototype uses the Wisconsin Breast Cancer Diagnostic benchmark with PCA-based dimensionality reduction for quantum angle encoding.

The dataset is used only as a compact proof-of-concept benchmark for testing the operational behavior of the UVIF-Q framework.

## Key Outputs

The implementation automatically generates:

- repeated-run performance tables,
- calibration summaries,
- robustness summaries,
- noise-sensitivity tables,
- confidence-interval plots,
- reliability--robustness maps,
- and a framework overview figure.

## Reproducibility

The notebooks are designed for execution in Google Colab and automatically save results to Google Drive under structured output folders.

The implementation includes:

- fixed random seeds,
- automated logging,
- generated figures,
- generated tables,
- manuscript interpretation files,
- and indexed output artifacts.

## Scientific Positioning

This repository does **not** claim quantum advantage or quantum supremacy.

Instead, UVIF-Q is positioned as a reliability-aware, multi-objective, equilibrium-oriented framework for hybrid quantum-classical artificial intelligence, especially under noisy intermediate-scale quantum constraints.

## Citation

If this repository is used, please cite the associated manuscript:

```bibtex
@misc{hamam2026uvifq,
  author       = {Hamam, Habib and collaborators},
  title        = {UVIF-Q: Reliability-Aware Hybrid Quantum-Classical Artificial Intelligence},
  year         = {2026},
  publisher    = {GitHub},
  note         = {Reproducible implementation of the Quantum-Classical Unified Variational Intelligence Framework},
  howpublished = {\url{https://github.com/hamamh66/UVIF-Q_Reliability_Aware_Hybrid_Quantum_AI}}
}
```

## License

A license file should be added before public release. For academic reproducibility, the MIT License or Apache License 2.0 may be considered.

## Contact

For questions or collaboration inquiries, please contact the corresponding author through the manuscript or repository profile.
