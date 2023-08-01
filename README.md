# BACE-1 inhibition

Prediction of Beta-secretase 1 (BACE-1) inhibition. BACE-1 is expressed mainly in neurons and has been involved in the development of Alzheimer's disease. This model has been trained on the BACE dataset from MoleculeNet using the GROVER transformer (see eos7w6n or grover-embedding for a detail of the molecular featurization step with GROVER). 

## Identifiers

* EOS model ID: `eos2mhp`
* Slug: `grover-bace`

## Characteristics

* Input: `Compound`
* Input Shape: `Single`
* Task: `Classification`
* Output: `Probability`
* Output Type: `Float`
* Output Shape: `Single`
* Interpretation: Probability that the molecule is a BACE-1 inhibitor (using a 0.1 uM cut-off)

## References

* [Publication](https://arxiv.org/abs/2007.02835)
* [Source Code](https://github.com/tencent-ailab/grover)
* Ersilia contributor: [Amna-28](https://github.com/Amna-28)

## Ersilia model URLs
* [GitHub](https://github.com/ersilia-os/eos2mhp)
* [AWS S3](https://ersilia-models-zipped.s3.eu-central-1.amazonaws.com/eos2mhp.zip)
* [DockerHub](https://hub.docker.com/r/ersiliaos/eos2mhp) (AMD64, ARM64)

## Citation

If you use this model, please cite the [original authors](https://arxiv.org/abs/2007.02835) of the model and the [Ersilia Model Hub](https://github.com/ersilia-os/ersilia/blob/master/CITATION.cff).

## License

This package is licensed under a GPL-3.0 license. The model contained within this package is licensed under a MIT license.

Notice: Ersilia grants access to these models 'as is' provided by the original authors, please refer to the original code repository and/or publication if you use the model in your research.

## About Us

The [Ersilia Open Source Initiative](https://ersilia.io) is a Non Profit Organization ([1192266](https://register-of-charities.charitycommission.gov.uk/charity-search/-/charity-details/5170657/full-print)) with the mission is to equip labs, universities and clinics in LMIC with AI/ML tools for infectious disease research.

[Help us](https://www.ersilia.io/donate) achieve our mission!