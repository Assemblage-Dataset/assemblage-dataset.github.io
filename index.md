---
layout: default
---

# About Assemblage

Assemblage is a dataset of x86-64 Linux ELF and Windows PE executables built from open-source C/C++ and Rust projects, along with a cloud-based distributed system for building large, diverse corpora of binaries.

<div class="arch">
  <figure>
    <img src="/assets/images/assemblage-design.png" alt="Assemblage's high-level system design" width="465">
    <figcaption>A coordinator dispatches GitHub repositories to a pool of build workers over RabbitMQ, and the resulting binaries and metadata are stored for export.</figcaption>
  </figure>
</div>

## Datasets

All datasets are hosted on Hugging Face (the Kaggle copies are no longer updated) and contain only licensed code. For download instructions, schemas, and changelogs, see the [Assemblage Docs](https://assemblagedocs.readthedocs.io/en/latest/dataset.html).

{% include dataset-cards.html %}

## GitHub Repo

Assemblage's public source is released [on GitHub](https://github.com/Assemblage-Dataset/Assemblage), please report bugs via GitHub Issues.

## Contact Us

For dataset access, deployment, or any other questions, email the maintainers. We'd also love to hear how you use Assemblage in your binary analysis work.

{% include contact.html %}

## Cite

If you find our dataset useful, we'd appreciate a citation.

{% include cite.html %}
