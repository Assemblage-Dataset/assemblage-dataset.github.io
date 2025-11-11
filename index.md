---
layout: default
---


Assemblage is both a dataset (of x86-64 ELF and Windows PE
executables) and a cloud-based distributed system for building large,
diverse, corpuses of binaries. Assemblage runs continuously on AWS,
crawling GitHub for available repositories (of C and C++ code, for
now) and then configuring, diversifying (across compiler / flag
variants), and building binary artifacts. To date, Assemblage has
built over 890k Windows PE binaries, along with 428k Linux ELF
binaries.

Assemblage's high-level design looks like this:

![Assemblage's high-level system design](/assets/images/assemblage-design.png){:width="600"}


## March '24 Dataset Snapshot

As of March '24, our dataset looks roughly like this (see our [datasheet](https://assemblage-dataset.net/assets/total-datasheet.pdf) for more information):

| Source  | Platform | License  | Total | Repositories | Functions | Functions (w/ source code) |
|---------|----------|----------|-------|--------------|-----------|-----------------------------|
| GitHub  | Windows  | Mixed    | 890k  | 172k         | 298M      | 20M                         |
|         |          | Licensed | 62k   | 12k          | 38M       | 3M                          |
|         | Linux    | Mixed    | 428k  | 48k          | 316M      | N/A                         |
|         |          | Licensed | 211k  | 13k          | 186M      | N/A                         |
| vcpkg   | Windows  | Licensed | 29k   | 1k           | 48M       | N/A                         |

## Publicly-Hosted Snapshots

Here we include only the subset of binaries for which permissive
licenses can be ascertained. Please contact us if you would like
recipes for unlicensed repositories. PDB files are too large to be
included in our publicly-hosted repositories; datasets with PDB files
are also available upon request.

Each dataset is broken up into both (a) an SQLite file, which includes
metadata, and (b) a dump of the binaries themselves. Please see our
[datasheet](/assets/dataset-total.pdf) for a description of database
organization. We are working on additional tutorials now, please reach
out if you are interested in specific types of queries.

For dataset usage and docs, please refer to [Assemblage Docs](https://assemblagedocs.readthedocs.io). 
We are currently hosting the public dataset on Kaggle and Hugging Face (datasets hosted on these platforms are the same)

1. Windows PE Binaries:

- [Kaggle](https://www.kaggle.com/datasets/changliuh7rfs5/assemblagedataset)
- [Hugging Face](https://huggingface.co/datasets/changliu8541/Assemblage_PE)

2.Windows vcpkg dataset:

- [Kaggle](https://www.kaggle.com/datasets/changliuh7rfs5/assemblage-vcpkg)
- [Hugging Face](https://huggingface.co/datasets/changliu8541/Assemblage_vcpkgDLL)
 
3.Linux GitHub dataset:

- [Kaggle](https://www.kaggle.com/datasets/changliuh7rfs5/assemblagelinux)
- [Hugging Face](https://huggingface.co/datasets/changliu8541/Assemblage_LinuxELF)


## GitHub Repo / Bug Reports

Assemblage's public source is kept
[here](https://github.com/Assemblage-Dataset/Assemblage). 

Please report bugs via GitHub.

## Contact Us / Citations

Assemblage is primarily developed at Syracuse University, by a team
that includes:

- Chang Liu, cliu57@syr.edu, Syracuse University (PhD student)
- Yihao Sun, ysun67@syr.edu, Syracuse University (PhD student)
- Kristopher Micinski, kkmicins@syr.edu Asst. Prof @ Syracuse University

Please reach out if you are using the Assemblage dataset for your work
or would be interested in chatting about your usage apropos binary
analysis.


Please cite our Arxiv draft (link forthcoming).
