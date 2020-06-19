## Curated alignments

We periodically combine genomic sequences generated as part of our consortium with publicly available sequences. Our curated alignments do not include:

   - laboratory strains (adapted, passaged, recombinant, antiviral & vaccine experiments)

   - sequences without a timestamp

   - subsequent timepoints, if multiple timepoints are available

   - duplicates (when more than one sequence is available for a single strain)

   - sequences from identified hospital epidemics (Lassa dataset only)


Remaining sequences are trimmed to their coding regions, codon aligned using [mafft](https://mafft.cbrc.jp/alignment/software/tips0.html) and inspected manually. At this step we discard:

  - low quality sequences (manual curation)

  - incomplete sequences (<95% of (GP+NP) or (Z+L) or (NP+VP35+VP40+GP+VP30+VP24+L) ORFs length)


ORFs are arranged in sense orientation as follows:

Lassa S segment: NP -NNN- GP

Lassa L segment: L -NNN- Z

Ebola: NP -NNN- VP35 -NNN- VP40 -NNN- GP -NNN- VP30 -NNN- VP24 -NNN- L


For each alignment, a maximum likelihood (ML) phylogeny is reconstructed with RAxML using the general time-reversible (GTR) nucleotide substitution model, gamma-distributed rates among sites and bootstrap resampling with 500 replicates.

We will be releasing such curated alignments periodically to be used by the broader community for downstream analyses.

## Lassa S segment

Alignment File: [LASV_NP_GPC_2019.11.21.fasta](https://github.com/cvisb/curated-alignments/blob/master/lassa/LASV_NP_GPC_2019.11.21.fasta)

Total Number of sequences: 632

FASTA header format:
```
> GenBank Accession | Species | Outcome | Country | Date
```
ML Tree file:


![LASV_NP_GPC_2019.11.27.png](https://github.com/cvisb/curated-alignments/blob/master/lassa/LASV_NP_GPC_2019.11.27.png)

Key:

Species

| Code | Species | Count |
|:---|:---|:---|
| Hs | *Homo sapiens* | 589 |
| Hp | *Hylomyscus pamfi* | 1 |
| Me | *Mastomys erythroleucus* | 9 |
| Mn | *Mastomys natalensis* | 31 |
| Unk | *Unknown* | 2 |

Country

| Code | Country | Count |
|:--|:--|:--|
|CIV | Ivory Coast | 13 |
|GHA | Ghana | 1 |
|GIN | Guinea | 11 |
| LBR | Liberia | 24 |
| MLI | Mali | 5 |
| NGA | Nigeria | 481 |
| SLE | Sierra Leone | 95 |
| TGO | Togo | 2 |

Outcome

|Code | Outcome | Count |
|:-- |:-- |:-- |
| Died | Died | 119 |
| Discharged | Discharged | 90 |
| Unk | Unknown | 423 |

## Lassa L segment

Alignment File: [LASV_L_Z_2019.11.22.fasta](https://github.com/cvisb/curated-alignments/blob/master/lassa/LASV_L_Z_2019.11.22.fasta)

Total Number of sequences: 508

FASTA header format:
```
> GenBank Accession | Species | Outcome | Country | Date
```
ML Tree file:

![LASV_L_Z_2019.11.27.png](https://github.com/cvisb/curated-alignments/blob/master/lassa/LASV_L_Z_2019.11.27.png)

Key:

Species

| Code | Species | Count |
|:---|:---|:---|
| Hs | *Homo sapiens* | 469 |
| Hp | *Hylomyscus pamfi* | 1 |
| Me | *Mastomys erythroleucus* | 9 |
| Mn | *Mastomys natalensis* | 28 |
| Unk | *Unknown* | 1 |

Country

| Code | Country | Count |
|:--|:--|:--|
|CIV | Ivory Coast | 13 |
|GHA | Ghana | 1 |
|GIN | Guinea | 11 |
| LBR | Liberia | 20 |
| MLI | Mali | 3 |
| NGA | Nigeria | 381 |
| SLE | Sierra Leone | 77 |
| TGO | Togo | 2 |

Outcome

|Code | Outcome | Count |
|:-- |:-- |:-- |
| Died | Died | 106 |
| Discharged | Discharged | 76 |
| UNK | Unknown | 326 |

## Ebola

Alignment File: [EBOV_ORFs_2020.06.12.fasta](https://github.com/cvisb/curated-alignments/blob/master/ebola/EBOV_ORFs_2020.06.12.fasta)

Total Number of sequences: 2079

FASTA header format:
```
> GenBank Accession | Species | Outcome | Country | Date
```
ML Tree file: in progress...

![EBOV_ORFS_tree_2020.06.16.png](https://github.com/cvisb/curated-alignments/blob/master/ebola/previous_versions/EBOV_ORFS_tree_2020.06.16.png)

Key:

Species

| Code | Species | Count |
|:---|:---|:---|
| Hs | *Homo sapiens* | 2079 |

Country

| Code | Country | Count |
|:--|:--|:--|
| CHE | Switzerland | 1 |
| COD | Democratic Republic of the Congo | 98 |
| COG | Republic of the Congo | 2 |
| DEU | Germany | 1 |
| GAB | Gabon | 7 |
| GBR | United Kingdom | 4 |
| GIN | Guinea | 346 |
| ITA | Italy | 2 |
| LBR | Liberia | 242 |
| MLI | Mali | 4 |
| NGA | Nigeria | 11 |
| SLE | Sierra Leone | 1359 |
| USA | United States | 2 |

*IMP = presumed imports (CHE, DEU, GBR, ITA, USA)

Outcome

|Code | Outcome | Count |
|:-- |:-- |:-- |
| Died | Died | 384 |
| Discharged | Discharged | 151 |
| Unk | Unknown | 1544 |

---
**Andersen Lab**  
The Scripps Research Institute  
La Jolla, CA, USA  
[data@andersen-lab.com](mailto:data@andersen-lab.com)
