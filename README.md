## CLF WBLCA Benchmark Study v2 - Dataset
This is a public repository containing data that were collected, prepared, and published as part of the CLF WBLCA Benchmark Study V2 and referenced by a forthcoming Data Descriptor paper titled "A Harmonized Dataset of High-Resolution Whole Building Life Cycle Assessment Results in North America". 

The dataset contains building design characteristics, life cycle inventories, and environmental impact assessment results for 292 building projects in the United States and Canada. It includes harmonized and non-aggregated LCA model results across life cycle stages, building elements, and building materials to enable detailed analysis, comparisons, and data reuse. It’s composed of over 90 building design and LCA features to assess distributions and trends of material use and environmental impacts. Uniquely, the data were crowd-sourced from designers conducting LCAs of real-world building projects.

The code used to prepare this dataset is available at: https://github.com/Life-Cycle-Lab/wblca-benchmark-v2-data-preparation

## Repository Contents
The repository contains:
- **readme.md** is a text file containing general descriptions of the dataset
- **buildings_metadata.xlsx** includes all project metadata and LCA parameters for every project associated with a unique index number to cross-reference across other files. This also includes various calculated summaries of LCI and LCIA totals and intensities per project. 
- **full_lca_results.xlsx** includes LCI and LCIA results per material and life cycle stage of each building project. 
- **data_glossary.xlsx** identifies and defines each feature of the dataset including its name, data structure, syntax, units, descriptions, and more

## Data Structure
**Please refer to the data descriptor article for full details, descriptions, and usage notes regarding the dataset and its structure.**

The **buildings_metadata.xlsx** file is structured so that each row of data reflects a single project. It contains 72 features organized by feature types including site context, building design, structural design, LCA methods, and calculated summaries. 

The **full_lca_results.xlsx** file is structured in a novel way that enables high-resolution data filtering and comparison-making. It is similar to the non-aggregated LCA tool output formats of Tally and One Click LCA where each row of data reflects a single material and life cycle stage from an individual project and contains the materials associated classifications, inventory data, and impacts. It contains 21 features organized by feature types for LCA classifications, LCI results, LCIA results, and calculated summaries. The two dataset files can be merged or joined using unique primary keys (project_index) that are assigned to each project to facilitate a wide range of uses and types of analysis. 

## Versioning
Versions on this repository are tracked using Releases on GitHub. 

## How to cite
Please cite both the Data Descriptor and the specific data version used:
- **Data Descriptor:** Benke, B., Chafart, M., Shen, Y., Ashtiani, M., Carlisle, S., and Simonen, K.  *A Harmonized Dataset of High-Resolution Whole Building Life Cycle Assessment Results in North America.* In Review. Preprint available at https://doi.org/10.21203/rs.3.rs-6108016/v1
- **Dataset:** Refer to the latest version on Figshare https://doi.org/10.6084/m9.figshare.28462145.v1

## Project Background 
In 2017, the Carbon Leadership Forum (CLF) published the Embodied Carbon Benchmark Study for North American buildings. Since then, the practice of whole-building life cycle assessment (WBLCA) has grown rapidly in the AEC industry, and it’s become clear that more robust and reliable benchmarks are critical for advancing work in this field. The new CLF WBLCA Benchmark Study (Version 2) is built upon research and insights from the 2017 study. The project expanded our research methodology, included more comprehensive data collection, and resulted in a high-resolution dataset of harmonized WBLCA model results and project design characteristics for nearly 300 buildings across the United States and Canada. Outcomes from this project are aimed to enable designers and decision-makers to set reliable embodied carbon targets and understand the potential for reduction throughout the design and construction processes.

## Additional Project Resources
- [WBLCA Benchmark Study V2 Project Page - Carbon Leadership Forum](https://carbonleadershipforum.org/clf-wblca-v2/)
- [WBLCA Benchmark Study V2 Project Page - Life Cycle Lab at University of Washington](https://www.lifecyclelab.org/projects/)
- [Data Descriptor - A Harmonized Dataset of High-Resolution Whole Building Life Cycle Assessment Results in North America](https://doi.org/10.21203/rs.3.rs-6108016/v1)
- [California Carbon Report](https://carbonleadershipforum.org/california-carbon/)
- [Data Entry Template](https://hdl.handle.net/1773/51286)
- [Data Collection User Guide](https://hdl.handle.net/1773/51285)
- Benchmark Study Dashboard (forthcoming)

## Acknowledgements
We would like to thank the Alfred P. Sloan Foundation, the ClimateWorks Foundation, and the Breakthrough Energy Foundation for supporting this research project. 

We thank this study’s participating design practitioners (data contributors) who provided substantial time and effort in recording and submitting building project data and sharing feedback with the research team. These companies included: Arrowstreet Architects, Arup, BranchPattern, Brightworks Sustainability, Buro Happold, BVH Architecture, DCI Engineers, EHDD, Ellenzweig, Gensler, GGLO, Glumac, Group 14 Engineering, Ha/f Climate Design, HOK, KieranTimberlake, KPFF Consulting Engineers, Lake|Flato, LMN Architects, Mahlum Architects, Mead & Hunt, Inc., Mithun, Perkins&Will, reLoad Sustainable Design Inc., SERA Architects, Stok, The Green Engineer Inc., The Miller Hull Partnership, LLP., Walter P Moore, and ZGF Architects LLP.
