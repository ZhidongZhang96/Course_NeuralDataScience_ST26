# Repository for Neural Data Science


Coding lab for 'Neural Data Science 2026' in GTC, Tübingen.

The labs were completed as a group (with **[@Yuzhe Han](https://github.com/Hzzz12138)** and **[@Bach Nguyen](https://github.com/bachnguyenTE)**), through individual coding and panel discussions. This repository contains the version initialized by **[@Zhidong Zhang](https://github.com/ZhidongZhang96)**.

> Data in the folder `data/` are not included due to GitHub size limits. 

The notebooks are stored in the folder `notebooks/`; their contents are as follows:

| Notebook| Content|
|:--:|:---:|
|1|Spike detection & feature extraction (PCA)|
|2|Spike sorting (clustering and correlograms)|
|3|2-photon calcium recordings to spike trains|
|4|Spike trains & tuning curve|
|5|Receptive field|
|6|Latent variable model (Poisson GPFA)|
|7|Transcriptomics|
|8|Neural Morphologies (statistics & density maps)|



## Instructions

To work in this repository install the required dependencies and tools by running `setup.sh`.
This sets up the correct folders initializes a git repository, installs `pre-commit` hooks, conda / python packages and configures git to use `nbdime`.


You can also do all of this manually of course.

```bash
conda env create -f environment.yml
```

or via

```bash
python3 -m pip install -r requirements.txt
```

Set up git.

```bash
git init
```

`pre-commit` hooks for working with notebooks can be installed with 

```bash
pre-commit install
```

Set up `nbdime`.
```bash
nbdime config-git --enable
```

> The `pre-commit` notebook hook activates the `nds_env` conda environment before running `nbdev_clean`. (edition on `run_nbdev_on_staged_files.sh`)

