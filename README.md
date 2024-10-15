# FAST-flow
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
| Name          | Description                          | Algorithm      | Input data              | Citation                    | Repository                    | Web Server           |
|---------------|--------------------------------------|---------------------|------------------------|-----------------------------|----------------------------------------|----------------------|
| Tome | Predicting microorganism growth temperatures and enzyme catalytic optima | Different 6 machine learning models | Sequence| [Li, 2019, ACS Synthetic Biology](https://pubs.acs.org/doi/full/10.1021/acssynbio.9b00099)  | [GitHub](https://github.com/EngqvistLab/Tome)  | Not available|
| TOMER | Improving the accuracy of predicting optima for Topt values >85 °C| Ensemble learning and resampling strategies| Sequence| [Gado, 2020, ACS JCIM](https://pubs.acs.org/doi/full/10.1021/acs.jcim.0c00489)  | [GitHub](https://github.com/jafetgado/tomer/)  | Not available |
| DeepET | A transfer learning approach model for optima prediction trained on 3 million BRENDA enzymes |  Deep neural networks| Sequence| [Li, 2022, Protein Science](https://onlinelibrary.wiley.com/doi/full/10.1002/pro.4480)  | [GitHub](https://github.com/EngqvistLab/DeepET_reps)  |Not available|
| DeepSTABp |Protein melting temperature prediction | Transformer-based protein language model    | Sequence | [Jung, 2023, Int. J. Mol. Sci.](https://www.mdpi.com/1422-0067/24/8/7444)  | [GitHub to Web-UI code](https://github.com/CSBiology/deepStabP)  | [DeepSTABp](https://csb-deepstabp.bio.rptu.de/) |
| GRAPE | Hybrid strategy for protein thermostability improvement  |  hybrid method and greedy algorithm | Sequence and structure| [Cui, 2021, ACS Catalysis](https://pubs.acs.org/doi/10.1021/acscatal.0c05126)  | Not available  |[GRAPE](https://nmdc.cn/grape-web/)|
| MutCompute        | Engineering protein thermal stability tested by FAST-PETase| self-supervised 3D Convolutional Neural Network | Structure    | [Lu, 2022, Nature](https://www.nature.com/articles/s41586-022-04599-z)  | Not available | [MutCompute](https://mutcompute.com/view) |
| FireProt 2.0| Designing thermal stable proteins| Energy-based, evolution-based and ancestral reconstruction-based approaches| Sequence and structure | [Musil, 2023, Briefings in Bioinformatics](https://academic.oup.com/bib/article/25/1/bbad425/7453438)  | Not available| [FireProt 2.0](https://loschmidt.chemi.muni.cz/fireprotweb/) |


## 2. Enzyme Kinetics 
| Name          | Description                          | Algorithm      | Dataset              | Citation                    | Repository                     | Web Server           |
|---------------|--------------------------------------|---------------------|------------------------|-----------------------------|----------------------------------------|----------------------|
| Tool A        | A tool for screening enzyme functions| Machine Learning     | Protein sequences       | Author A. (Year). Title.  | [Link to Tool A](http://example.com)  | [Tool A Web Server](http://example.com) |
| Tool B        | A method for enzyme design           | Molecular Dynamics    | Structural data         | Author B. (Year). Title.  | [Link to Tool B](http://example.com)  | No                   |
| Tool C        | An approach for predicting activity   | Statistical Modeling  | Experimental data       | Author C. (Year). Title.  | [Link to Tool C](http://example.com)  | [Tool C Web Server](http://example.com) |
| Tool D        | Tool for optimizing enzyme properties | Genetic Algorithms    | Genomic data           | Author D. (Year). Title.  | [Link to Tool D](http://example.com)  | No                   |
| Tool E        | A tool for analyzing thermodynamics   | Thermodynamic Modeling| Simulation data         | Author E. (Year). Title.  | [Link to Tool E](http://example.com)  | [Tool E Web Server](http://example.com) |
| Tool F        | A platform for enzyme engineering      | Hybrid Approach       | Multi-omics data       | Author F. (Year). Title.  | [Link to Tool F](http://example.com)  | No                   |

## 3. Folding Stability (Folding energy)
| Name          | Description                          | Algorithm      | Dataset              | Citation                    | Repository                        | Web Server           |
|---------------|--------------------------------------|---------------------|------------------------|-----------------------------|----------------------------------------|----------------------|
| Tool A        | A tool for screening enzyme functions| Machine Learning     | Protein sequences       | Author A. (Year). Title.  | [Link to Tool A](http://example.com)  | [Tool A Web Server](http://example.com) |
| Tool B        | A method for enzyme design           | Molecular Dynamics    | Structural data         | Author B. (Year). Title.  | [Link to Tool B](http://example.com)  | No                   |
| Tool C        | An approach for predicting activity   | Statistical Modeling  | Experimental data       | Author C. (Year). Title.  | [Link to Tool C](http://example.com)  | [Tool C Web Server](http://example.com) |
| Tool D        | Tool for optimizing enzyme properties | Genetic Algorithms    | Genomic data           | Author D. (Year). Title.  | [Link to Tool D](http://example.com)  | No                   |
| Tool E        | A tool for analyzing thermodynamics   | Thermodynamic Modeling| Simulation data         | Author E. (Year). Title.  | [Link to Tool E](http://example.com)  | [Tool E Web Server](http://example.com) |
| Tool F        | A platform for enzyme engineering      | Hybrid Approach       | Multi-omics data       | Author F. (Year). Title.  | [Link to Tool F](http://example.com)  | No                   |
