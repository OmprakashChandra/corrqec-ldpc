# CorrQEC
Repository containing code and data for *Detrimental non-Markovian errors for surface code memory*.

## Links and abstract

DOI: https://iopscience.iop.org/article/10.1088/2058-9565/adebab \
arXiv: https://arxiv.org/abs/2410.23779 

Abstract:
>The realization of fault-tolerant quantum computers hinges on effective quantum error correction protocols, whose performance significantly relies on the nature of the underlying noise. In this work, we directly study the structure of non-Markovian correlated errors and their impact on surface code memory performance. Specifically, we compare surface code performance under non-Markovian noise and independent circuit-level noise, while keeping marginal error rates constant. Our analysis shows that while not all temporally correlated structures are detrimental, certain structures, particularly multi-time "streaky" correlations affecting syndrome qubits and two-qubit gates, can severely degrade logical error rate scaling. Furthermore, we discuss our results in the context of recent quantum error correction experiments on physical devices. These findings underscore the importance of understanding and mitigating non-Markovian noise toward achieving practical, fault-tolerant quantum computing.

## Usage
Install requirements into a fresh Python environment via pip (in project root).
```
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

Run experiment scripts, for example:
```
python -m scripts.experiment1.class0
python -m scripts.experiment1.class1
python -m scripts.experiment1.class2
python -m scripts.experiment1.figures
```
Also see [`script_commands.txt`](https://github.com/jkfids/corrqec/main/script_commands.txt).

## Repository overview

- `src`: Source code containing noise models, simulation, data analysis and visualisation tools.
- `scripts`: Scripts to reproduce (simulation and plotting) the main results.
- `tests`: Basic tests mainly to test for correct marginalization of correlated noise models.
- `data/saved`: Saved data used to generate figures in paper.
- `notebooks`: Jupyter notebooks related to correlation matrices.

## Citation

BibTeX:
```
@article{F Kam_2025,
doi = {10.1088/2058-9565/adebab},
url = {https://doi.org/10.1088/2058-9565/adebab},
year = {2025},
month = {jul},
publisher = {IOP Publishing},
volume = {10},
number = {3},
pages = {035060},
author = {F Kam, John and Gicev, Spiro and Modi, Kavan and Southwell, Angus and Usman, Muhammad},
title = {Detrimental non-Markovian errors for surface code memory},
journal = {Quantum Science and Technology}
```
RIS: See IOP QST [page](https://iopscience.iop.org/article/10.1088/2058-9565/adebab).


## Contact

Email: john.kam@monash.edu

## License
MIT license in [`LICENSE`](https://github.com/jkfids/corrqec/main/LICENSE).