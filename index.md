---
layout: default
---

Assemblage is both a dataset (of x86-64 ELF and Windows PE
executables) and a cloud-based distributed system for building large,
diverse, corpuses of binaries. Assemblage runs continuously on AWS,
crawling GitHub for available repositories (of C and C++ code, for
now) and then configuring, diversifying (across compiler / flag
variant), and building binary artifacts. To date, Assemblage has built
over 890k Windows PE binaries, along with 428k Linux ELF binaries.

Assemblage's high-level design looks like this:

![Assemblage's high-level system design](/assets/images/assemblage-design.png){:width="600"}


## March '24 Dataset Snapshot

As of March '24, our dataset looks roughly like this (see our [datasheet](/assets/dataset-total.pdf) for more information):

| Source  | Platform | License  | Total | Repositories | Functions | Functions (w/ source code) |
|---------|----------|----------|-------|--------------|-----------|-----------------------------|
| GitHub  | Windows  | Mixed    | 890k  | 172k         | 298M      | 20M                         |
|         |          | Licensed | 62k   | 12k          | 38M       | 3M                          |
|         | Linux    | Mixed    | 428k  | 48k          | 316M      | N/A                         |
|         |          | Licensed | 211k  | 13k          | 186M      | N/A                         |
| vcpkg   | Windows  | Licensed | 29k   | 1k           | 48M       | N/A                         |

## Publicly-Hosted Snapshots

We are currently hosting on AWS, please contact us is you plan to
consume large amounts of bandwidth.

We include only the subset of binaries for which permissive licenses can be ascertained.

PDB files are too large to be included in our publicly-hosted
repositories; datasets with pdb files are also available upon request.

1. 62k Windows PE Binaries (Processed to SQLite database, last updated: Apr 14th 2024):

- SQLite databse (12G):
  - [https://assemblage-lps.s3.us-west-1.amazonaws.com/public/winpe_licensed.sqlite.zip](https://assemblage-lps.s3.us-west-1.amazonaws.com/public/winpe_licensed.sqlite.zip)

- Binary dataset (7G):
  - [https://assemblage-lps.s3.us-west-1.amazonaws.com/public/winpe_licensed.zip](https://assemblage-lps.s3.us-west-1.amazonaws.com/public/winpe_licensed.zip)

2.Windows vcpkg dataset (Processed to SQLite database, 29k):

- SQLite database (3.3GB):
  - [https://assemblage-lps.s3.us-west-1.amazonaws.com/public/vcpkg.sqlite.zip](https://assemblage-lps.s3.us-west-1.amazonaws.com/public/vcpkg.sqlite.zip)

- Binary dataset (18G):
  - [https://assemblage-lps.s3.us-west-1.amazonaws.com/public/vcpkg.zip](https://assemblage-lps.s3.us-west-1.amazonaws.com/public/vcpkg.zip)

3.Linux GitHub dataset (Processed to SQLite database, 211k):

- SQLite database (23M):
  - [https://assemblage-lps.s3.us-west-1.amazonaws.com/public/feb15_linux_licensed.sqlite](https://assemblage-lps.s3.us-west-1.amazonaws.com/public/feb15_linux_licensed.sqlite)

- Binary dataset (72G):
  - [https://assemblage-lps.s3.us-west-1.amazonaws.com/public/licensed_linux.zip](https://assemblage-lps.s3.us-west-1.amazonaws.com/public/licensed_linux.zip)

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
