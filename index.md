---
layout: default
---

# About Assemblage

Assemblage is a dataset of x86-64 ELF and Windows PE executables, along with a cloud-based distributed system for building large, diverse corpora of binaries.

Assemblage's high-level design looks like this:

![Assemblage's high-level system design](/assets/images/assemblage-design.png){:width="500"}


## Dataset Snapshot

Our dataset was initially released in March 2024 and looks roughly like this:

| Source  | Platform | License  | Total | Repositories | Functions |
|---------|----------|----------|-------|--------------|-----------|
| GitHub  | Windows  | Mixed    | 890k  | 172k         | 298M      |
|         |          | Licensed | 62k   | 12k          | 38M       |
|         | Linux    | Mixed    | 428k  | 48k          | 316M      |
|         |          | Licensed | 211k  | 13k          | 186M      |
| vcpkg   | Windows  | Licensed | 29k   | 1k           | 48M       |

<br>

As of May 2026, the public dataset has been updated with the latest statistics:

| Source       | Platform      | License  | Total | Repositories | Functions |
|--------------|---------------|----------|-------|--------------|-----------|
| GitHub       | Windows       | Licensed | 890k  | 172k         | 298M      |
|              | Linux         | Licensed | 249k  | 16k          | 613M      |
| vcpkg        | Windows       | Licensed | 29k   | 1k           | 48M       |
| GitHub       | Windows/Linux | Licensed | 73k   | 248          | 441M      |



## Publicly-Hosted Snapshots

- For dataset access and docs, please refer to [Assemblage Docs](https://assemblagedocs.readthedocs.io).
- Starting in May 2026, we will only update datasets hosted on Hugging Face due to Kaggle’s data size limitations.
- Starting in May 2026, we will migrate from SQLite to DuckDB for improved durability and performance.


## GitHub Repo

Assemblage's public source is kept [here](https://github.com/Assemblage-Dataset/Assemblage), please report bugs via GitHub Issues.

## Contact Us

To contact us about datasets access, deployment, or any other questions, please email current maintainers by:

- Kristopher Micinski: kkmicins@syr.edu 
- Chang Liu: cliu57@syr.edu 

Here are the email addresses of all contributors to this project (sorted by last name):

- Naveen Ashok: nashok@syr.edu
- Alex Duly: apduly@syr.edu
- Maya Fuchs: fuchs_maya@bah.com
- James Holt: holt@lps.umd.edu
- Mia Kerchen: mhkerche@syr.edu
- Chang Liu: cliu57@syr.edu
- Kristopher Micinski: kkmicins@syr.edu 
- Townsend Southard Pantano: tgsoutha@syr.edu
- Edward Raff: Raff.Edward@gmail.com
- Rebecca Saul: Saul_Rebecca@bah.com
- Yihao Sun: ysun67@syr.edu


Please reach out if you are using the Assemblage dataset for your work
or would be interested in chatting about your usage apropos binary
analysis. If you find our dataset useful, we'd appreciate a [citation](https://proceedings.neurips.cc/paper_files/paper/2024/hash/6bbefc73a187dd42e0dc065b4e7a0615-Abstract-Datasets_and_Benchmarks_Track.html).