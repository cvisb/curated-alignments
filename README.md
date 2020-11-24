## Curated alignments

We periodically combine genomic sequences generated as part of our consortium with publicly available sequences. Our curated alignments do not include:

   - laboratory strains (adapted, passaged, recombinant, antiviral & vaccine experiments)

   - sequences without a timestamp

   - subsequent timepoints, if multiple timepoints are available

   - duplicates (when more than one sequence is available for a single strain)


Remaining sequences are trimmed to their coding regions, aligned using [mafft](https://mafft.cbrc.jp/alignment/software/tips0.html) and inspected manually. At this step we discard:

  - low quality sequences (manual curation)

  - incomplete sequences (<95% of (NP+GPC) or (L+Z) or (NP+VP35+VP40+GP+VP30+VP24+L) ORFs length)


ORFs are arranged in sense orientation as follows:

Lassa S segment: NP -NNN- GPC

Lassa L segment: L -NNN- Z

Ebola: NP -NNN- VP35 -NNN- VP40 -NNN- GP -NNN- VP30 -NNN- VP24 -NNN- L


For each alignment, a maximum likelihood (ML) phylogeny is reconstructed with RAxML using the general time-reversible (GTR) nucleotide substitution model, gamma-distributed rates among sites and bootstrap resampling with 500 (LASV) or 100 (EBOV) replicates.

We will be releasing such curated alignments periodically to be used by the broader community for downstream analyses.

## Lassa S segment

Alignment File: [LASV_NP_GPC_2020.11.23.fasta](https://github.com/cvisb/curated-alignments/blob/master/lassa/LASV_NP_GPC_2020.11.23.fasta)

Total Number of sequences: 652

FASTA header format:
```
> GenBank Accession | Species | Outcome | Country | Date
```
ML Tree file: In progress...

Key:

Species

| Code | Species | Count |
|:---|:---|:---|
| Hs | *Homo sapiens* | 608 |
| Hp | *Hylomyscus pamfi* | 1 |
| Me | *Mastomys erythroleucus* | 9 |
| Mn | *Mastomys natalensis* | 32 |
| Unk | *Unknown* | 2 |

Country

| Code | Country | Count |
|:--|:--|:--|
| BEN | Benin | 11 |
| CIV | Ivory Coast | 13 |
| GHA | Ghana | 1 |
| GIN | Guinea | 11 |
| LBR | Liberia | 25 |
| MLI | Mali | 5 |
| NGA | Nigeria | 481 |
| SLE | Sierra Leone | 103 |
| TGO | Togo | 2 |

Outcome

|Code | Outcome | Count |
|:-- |:-- |:-- |
| Died | Died | 129 |
| Discharged | Discharged | 96 |
| Unk | Unknown | 427 |

## Lassa L segment

Alignment File: [LASV_L_Z_2020.11.23.fasta](https://github.com/cvisb/curated-alignments/blob/master/lassa/LASV_L_Z_2020.11.23.fasta)

Total Number of sequences: 520

FASTA header format:
```
> GenBank Accession | Species | Outcome | Country | Date
```
ML Tree file: In progress ...

Key:

Species

| Code | Species | Count |
|:---|:---|:---|
| Hs | *Homo sapiens* | 480 |
| Hp | *Hylomyscus pamfi* | 1 |
| Me | *Mastomys erythroleucus* | 9 |
| Mn | *Mastomys natalensis* | 28 |
| Unk | *Unknown* | 2 |

Country

| Code | Country | Count |
|:--|:--|:--|
| BEN | Benin | 10 |
| CIV | Ivory Coast | 13 |
| GHA | Ghana | 1 |
| GIN | Guinea | 11 |
| LBR | Liberia | 22 |
| MLI | Mali | 3 |
| NGA | Nigeria | 381 |
| SLE | Sierra Leone | 77 |
| TGO | Togo | 2 |

Outcome

|Code | Outcome | Count |
|:-- |:-- |:-- |
| Died | Died | 113 |
| Discharged | Discharged | 79 |
| UNK | Unknown | 328 |

## Ebola

Alignment File: [EBOV_ORFs_2020.08.04.fasta](https://github.com/cvisb/curated-alignments/blob/master/ebola/EBOV_ORFs_2020.08.04.fasta)

Total Number of sequences: 2684

FASTA header format:
```
> GenBank Accession | Species | Outcome | Country | Date
```
ML Tree file: In progress ...

Key:

Species

| Code | Species | Count |
|:---|:---|:---|
| Hs | *Homo sapiens* | 2684 |

Country

| Code | Country | Count |
|:--|:--|:--|
| COD | Democratic Republic of the Congo | 704 |
| COG | Republic of the Congo | 2 |
| GAB | Gabon | 7 |
| GIN | Guinea | 346 |
| LBR | Liberia | 242 |
| MLI | Mali | 4 |
| NGA | Nigeria | 11 |
| SLE | Sierra Leone | 1362 |
| Unk | Unknown | 5 |
| USA | United States | 1 |

Outcome

|Code | Outcome | Count |
|:-- |:-- |:-- |
| Died | Died | 384 |
| Discharged | Discharged | 151 |
| Unk | Unknown | 2149 |

---
**Andersen Lab**  
The Scripps Research Institute  
La Jolla, CA, USA  
[data@andersen-lab.com](mailto:data@andersen-lab.com)
