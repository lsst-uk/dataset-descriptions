# GaiaXCatWISE

## Description
Associations between Gaia DR3 and CatWISE2020.
Uses probabilistic cross-match algorithms as described by Wilson and Naylor (MNRAS, 2017, 2018a,b) and Wilson (RNAAS, 2022).
Sources are returned either as a pairing, in which the Gaia and WISE objects are the same astrophysical source detected twice, or as non-matches, with that particular object in one of the catalogues having a corresponding flux upper limits in the opposing catalogue, and entries include various pieces of metadata such as the probability of the match/non-match, likelihood of match on purely position or brightness grounds, and information on the level to which objects suffer contamination due to hidden and unresolved background sources.

## Data Products
* **README.md**: This file.
* **GaiaXCatWISE**: Comprised of 9,348 CSV-formatted files, totalling 960 GiB
* **UK IDAC Dataset**: `macauff_gaiadr3xcatwise2020`
* **On Echo**: Files are structured, for efficient data transfer, as 422 CSV files, plus 913 ZIP files containing the remaining 8,912 CSV files, plus metadata files listing the contents of the corresponding ZIP files, giving 2,413 objects totalling 354 GiB.

## Provenance and Methodology
This was produced by running the [macauff](https://github.com/macauff/macauff) code on the Cirrus UK National Tier-2 HPC Service, using Gaia DR3 and CatWISE2020 datasets as input. The code was used at commit [SHA:f3e3d3b](https://github.com/macauff/macauff/tree/f3e3d3ba5e850058c25206459d5fe5cb98c54a79).

### 1. Source Data
| Input Entity |
| :--- |
| Gaia DR3 |
| CatWISE2020 |

### 2. Processing Activity
| Parameter | Value | Details |
| :--- | :--- | :--- |
| **Software Used** | https://github.com/macauff/macauff | https://github.com/macauff/macauff/tree/f3e3d3ba5e850058c25206459d5fe5cb98c54a79 |
| **Production Date** | 20250627T144300 |  |
| **Production System"" | https://www.cirrus.ac.uk | This work used the Cirrus UK National Tier-2 HPC Service at EPCC (http://www.cirrus.ac.uk) funded by the University of Edinburgh and EPSRC (EP/P020267/1) |
| **Dependencies** | numpy==1.26.4,scipy==1.13.1,astropy==7.0.0,matplotlib==3.9.0,skypy==0.5.3,speclite==0.20,pandas==2.2.2,dustmaps==1.0.14,scikit-build-core==0.11.2,mpi4py==3.1.6,cmake==3.21.3,Python==3.12.1,GNU Fortran (GCC)==10.2.0 |   |

## Creator and Contact
* **Creator:** Dr Tom J. Wilson
* **Affiliation:** Physics and Astronomy, University of Exeter
* **Contact:** `T.J.Wilson@exeter.ac.uk`
* **UK IDAC Publication Date:** 2025-10-24 10:31:59

## Usage and Citation
This dataset is subject to the usage rights as derived from the parent datasets.
Software is developed under the BSD 3-Clause License and published as opensource via GitHub.

**Citation:**
> Wilson & Naylor, MNRAS, 468, 2017, 2517–2525.
> Wilson & Naylor, MNRAS, 481, 2018, 2148–2167.
> Wilson & Naylor, MNRAS, 473, 2018, 5570–5590.
> Wilson, Res. Notes AAS, 6, 2022, 60.
