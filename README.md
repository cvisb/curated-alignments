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


For each alignment, a maximum likelihood (ML) phylogeny is reconstructed with IQ-TREE with ultrafast bootstrap approximation (1000 replicates).

We will be releasing such curated alignments periodically to be used by the broader community for downstream analyses.

## Lassa S segment

Alignment File: [LASV_NP_GPC_2020.11.23.fasta](https://github.com/cvisb/curated-alignments/blob/master/lassa/LASV_NP_GPC_2020.11.23.fasta)

Total Number of sequences: 690

FASTA header format:
```
> GenBank Accession | Species | Outcome | Country | Date
```
ML Tree file: in progress...

Key:

Species

| Code | Species | Count |
|:---|:---|:---|
| Hs | *Homo sapiens* | 624 |
| Hp | *Hylomyscus pamfi* | 1 |
| Me | *Mastomys erythroleucus* | 9 |
| Mn | *Mastomys natalensis* | 54 |
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
| NGA | Nigeria | 486 |
| SLE | Sierra Leone | 136 |
| TGO | Togo | 2 |

Outcome

|Code | Outcome | Count |
|:-- |:-- |:-- |
| Died | Died | 134 |
| Discharged | Discharged | 97 |
| Unk | Unknown | 459 |

## Lassa L segment

Alignment File: [LASV_L_Z_2020.11.23.fasta](https://github.com/cvisb/curated-alignments/blob/master/lassa/LASV_L_Z_2020.11.23.fasta)

Total Number of sequences: 534

FASTA header format:
```
> GenBank Accession | Species | Outcome | Country | Date
```
ML Tree file: in progress...

Key:

Species

| Code | Species | Count |
|:---|:---|:---|
| Hs | *Homo sapiens* | 486 |
| Hp | *Hylomyscus pamfi* | 1 |
| Me | *Mastomys erythroleucus* | 9 |
| Mn | *Mastomys natalensis* | 36 |
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
| NGA | Nigeria | 386 |
| SLE | Sierra Leone | 86 |
| TGO | Togo | 2 |

Outcome

|Code | Outcome | Count |
|:-- |:-- |:-- |
| Died | Died | 114 |
| Discharged | Discharged | 79 |
| UNK | Unknown | 341 |

## Ebola

Alignment File: [EBOV_ORFs_2020.08.04.fasta](https://github.com/cvisb/curated-alignments/blob/master/ebola/EBOV_ORFs_2020.08.04.fasta)

Total Number of sequences: 2790

FASTA header format:
```
> GenBank Accession | Species | Outcome | Country | Date
```
ML Tree file: in progress...

Key:

Species

| Code | Species | Count |
|:---|:---|:---|
| Hs | *Homo sapiens* | 2790 |

Country

| Code | Country | Count |
|:--|:--|:--|
| COD | Democratic Republic of the Congo | 801 |
| COG | Republic of the Congo | 2 |
| GAB | Gabon | 7 |
| GIN | Guinea | 354 |
| LBR | Liberia | 243 |
| MLI | Mali | 4 |
| NGA | Nigeria | 11 |
| SLE | Sierra Leone | 1362 |
| Unk | Unknown | 6 |
| USA | United States | 1 |

Outcome

|Code | Outcome | Count |
|:-- |:-- |:-- |
| Died | Died | 384 |
| Discharged | Discharged | 151 |
| Unk | Unknown | 2255 |

---
**Andersen Lab**  
The Scripps Research Institute  
La Jolla, CA, USA  
[data@andersen-lab.com](mailto:data@andersen-lab.com)
