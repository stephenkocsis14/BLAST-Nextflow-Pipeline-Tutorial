# Nextflow BLAST Pipeline

This repository contains a Nextflow pipeline tutorial for running BLAST (Basic Local Alignment Search Tool) on a set of sequences. This pipeline has been adapted from open-source BLAST and Nextflow tutorials. The pipeline is designed to be modular, efficient, and easy to use, allowing you to perform sequence alignment tasks with minimal setup.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
  - [Running the Pipeline](#running-the-pipeline)
  - [Pipeline Help](#pipeline-help)

## Introduction

The Nextflow BLAST pipeline simplifies the process of running BLAST by automating the sequence alignment tasks using Nextflow. This pipeline is suitable for researchers and bioinformaticians who need to perform sequence similarity searches efficiently.

## Features

- **Automated BLAST execution**: Streamlines the process of running BLAST.
- **Modular design**: Easy to customize and extend.
- **Scalability**: Utilizes Nextflow's parallel execution capabilities.
- **Compatibility**: Supports various BLAST tools including blastn, blastp, tblastn, and blastx.

## Requirements

- [Nextflow](https://www.nextflow.io/)
- [BLAST+](https://blast.ncbi.nlm.nih.gov/Blast.cgi?PAGE_TYPE=BlastDocs&DOC_TYPE=Download)
- An internet connection (for downloading dependencies)

## Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/stephenkocsis14/BLAST-nextflow-pipeline.git
   cd BLAST-nextflow-pipeline

## Usage

1. **Running the Pipeline**
   ```sh
   nextflow run blast.nf --query input.fasta --dbDir /path/to/my/blastDB/ --dbName myBlastDB --outdir results

2. Pipeline Help
   ```sh
   nextflow run blast.nf --help

