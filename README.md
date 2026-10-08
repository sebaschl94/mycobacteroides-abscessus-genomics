# Mycobacteroides abscessus Genomic Analysis

Bioinformatic analysis of two *Mycobacteroides abscessus* genomic samples,
1651 and 1783.

## Samples

| Sample | Assembly size | Estimated coverage | Contigs |
|---|---:|---:|---:|
| 1651 | 5,048,032 bp | 99.0% | 78 |
| 1783 | 4,934,846 bp | 96.8% | Not determined |

## Analysis workflow

Illumina MiSeq
→ Quality control
→ Unicycler genome assembly
→ Taxonomic identification
→ MLST / rMLST
→ Subspecies analysis
→ erm(41) analysis
→ Antimicrobial resistance analysis with ABRicate/CARD

## Repository structure

- `assembly/` — genome assemblies and Unicycler logs
- `mlst/` — MLST results
- `taxonomy/` — taxonomic and rMLST results
- `amr/` — antimicrobial resistance results
- `subspecies/` — subspecies and erm(41) analysis
- `metadata/` — sample metadata
- `scripts/` — analysis scripts
- `environment/` — software versions
- `report/` — reports and summaries

## Taxonomic identification

Sample 1651 was identified by rMLST as:

**Mycobacteroides abscessus**

Taxonomic lineage:

Actinomycetota > Actinomycetes > Mycobacteriales >
Mycobacteriaceae > Mycobacteroides > Mycobacteroides abscessus

The rMLST results for both samples are available in `taxonomy/rmlst/`.

## MLST

MLST results are available under `mlst/`.

Sample 1651 was analyzed using the `mycobacteria_2` scheme.

## Antimicrobial resistance

Resistance screening was performed using ABRicate with the CARD database.

Results are available under:

`amr/abricate/`

and

`amr/card/`

## Subspecies and erm(41)

Sequence files used for subspecies characterization and `erm(41)` analysis
are available under:

`subspecies/`

## Raw sequencing data

Original Illumina FASTQ files are not included because of file size.

## Reproducibility

Software versions, commands, logs and analysis scripts will be documented
in this repository as the analysis progresses.

## Project status

Current repository contains the genomic analysis results generated for
samples 1651 and 1783.
