# Heuer_2020
code used for Heuer et al, 2020 manuscript for gene expression analysis of genetically diverse AD-BXD and Ntg-BXD mice

Documents in this repository:

1) "Kacz_Pear_cluster_assignments.csv" - File with all genes and assigned modules used in this study 
  Column A: genesymbols
  Column B: SpeakEasy module assignment

2) "Kacz_Pear_cluster_assignments_ONLY28Mod.csv"- File with all genes and modules with >29 members used for downstream analysis
  Column A: genesymbols
  Column B: SpeakEasy module assignment for 28 modules used for downstream analysis

3) "Kacz_Pear_module_values.csv"- File with standardized average expression for each of the 28 modules used for downstream behavioral analysis
  Column A: module ID 
  Columbs B-FA: Values for each of the 156 strain/sex/genotype/age group averaged "samples" used for this analysis

4) "Kacz_Pear_module_values_T.csv"- Transposed information from "Kacz_Pear_module_values.csv" 
  Column A: Sample ID with matching identifiers for Phenotype key
  Column B-AC: Standardized average module expression for each module

5) "ExpandedPhenoKey_strainAverages_allRNA.csv"- Corresponding behavioral measures for each of the 156 strain/sex/genotype/age group averaged "samples" used in this analysis. Some behavioral measures in this sheet were not used in this analysis.
  Column A: B6-BXD strains corresponding to each measure 
  Column B: Sex of each sample; 0 = female, 1 = male
  Column C: FAD mutation status or "Genotype"; 0 = Ntg-BXD, 5 = AD-BXD
  Column D: Age at which mouse was harvested; 6 = 6 months, 14 = 14 months
  Column E: Sample ID to match phenotype with module expression file
  Column F: B6-BXD strains corresponding to each measure using short-hand (with no BXD in label)
  Column G: Gender.Mean; Other column to call Sex of mouse; 0 = female, 1 = male
  Column H: Genotype; Another genotype column; 0 = Ntf-BXD, 5 = AD-BXD
  Column I: Age at which mouse was harvested; Another age column; 6 = 6 months, 14 = 14 months
  Column J: Strain_Sex_Age_Geno; abbreviation for identifier of sample by the BXD strain, Sex, Age harvested, and FAD mutation status
  Column K: ELISA; Ab1-42 ELISA results (ng/uL)
  Column L: Ymaze.Distance; total distance traveled during Y-maze test
  Column M: Ymaze.TotalArms; total number of arm entire furing Y-maze test
  Column N: Ymaze.SponAlt; Spontaneous alternation frequency (as %) during Y-maze test
  Column O: Weight; body weight of mouse 
  Column P: Narrow.Beam; Time (in seconds) the mouse took to walk across narrow beam
  Column Q: Incline.Screen; Incline screen score
  Column R: Grip.Strength: Grip strength score
  Column S: SM.Composite: Composite sensorimotor score generated from Narrow beam, incline screem and grip strength data
  Column T: EPM.Distance: Total disance traveled during elevated plus maze (EPM) test
  Column U: EPM.TotalArms: Total arms entered during elevated plus maze (EPM) test
  Column V: EPM.PercenOpenEntries; Percent of total arms entered were the open arm during elevated plus maze (EPM) test
  Column W: EPM.PercenOpenTime; Percent time spent in open arms during elevated plus maze (EPM) test
  Column X: CFC.Baseline: Percent of time spent freezing during CFC day 1 before any shock was delivered
  Column Y: CFC.PS4: Percent of time spent freezing during CFC day 1 after 4th shock was delivered
  Column Z: CFC.AcqSlope: Slope of line when percent freezing during each post-shock interval is measured as a function of each post-shock interval
  Column AA: CFC.CFM: Percent of time spent freezing during CFC day 2 when no shock is delivered

6) "ReducedPhenoKey_justCog_strainAverages_allRNA.csv"- - Corresponding behavioral measures for each of the 156 strain/sex/genotype/age group averaged "samples" used in this analysis; only includes behavioral measures used in this analysis.
  Column A: Sample ID to match phenotype with module expression file
  Column B: Sex of each sample; 0 = female, 1 = male
  Column C: FAD mutation status or "Genotype"; 0 = Ntg-BXD, 5 = AD-BXD
  Column D: Age at which mouse was harvested; 6 = 6 months, 14 = 14 months
  Column E: B6-BXD strains corresponding to each measure 
  Column F: B6-BXD strains corresponding to each measure using short-hand (with no BXD in label)
  Column G: Geno_Ag; Genotype and Age group identifier for each sample
  Column H: Geno_Age_Sex ; Genotype, Age and Sex group identifier for each sample
  Column I: Ymaze.SponAlt; Spontaneous alternation frequency (as %) during Y-maze test
  Column J: CFC.PS4: Percent of time spent freezing during CFC day 1 after 4th shock was delivered
  Column K: CFC.AcqSlope: Slope of line when percent freezing during each post-shock interval is measured as a function of each post-shock interval
  Column L: CFC.CFM: Percent of time spent freezing during CFC day 2 when no shock is delivered
  Column M: ELISA; Ab1-42 ELISA results (ng/uL)

7) "BarresLab_CellType_MAX.csv"- All genes tested in Zhang et al and pulled from brainrnaseq.org, and cell-type assignment based on where the gene had highest FPKM value
  Column A: genesymbol
  Column B: assigned cell-type

8) "SEmodule_eigengeneMapping.csv"- Module eigengene values in format where they can be mapped using rQTL
  Column A: Sample ID 
  Column B: Sex of each sample; 0 = female, 1 = male
  Column C: FAD mutation status or "Genotype"; 0 = Ntg-BXD, 5 = AD-BXD
  Column D: Age at which mouse was harvested; 6 = 6 months, 14 = 14 months
  Column E: B6-BXD strains corresponding to each measure using short-hand (with no BXD in label)
  Column F: B6-BXD strains corresponding to each measure in longer format
  Column G: m1 eigengene
  Column H: m2 eigengene
  Column I: m3 eigengene
  Column J: m4 eigengene
  Column K: m5 eigengene
  Column L: m6 eigengene
  Column M: m7 eigengene
  Column N: m8 eigengene
  Column O: m13 eigengene
  Column P: m14 eigengene
  Column Q: m15 eigengene
  Column R: m16 eigengene
  Column S: m18 eigengene
  Column T: m20 eigengene
  Column U: m23 eigengene
  Column V: m28 eigengene
  Column W-JVN:

9) "MousetoHuman_MatchedIDs_ALL.csv"- matched mouse genesymbols to human genesymbols 
  Column A: Human EnsembleID
  Column B: Human Ensemble transcript ID
  Column C: Mouse EnsembleID
  Column D: Mouse genesymbol
  Column E: mouse homology type from human EnsembleID

10) "Mostafavi2018_SpeakEasyModules.csv"- Module assignments from Mostafavi et al, 2018
  Column A: module assignments
  Column B: Human genesymbols
  Column C: misc. identifier information

11) "AMPAD_Modules_10Jan2019_SynapseDownload.csv"- Module assignments from Logston et al, 2019, AMP-AD modules
  Column A: Row ID number
  Column B: misc. Row version
  Column C: Human EnsembleID
  Column D: Module ID
  Column E: method used for module assignment
  Column F: method and module assignment
  Column G: brain region taken for RNAseq
  Column H: method and module assignment
  Column I: Human genesymbol
  
  




