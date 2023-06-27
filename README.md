# Trends
Code &amp; datasets for the paper "What’s next? Forecasting scientific research trends"

Abstract
Scientific research trends and interests evolve over time. The ability to identify and forecast these trends is vital. We predict future trends in scientific publications using heterogeneous public sources, including historical publications from PubMed, research and review articles, and patents. We demonstrate that scientific trends can be predicted five years in advance, with preceding publications and future patents serving as leading indicators for emerging scientific topics. We found that the ratio of reviews to original research articles is an informative feature for identifying increasing or declining topics, with declining topics having an excess of reviews. We find that language models provide improved insights and predictions into topic temporal dynamics. Our findings suggest that similar dynamics apply to molecular, technological, and conceptual topics across biomedical research.

Arxiv preprint:
https://arxiv.org/abs/2305.04133

```
@misc{ofer2023whats,
      title={Whats next? Forecasting scientific research trends}, 
      author={Dan Ofer and Michal Linial},
      year={2023},
      eprint={2305.04133},
      archivePrefix={arXiv},
      primaryClass={cs.DL}
}
```

A website to access the predictions is in progress and will also be made available. 

Replicating the pipeline:
* [OPTIONAL: For adding your own data]: Download datasets of terms results from PubmedByYear manually, using URLs constructed in `PrepData_Trends.ipynb` notebook (click links) - can also add additional topics here. This will output the training data `trends_v6.csv.gz` and long term historical context (`trends_context_v6.csv.gz`) (used for additional features) files.
      * Training data and context is already provided in this repo.
* Modelling results and evaluation: `plot trend pred + CV-V2023.ipynb`
* Analysis of Patents leading future publications, with CRISPR as an use-case: `crispr_patent_paper_Corr.ipynb`
