# BLAST Run Example

**Download Genome FASTA File**
- For this example, I will be using the Mus musculus genome GRCm39 from NCBI
  ```sh
   wget https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/001/635/GCF_000001635.27_GRCm39/GCF_000001635.27_GRCm39_genomic.fna.gz
   gunzip GCF_000001635.27_GRCm39_genomic.fna.gz

**Create a BLAST Database from your Genome Sequence FASTA**
```sh
makeblastdb -in GCF_000001635.27_GRCm39_genomic.fna -dbtype nucl -input_type fasta -out MusMusculus

**Run BLAST Command Using Database and Query Sequence**
```sh
blastn -db MusMusculus -query sample_mouse_genes.fasta -out blastout.txt
