
| Dataset Dir Name      |  Name                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Source- Target                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |                                                                                                           | Info                                                                                                                                                                                                                                                                                                                                                                                                      |
|-----------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| T-Box/Schema Matching |
| anatomy               | [Anatomy track](http://oaei.ontologymatching.org/2023/anatomy/index.html)                                                                                                                                                                            | `mouse` - `human`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |                                                                                                           | The anatomy real world case is about matching the Adult Mouse Anatomy (2744 classes) and the NCI Thesaurus (3304 classes) describing the human anatomy.                                                                                                                                                                                                                                                   |
| food                  | [Food Nutritional Composition](http://oaei.ontologymatching.org/2023/food/index.html)                                                                                                                                                                | `ciqual`-`siren`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | `food_v2sub`                                                                                              | This track consists of finding alignments between food concepts from CIQUAL, the French food nutritional composition database, and food concepts from SIREN. Food concepts from both databases are described in LanguaL, a well-known multilingual thesaurus using faceted classification.                                                                                                                |
| biodiv                | [Biodiversity and Ecology track](http://oaei.ontologymatching.org/2022/biodiv/index.html)                                                                                                                                                            | `envo`-`sweet`<br>`gemet`-`anaeethes` <br> `nalt`-`agrovoc` <br> `taxrefldAnimalia`-`ncbitaxonAnimalia` <br> `taxrefldBacteria`-`ncbitaxonBacteria` <br> `taxrefldChromista`-`ncbitaxonChromista` <br> `taxrefldFungi`-`ncbitaxonFungi` <br> `taxrefldPlantae`-`ncbitaxonPlantae` <br> `taxrefldProtozoa`-`ncbitaxonProtozoa`                                                                                                                                                                                                                                                                         | `biodiv_2022`                                                                                             | The goal of the track is to find pairwise alignments between ontologies and thesauri that are particularly useful for biodiversity and ecology research and are being used in various projects. They have been developed in parallel and are very overlapping. They are semantically rich and contain tens of thousands of classes.                                                                       |
| **`bio-ml`            | [Bio-ML](https://www.cs.ox.ac.uk/isg/projects/ConCur/oaei/) <br/> [Bio-ML Trak 2023](https://www.cs.ox.ac.uk/isg/projects/ConCur/oaei/2023/index.html) <br/> [Bio-ML: Documentation](https://krr-oxford.github.io/DeepOnto/bio-ml/#oaei-bio-ml-2023) |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |                                                                                                           | Totally a different modeling                                                                                                                                                                                                                                                                                                                                                                              |                                                                                                                                                                                                                                                                                                                                                                                                       |
| commonkg              | [Common Knowledge Graphs](http://oaei.ontologymatching.org/2023/commonKG/index.html)                                                                                                                                                                 | `yago`-`wikidata`<br/>`nell`-`dbpedia`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | `commonkg_yago-wikidata-v1` <br/> `commonkg_nell-dbpedia-v1`                                              | This track composes of a task aimed at matching the schema of two common and highly influential knowledge graphs which are : DBpedia and the Never Ending Language Learner (NELL).                                                                                                                                                                                                                        |
| +largebio             | [Large BioMed Track (largebio)](http://www.cs.ox.ac.uk/isg/projects/SEALS/oaei/)                                                                                                                                                                     | `snomed`-`nci`  <br/>  `fma`-`nci` <br/>`fma`-`snomed`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | `largebio-snomed_nci_whole_2016`<br/> `largebio-fma_nci_whole_2016`<br/> `largebio-fma_snomed_whole_2016` |
| +phenotype            | [Disease and Phenotype Track](https://sws.ifi.uio.no/oaei/phenotype/)                                                                                                                                                                                | `doid`-`ordo` <br/> `hp`-`mp`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         | `phenotype_phenotype-doid-ordo-2017-bioportal` <br> `phenotype_phenotype-hp-mp-2017-bioportal`            |
| mse                   | [Material Sciences and Engineering](https://github.com/EngyNasr/MSE-Benchmark/tree/main)                                                                                                                                                             | `MaterialInformationReduced`-`MatOnto` <br> `MaterialInformation`-`MatOnto` <br> `MaterialInformation`-`EMMO`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         | `mse_2021`                                                                                     | The Material Sciences and Engineering (MSE) track contains the first benchmark for the evaluation of (semi-)automatic ontology matching techniques. In this emerging ontological domain, small to mid-sized upper and domain level ontologies are used that contain concepts described in natural language and are implemented by heterogeneous design principles with only partial overlap to each other |


Notes:
- MELT Track Repository: https://dwslab.github.io/melt/track-repository
- [MultiFarm](http://oaei.ontologymatching.org/2022/multifarm/index.html): supports various languges
- Complex track - OAEI 2023 is simpler than OAEI-2022 (we considered 2022)
  - However, only `Populated GeoLink` and `Populated Enslaved` had no conflict with other tracks so we considered them
- OAEI 2023 Campaign: http://oaei.ontologymatching.org/2023/
- OAEI 2022 Campaign (results exists): http://oaei.ontologymatching.org/2022/
- Public OAEI systems for the latest campaigns: https://drive.google.com/drive/folders/14yFbYm4IMnO1CIDi7umLr4WJPZMumH7Q
- MELT python example matcher eval: https://github.com/dwslab/melt/tree/master/examples/externalPythonMatcherWeb
- ** Bio-ML: Machine Learning-Friendly Biomedical Datasets for Equivalence and Subsumption Ontology Matching
  - https://zenodo.org/record/6946466
  - The Bio-ML track is a Machine Learning (ML) friendly Biomedical track for Equivalence and Subsumption Matching. This track presents an unified evaluation framework suitable for both ML-based and non-ML-based OM systems. The datasets of this track are based on Mondo and UMLS Metathesarus. This track supersedes the previous largebio and phenotype tracks.
  - +: `phenotype` and `largebio` are in Bio-ML
- **Tabular data to Knowledge Graph matching** un-explored in this work
  - https://www.cs.ox.ac.uk/isg/challenges/sem-tab/