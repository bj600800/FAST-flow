FAST-flow
**F**unctional **A**ssessment, **S**creening and **T**esting **Workflow** for enzymes

## Background
Protein function prediction is considered the Holy Grail of structural biology, aiming to directly infer protein function from sequence and 3D-structure. Algorithms for enzyme function screening and design have been developed over several decades, resulting in the creation of thousands of distinct methods. However, the rapid pace of algorithm advancement, coupled with a lack of comprehensive classification and comparison, has significantly limited the effective integration of these tools into life sciences research. A well-organized knowledge base that categorizes and reviews these algorithms is essential for facilitating their practical use and advancing enzyme function prediction.

## Motivation
⭐ **Centralized Resource**: Provide streamlined access to diverse enzyme function screening and design tools, enhancing research efficiency.

⭐ **Encourage Innovation**: Inspire new ideas and approaches by showcasing available methodologies and their applications.

⭐ **Bridge Bench and Silicon Research**: Facilitate collaboration between computational scientists and experimental biochemists.

## Results
We have summarized cutting-edge algorithms in the field of enzyme function research, categorizing them into six main types: enzyme function classification, catalytic kinetic parameter prediction, solubility prediction, folding stability prediction, thermal stability prediction, and hybrid methods. For each algorithm, we collected seven relevant pieces of information: method name, description of method characteristics, algorithm type, dataset, citation, code repository, and online server availability. We hope that FAST-flow, this comprehensive knowledge base, will meet the algorithmic needs of researchers in this field, thereby facilitating their endeavors in enzyme research.

## 1. Thermal Stability (Catalysis related)
| Name          | Description                          | Algorithm      | Input | Output        | Citation                    | Repository                    | Web Server           |
|---------------|--------------------------------------|---------------|---------|----|-----------------------------|----------------------------------------|----------------------|
| Tome | Predicting microorganism growth temperatures and enzyme catalytic optima | Different 6 machine learning models | Sequence|  OGT/Topt   | [Li, 2019, ACS Synthetic Biology](https://pubs.acs.org/doi/full/10.1021/acssynbio.9b00099)  | [GitHub](https://github.com/EngqvistLab/Tome)  | Not available|
| TOMER | Improving the accuracy of predicting optima for Topt values >85 °C| Ensemble learning and resampling strategies| Sequence| Topt |[Gado, 2020, ACS JCIM](https://pubs.acs.org/doi/full/10.1021/acs.jcim.0c00489)  | [GitHub](https://github.com/jafetgado/tomer/)  | Not available |
| DeepET | A transfer learning approach model for optima prediction trained on 3 million BRENDA enzymes |  Deep neural networks| Sequence| Topt |[Li, 2022, Protein Science](https://onlinelibrary.wiley.com/doi/full/10.1002/pro.4480)  | [GitHub](https://github.com/EngqvistLab/DeepET_reps)  |Not available|
| DeepSTABp |Protein melting temperature prediction | Transformer-based protein language model    | Sequence |Tm |[Jung, 2023, Int. J. Mol. Sci.](https://www.mdpi.com/1422-0067/24/8/7444)  | [GitHub to Web-UI code](https://github.com/CSBiology/deepStabP)  | [DeepSTABp](https://csb-deepstabp.bio.rptu.de/) |
| ThermoFinder| Classification and regression models for thermostability prediction |  Using ensemble learning for representations classification generated by different large language models  | Sequence | Topt/Thermal label| [Yu, 2024, International Journal of Biological Macromolecules](https://www.sciencedirect.com/science/article/pii/S0141813024032744)  | [ThermoFinder](https://github.com/Luo-SynBioLab/ThermoFinder)|Not available |
| GRAPE | Hybrid strategy for protein thermostability improvement  |  hybrid method and greedy algorithm | Sequence and structure| Mutation|[Cui, 2021, ACS Catalysis](https://pubs.acs.org/doi/10.1021/acscatal.0c05126)  | Not available  |[GRAPE](https://nmdc.cn/grape-web/)|
| MutCompute        | Engineering protein thermal stability tested by FAST-PETase| self-supervised 3D Convolutional Neural Network | Structure | Mutation  | [Lu, 2022, Nature](https://www.nature.com/articles/s41586-022-04599-z)  | Not available | [MutCompute](https://mutcompute.com/view) |
| FireProt 2.0| Designing thermal stable proteins| Energy-based, evolution-based and ancestral reconstruction-based approaches| Sequence and structure |Mutation |[Musil, 2023, Briefings in Bioinformatics](https://academic.oup.com/bib/article/25/1/bbad425/7453438)  | Not available| [FireProt 2.0](https://loschmidt.chemi.muni.cz/fireprotweb/) |



## 2. Catalytic Kinetic Parameters
| Name          | Description                          | Algorithm      | Input | Output             | Citation                    | Repository                    | Web Server           |
|---------------|-------------------------------------|----------------|---------|--------------|---------------|-------------------------------|----------------------|
| UniKP         | A unified framework for predicting enzyme kinetic parameters (kcat, Km) | Machine learning models | Sequence | Kinetic parameters |[Yu, 2023, Nat Commun](https://doi.org/10.1038/s41467-023-44113-1) | [GitHub](https://github.com/Luo-SynBioLab/UniKP)  | Not available       |
| MPEK          | A multitask deep learning framework for predicting enzymatic reaction kinetic parameters | Pretrained language models | Sequence| Kcat, and Km values  |[Wang, 2024, Briefings in Bioinformatics](https://doi.org/10.1093/bib/bbae387)  | [GitHub](https://github.com/kotori-y/mpek)  | [Web Server](http://mathtc.nscc-tj.cn/mpek) |
| DeepEnzyme    | A deep learning model utilizing protein 3D-structure features for predicting enzyme turnover numbers (kcat) | GCN, Transformers | Sequence, 3D-structure, substrate information| Kcat|[Wang, 2024, Briefings in Bioinformatics](https://doi.org/10.1093/bib/bbae409)  | [GitHub](https://GitHub.com/hongzhonglu/DeepEnzyme)  | Not available       |
| EITLEM-Kinetics | A deep learning and ensemble transfer learning strategy for enzyme mutant kinetic parameter prediction | Deep learning, Transfer learning | Sequence, substrate information|  kcat, Km, Km|[Shen, 2024, Chem Catalysis](https://www.sciencedirect.com/science/article/abs/pii/S2667109324002665) | [GitHub](https://github.com/XvesS/EITLEM-Kinetics)  | Not available |

## 3. Folding Stability (ddG related)
| Name          | Description                          | Algorithm      | Input | Output        | Citation                    | Repository                    | Web Server           |
|---------------|--------------------------------------|---------------|---------|----|-----------------------------|----------------------------------------|----------------------|
| Pstab | Rapid prediction of changes in protein stabilities over a range of temperatures and experimental conditions upon single- or multiple-point substitutions of charged residues | Ising-like statistical mechanical model | Structure|  ddG   | [Gopi, 2018, Bioinfomatics](https://doi.org/10.1038/s41467-023-44113-1)  | Not available  | [Pstab](https://pbl.biotech.iitm.ac.in/pStab/)|
| FunFolDes | Embed functional motifs into heterologous proteins with Rosetta | Ensemble learning and resampling strategies| Structure | Designed structure |[Bonet, 2018, PLOS Computational Biology](https://doi.org/10.1371/journal.pcbi.1006623)  | [Github](https://github.com/lpdi-epfl/FunFolDesData)  | Not available |
| Rosetta | A comprehensive platform for protein sampling and design | Energy physical functions| Structure | Designed structure |[Leman, 2020, Nature methods](https://www.nature.com/articles/s41592-020-0848-2)  | [Github](https://github.com/rosettacommons)  | [Rosetta commons](https://rosettacommons.org/) |
| FoldX | parallel functions of Rosetta |Empirical energy functions | Structure |ddG | [Delgado, 2019, Bioinformatics](https://academic.oup.com/bioinformatics/article/35/20/4168/5381539)  | Not available  | [FoldX](http://foldxsuite.crg.eu/) |



## Acknowledgment
I would like to acknowledge Chen Muyang and Li Jiahao for their valuable contributions to this review.


