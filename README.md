# *Loxia* whole genome resequencing data
Data description and analysis plans/workflow for *Loxia* whole genome resequencing data generated for 217 birds including most representatives of Loxia curvirostra that have been recongnized as subspecies, ecotypes, or other populations of interest.

## Information on samples and sequencing


## Reference genome(s)

### 1. Chromosome-level assembly 

We used to rounds of sequencing and assembly to generate a chromosome-level genome assembly for *Loxia sinesciuris*. An initial *de novo* assembly from variable insert size paired-end Illumina sequencing in 2015. This assembly was used as input for scaffolding with the HiRise assembler after sequencing of Chicago and HiC libraries by Dovetail genomics. Report summarizing the assembly is in `red_crossbill_24Feb2018_V5eIH.report.pdf` in this repository. This is essentially a full chromosome level assembly. Jose Cerca has run a diversity of annotation steps that we are going to use along with the assembly to write a short genome note.

Assembly and associated annotation files are on Parchman servers available on request.


|   |   Input Assembly   |   Dovetail HiRise Assembly  |
| :---------------- |   :------:   | :----: |
| Total Length   |   1,034.65 Mb   | 31,034.75 Mb |
| L50/N50   |   91 scaffolds; 3.108 Mb   | 65 scaffolds; 71.807 Mb |
| L90/N90   |   421 scaffolds; 0.451 Mb   | 19 scaffolds; 14.608 Mb |

The assembly in fasta format can be found at:

https://drive.google.com/drive/folders/1MZ8tg9HuzDOGfTKeEXNrDLwpbPsN9_vI?usp=sharing


### 2. Additional de novo assemblies with PacBio HiFi 
We recently used PacBio Hifi sequencing to *de novo* assemble two additional genomes for one type 2 and one type 5 *L. curvirostra*. This workflow, the assemblies and annotation are summarized in `Azenta Bioinformatics Report - Pacbio - denovo assembly - 30-742644819.pdf` in this repository. These assemblies are pretty underwhelming, but would be a good basis for HiC to get them to chromosome level and perhaps some analyses.

The assemblies, in fasta format, can be found at the google drive link below. Summaries of the assemblies can be found in the report referenced above. The assembly for the type 2 bird is in `S170996-2.hifireads.fa` and the assembly for the type 5 is in `171203-5.hifireads.hifireads.fa`

 https://drive.google.com/drive/folders/1VuieqGBdZpBElW6PBIfuvjLluhAqGtEA?usp=sharing


## Whole genome resequencing data

We completed two rounds of WGRS with paired end illumina Novaseq lanes. The first was aimed at thorough sampling of type 2, type 5, and Cassia crossbills (type 9) and was completed via BGI (n=92). The second was aimed at generating global taxonomic sampling with tissue from as many species, subspecies, and ecotypes as we could get our hands on. This second batch was done with Azenta (n=125). Details on each batch are below.

**Sample information and numbers (Total n = 217)**

| Taxon              |   Geography   |   n   |
| :----------------: |   :------:   | ----: |
| *Loxia sinesciuris*   |   South Hills, ID   | 30 |
| *Loxia curvirostra* type 1   |   Virginia   | 6 |
| *Loxia curvirostra* type 1   |   North Carolina   | 1 |
| *Loxia curvirostra* type 2   |   California   | 23 |
| *Loxia curvirostra* type 2   |   Colorado   | 6 |
| *Loxia curvirostra* type 2   |   Montana   | 1 |
| *Loxia curvirostra* type 3   |   California   | 5 |
| *Loxia curvirostra* type 3   |   Oregon   | 2 |
| *Loxia curvirostra* type 4   |   California   | 2 |
| *Loxia curvirostra* type 4   |   Oregon   | 3 |
| *Loxia curvirostra* type 4   |   British Columbia   | 2 |
| *Loxia curvirostra* type 5   |   Colorado   | 16 |
| *Loxia curvirostra* type 5   |   Idaho   | 4 |
| *Loxia curvirostra* type 5   |   Arizona   | 4 |
| *Loxia curvirostra* type 5   |   Oregon   | 2 |
| *Loxia curvirostra* type 6   |   Arizona   | 8 |
| *Loxia curvirostra* type 7   |   British Columbia   | 4 |
| *Loxia curvirostra* type 7   |   Oregon   | 2 |
| *Loxia curvirostra* type 10   |   Oregon   | 3 |
| *Loxia curvirostra* Cypress Hills (type 2?)   | Cypress Hills, Canada  | 8 |
| *Loxia curvirostra percna*  |   Newfoundland   | 1 |
| *Loxia curvirostra poliogyna*  |   Morocco   | 9 |
| *Loxia curvirostra balearica*  |   Mallorca, Spain   | 7 |
| *Loxia curvirostra hispana*  |   Montes de Malaga, Spain   | 6 |
| *Loxia curvirostra curvirostra*  |   Pyrenees, Spain   | 2 |
| *Loxia curvirostra curvirostra*  |   Russia   | 2 |
| *Loxia curvirostra guillemardi*  |   Cyprus   | 3 |
| *Loxia curvirostra tianschanica*  |   Kazakhstan   | 3 |
| *Loxia curvirostra altaiensis*  |   Mongolia   | 4 |
| *Loxia curvirostra bangsi*  |   China   | 1 |
| *Loxia curvirostra himalayensis*  |   Nepal   | 5 |
| *Loxia curvirostra japonica*  |   Japan   | 3 |
| *Loxia curvirostra meridionalis*  |   Vietnam   | 1 |
| *Loxia curvirostra luzoniensis*  |   Philippines   | 8 |
| *Loxia scotia*  |   Scotland   | 2 |
|*Loxia megaplaga*    |   Dominican Republic   | 4 |
| *Loxia l. leucoptera*    |   British Columbia   | 4 |
| *Loxia l. leucoptera*    |   Ontario   | 1 |
| *Loxia l. leucoptera*    |  Alaska   | 1 |
| *Loxia l. leucoptera*    |   New York   | 1 |
| *Loxia l. leucoptera*    |   North Carolina   | 3 |
| *Loxia l. leucoptera*    |   Colorado   | 2 |
| *Loxia l. leucoptera*    |   Unknown North America   | 2 |
| *Loxia pytyopsittacus*    |   Russia   | 3 |


### 2021 WGRS at BGI
A list of fastq IDs and associated information on each bird sequenced during this round can be found in `BGI_2021_fastq_sample_info.csv`. There is data for 92 birds here: 30 *Loxia curvirostra* type 2, 26 *Loxia curvirostra* type 5, 30 *Loxia sinesciuris*, 3 *Loxia leucoptera*, and 3 *Loxia curvirostra poliogyna* (Atlas Mts., Morrocco). Coverage depth should be between 20-30x for these.

Fastq files are on Parchman's storage server (`ponderosa:/backups/rawdata_to_backup/xbill_WGRS/BGI_2022_259/Clean/`), and are now posted on google drive at:

https://drive.google.com/drive/folders/1DrcmMfYGPfCgd95v63GraoRk5PEXOBF3?usp=sharing



### 2023 WGRS at Azenta

This sequencing round included more extensive and broad taxonomic and ecotypic sampling. A list of fastq IDs and associated information on each bird sequenced during this round can be found in `WGRS_Azenta_2023_fastq_sample_info.csv`. Coverage depth should be between 20-25x for these.

Fastq files are on Parchman's storage server (`ponderosa:/backups/rawdata_to_backup/xbill_WGRS/azenta_9_23/30-730065926/00_fastq`), also in a google drive directory in order to share with Andi Kautt:

https://drive.google.com/drive/folders/1ozppxVr5j0BkfZfFbM4OvmhhVj9x2v7d?usp=sharing





## Old GBS data for new and old world *Loxia*

We have ddRADseq data for more thorough sets of new and old world *Loxia* that were analyzed and published in two separate papers, one focusing on North American ecotypes (Parchman et al. 2016, Molecular Ecology), and one focusing on the European birds (Parchman et al. 2018, Journal of Evolutionary Biology). Combined, those samples (n > 375) should serve a nice basis for phylogenetic analyses of broad patterns of diversification in the group. Chad Brock had worked on this data and analyses for this purpose, so he may be the most efficient communicator in terms of sample inclusion, questions, and preliminary findings.