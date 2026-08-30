# Hybrid Variational Quantum-Classical Framework with Adaptive Weighting and Efficiency Assessment

**Dilli Hang Rai**

**Institute of Science and Technology**

**Tribhuvan University, Kritipur, Nepal**

**dillihangrae@gmail.com**

Hybrid quantum-classical neural networks have emerged as a promising approach for leveraging quantum computing in machine learning while mitigating current hardware limitations. This paper presents Sim-HVQC, a hybrid Deep Quantum Neural Network that couples an adaptive, parameter-free SimAM weighting module with classical feature extraction to preserve class-discriminative information prior to encoding into a Variational Quantum Circuit (VQC). Previous studies are restricted to binary classification [1] [2] [3], [4] [5]. In contrast, the proposed framework is trained and evaluated on various multi-class datasets(MNIST, KMNIST, Fashion-MNIST, and EMNIST). The framework further demonstrates reproducibility, parameter efficiency, and interpretability through multi-seed evaluation, parameter analysis, and latent/quantum feature inspection. The source code is publicly available at [github.com/Dilli822/SimAM-HVQC](https://github.com/Dilli822/SimAM-HVQC).

## Architecture

Overview of the proposed SimAM-HVQC framework. The input image is first refined using the parameter-free SimAM attention module, followed by a classical feature extractor that compresses the representation into an 8-dimensional latent vector. The compressed features are encoded into an 8-qubit Variational Quantum Circuit (VQC) composed of six strongly entangling layers. Pauli-Z expectation measurements are subsequently processed by a lightweight classifier to generate the final class prediction.

![1788071048055](<images/Hybrid VQC.png>)

## Features

- Parameter-free SimAM attention mechanism.
- Hybrid quantum-classical architecture.
- 8-qubit Variational Quantum Circuit.
- Multi-class image classification framework.
- Multi-dataset evaluation.
- Reproducibility analysis with multiple random seeds.
- Efficiency assessment through latency and throughput measurements.
- Interpretability through latent and quantum feature analysis.

## Results

| Dataset       | Accuracy (%)  |
| ------------- | ------------- |
| MNIST         | 97.57 ± 0.05 |
| Fashion-MNIST | 87.98 ± 0.08 |
| KMNIST        | 88.20 ± 0.61 |
| EMNIST        | 80.16 ± 0.17 |

## Efficiency

| Metric             | Value             |
| ------------------ | ----------------- |
| Parameters         | 236,258           |
| Quantum Parameters | 144               |
| Latency            | 0.8124 ms/sample  |
| Throughput         | 1230.85 samples/s |

## Citation

```bibtex
@inproceedings{rai2026simamhvqc,
  title={Hybrid Variational Quantum-Classical Framework with Adaptive Weighting and Efficiency Assessment},
  author={Dilli Hang Rai},
  year={2026}
}
```
