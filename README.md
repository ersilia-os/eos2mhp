# BACE-1 inhibition
## Model identifiers
- Slug: grover-bace
- Ersilia ID: eos2mhp
- Tags: Alzheimer, Target, BACE, MoleculeNet

# Model description
Prediction of BACE-1 inhibition, related to Alzheimer's disease.
- Input: SMILES
- Output: Alzheimer, Target
- Model type: Classification
- Training set: 10,000,000 (https://paperswithcode.com/dataset/moleculenet)
- Mode of training: Pretrained

# Source code
This model was published by Yu R., Yatao B. et al. Self-Supervised Graph Transformer on Large-Scale Molecular Data. arXiv Labs 2018. DOI: https://doi.org/10.48550/arXiv.2007.02835

- Code: https://github.com/tencent-ailab/grover
- Checkpoints: https://github.com/tencent-ailab/grover/tree/main/grover/model

# License
The GPL-v3 license applies to all parts of the repository that are not externally maintained libraries. This repository uses the externally maintained library "grover", located at /model and licensed under an MIT license

# History 
- Model was downloaded on 12.05.21 from TencentAILab
- We duplicated task/predict.py and scripts/save_features.py from Tencent GitHub repository
- Model was incorporated to Ersilia on 12/05/2021
