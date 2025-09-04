# BACE-1 inhibition

Prediction of Beta-secretase 1 (BACE-1) inhibition. BACE-1 is expressed mainly in neurons and has been involved in the development of Alzheimers disease. This model has been trained on the BACE dataset from MoleculeNet using the GROVER transformer (see eos7w6n or grover-embedding for a detail of the molecular featurization step with GROVER). 

This model was incorporated on 2022-07-13.


## Information
### Identifiers
- **Ersilia Identifier:** `eos2mhp`
- **Slug:** `grover-bace`

### Domain
- **Task:** `Annotation`
- **Subtask:** `Activity prediction`
- **Biomedical Area:** `Alzheimer`
- **Target Organism:** `Homo sapiens`
- **Tags:** `Alzheimer`, `BACE`, `MoleculeNet`, `Chemical graph model`

### Input
- **Input:** `Compound`
- **Input Dimension:** `1`

### Output
- **Output Dimension:** `1`
- **Output Consistency:** `Fixed`
- **Interpretation:** Probability that the molecule is a BACE-1 inhibitor (using a 0.1 uM cut-off)

Below are the **Output Columns** of the model:
| Name | Type | Direction | Description |
|------|------|-----------|-------------|
| bace_inhibition | float | high | Probability of inhibiting the BACE1 protein |


### Source and Deployment
- **Source:** `Local`
- **Source Type:** `External`
- **DockerHub**: [https://hub.docker.com/r/ersiliaos/eos2mhp](https://hub.docker.com/r/ersiliaos/eos2mhp)
- **Docker Architecture:** `AMD64`, `ARM64`
- **S3 Storage**: [https://ersilia-models-zipped.s3.eu-central-1.amazonaws.com/eos2mhp.zip](https://ersilia-models-zipped.s3.eu-central-1.amazonaws.com/eos2mhp.zip)

### Resource Consumption
- **Model Size (Mb):** `1378`
- **Environment Size (Mb):** `2422`
- **Image Size (Mb):** `6480.94`

**Computational Performance (seconds):**
- 10 inputs: `49.76`
- 100 inputs: `446.15`
- 10000 inputs: `-1`

### References
- **Source Code**: [https://github.com/tencent-ailab/grover](https://github.com/tencent-ailab/grover)
- **Publication**: [https://arxiv.org/abs/2007.02835](https://arxiv.org/abs/2007.02835)
- **Publication Type:** `Preprint`
- **Publication Year:** `2020`
- **Ersilia Contributor:** [Amna-28](https://github.com/Amna-28)

### License
This package is licensed under a [GPL-3.0](https://github.com/ersilia-os/ersilia/blob/master/LICENSE) license. The model contained within this package is licensed under a [MIT](LICENSE) license.

**Notice**: Ersilia grants access to models _as is_, directly from the original authors, please refer to the original code repository and/or publication if you use the model in your research.


## Use
To use this model locally, you need to have the [Ersilia CLI](https://github.com/ersilia-os/ersilia) installed.
The model can be **fetched** using the following command:
```bash
# fetch model from the Ersilia Model Hub
ersilia fetch eos2mhp
```
Then, you can **serve**, **run** and **close** the model as follows:
```bash
# serve the model
ersilia serve eos2mhp
# generate an example file
ersilia example -n 3 -f my_input.csv
# run the model
ersilia run -i my_input.csv -o my_output.csv
# close the model
ersilia close
```

## About Ersilia
The [Ersilia Open Source Initiative](https://ersilia.io) is a tech non-profit organization fueling sustainable research in the Global South.
Please [cite](https://github.com/ersilia-os/ersilia/blob/master/CITATION.cff) the Ersilia Model Hub if you've found this model to be useful. Always [let us know](https://github.com/ersilia-os/ersilia/issues) if you experience any issues while trying to run it.
If you want to contribute to our mission, consider [donating](https://www.ersilia.io/donate) to Ersilia!
