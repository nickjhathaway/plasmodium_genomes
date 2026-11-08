# plasmodium\_genomes
Version 2.0.0 - 2026-11


## *Plasmodium falciparum* genomes
Contains 13 Plasmodium falciparum reference genomes and annotation files. Genomes include Pf3D7 reference genome version 2020-09-01. Also included are the genomes from Otto et al 2018. 


*Otto , T. D., Böhme, U., Sanders, M., Reid, A., Bruske, E. I., Duffy, C. W., Bull, P. C., Pearson, R. D., Abdi, A., Dimonte, S., Stewart, L. B., Campino, S., Kekre, M., Hamilton, W. L., Claessens, A., Volkman, S. K., Ndiaye, D., Amambua-Ngwa, A., Diakite, M., … Berriman, M. (2018). Long read assemblies of geographically dispersed Plasmodium falciparum isolates reveal highly structured subtelomeres. Wellcome Open Research, 3, 52.*

## *Plasmodium vivax* genomes

Contains 3 Plasmodium vivax reference genomes and annotation files. These are PvP01, PvPAM (a vivax genome best for South America), PvW1. Files were downloaded from [PlasmoDB](https://plasmodb.org).

**PvP01** (Papua, Indonesia)

*Auburn, S., Böhme, U., Steinbiss, S., Trimarsanto, H., Hostetler, J., Sanders, M., Gao, Q., Nosten, F., Newbold, C. I., Berriman, M., Price, R. N., & Otto, T. D. (2016). A new Plasmodium vivax reference sequence with improved assembly of the subtelomeres reveals an abundance of pir genes. Wellcome Open Research, 1, 4.*

**PvPAM** (Peruvian Amazon)

*De Meulenaere, K., Cuypers, B., Gamboa, D., Laukens, K., & Rosanas-Urgell, A. (2023). A new Plasmodium vivax reference genome for South American isolates. BMC Genomics, 24, 606.*

**PvW1** (Thailand)

*Minassian, A. M., Themistocleous, Y., Silk, S. E., Barrett, J. R., Kemp, A., Quinkert, D., Nielsen, C. M., Edwards, N. J., Rawlinson, T. A., Ramos Lopez, F., Roobsoong, W., Ellis, K. J., Cho, J. S., Aunin, E., Otto, T. D., Reid, A. J., Bach, F. A., Labbé, G. M., Poulton, I. D., … Draper, S. J. (2021). Controlled human malaria infection with a clone of Plasmodium vivax with high-quality genome assembly. JCI Insight, 6(23), e152465.*

## *Plasmodium ovale* genomes

Contains a reference genome for *Plasmodium ovale curtisi* (Poc221, South Sudan) and *Plasmodium ovale wallikeri* (Pow222, Nigeria). Files were downloaded from [github.com/MatthewHiggins2017/HigginsMPovaleReferences](https://github.com/MatthewHiggins2017/HigginsMPovaleReferences).

*Higgins, M., Manko, E., Ward, D., Phelan, J. E., Nolder, D., Sutherland, C. J., Clark, T. G., & Campino, S. (2024). New reference genomes to distinguish the sympatric malaria parasites, Plasmodium ovale curtisi and Plasmodium ovale wallikeri. Scientific Reports, 14, 3843.*

## *Plasmodium malariae* genome

Contains 1 reference genome for *Plasmodium malariae* (PmUG01). Files were downloaded from [PlasmoDB](https://plasmodb.org).

*Rutledge, G. G., Böhme, U., Sanders, M., Reid, A. J., Cotton, J. A., Maiga-Ascofare, O., Djimdé, A. A., Apinjoh, T. O., Amenga-Etego, L., Manske, M., Barnwell, J. W., Renaud, F., Ollomo, B., Prugnolle, F., Anstey, N. M., Auburn, S., Price, R. N., McCarthy, J. S., Kwiatkowski, D. P., … Otto, T. D. (2017). Plasmodium malariae and P. ovale genomes provide insights into malaria parasite evolution. Nature, 542(7639), 101–104.*


## *Plasmodium knowlesi* genome

Contains 1 reference genome for *Plasmodium knowlesi* (PkH, assembly version 2). Files were downloaded from [PlasmoDB](https://plasmodb.org).

*Pain, A., Böhme, U., Berry, A. E., Mungall, K., Finn, R. D., Jackson, A. P., Mourier, T., Mistry, J., Pasini, E. M., Aslett, M. A., Balasubrammaniam, S., Borgwardt, K., Brooks, K., Carret, C., Carver, T. J., Cherevach, I., Chillingworth, T., Clark, T. G., Galinski, M. R., … Berriman, M. (2008). The genome of the simian and human malaria parasite Plasmodium knowlesi. Nature, 455(7214), 799–803.*


## Directory structure

*  genomes/  
	*	 Contains the fasta files of the genomes 
*	info/gff/
	*	 Contains the annotation files of the genomes in gff3 format 
*	info/drug_resistant_aaPositions.tsv
	*  A file with a list of currently (2025-02) known associated drug resistant loci 
*  info/drug_resistant_aaPositions.bed  
	*  The Pf3D7 genomic locations of the drug resistant loci 


Files are in gz format for size considerations but most programs will want the files in uncompressed format, once git is downloaded you can run the utility script in bin/unzip_data.sh to unzip all the gz files. The files are tracked with **git lfs** and so needs to be installed and make sure to pull them. 

```
git clone https://github.com/nickjhathaway/plasmodium_genomes.git
cd plasmodium_genomes
git lfs fetch
bin/unzip_data.sh
```

   