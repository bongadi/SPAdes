# SPAdes

#### Read Assembly
- **Why Perform Assembly?**: Once reads are cleaned and filtered, genome assembly is performed to reconstruct the entire genome or transcriptome from the sequencing reads. This process is especially crucial for de novo assemblies, where a reference genome is not available.
- **Tool (Illumina Short Reads)**: SPAdes
  - **Installation**:
    ```bash
    conda install -c bioconda spades
    ```
  - **Usage**:
    - Single-end:
      ```bash
      spades.py -s input.fastq -o output_directory
      ```
    - Paired-end:
      ```bash
      spades.py -1 input_R1.fastq -2 input_R2.fastq -o output_directory
