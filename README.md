# Paper

Title: Asymptotic benchmarking using the [atime](https://github.com/tdhock/atime) package


This repository contains source files, figures, and code used for benchmarking and performance testing. The paper focuses on [comparative benchmarking](https://github.com/DorisAmoakohene/atime-article/blob/main/codes/Comparative_Benchmarking_section.Rmd) and [continuous performance testing](https://github.com/DorisAmoakohene/atime-article/blob/main/codes/Continuous_and_Performance_Testing_Section.Rmd) using the atime approach. The results are visualized in the Figures folder, and the corresponding source files are in the [Paper Source Files](https://github.com/DorisAmoakohene/atime-article/tree/main/Paper%20source%20Files) directory.

# Repository Structure
[Codes/:](https://github.com/DorisAmoakohene/atime-article/tree/main/codes) Contains R Markdown (.Rmd) files used for generating benchmarking results and performance testing analyses.

[Figures/:](https://github.com/DorisAmoakohene/atime-article/tree/main/Figures) Stores output figures generated from the .Rmd scripts.

[Paper Source Files/:](https://github.com/DorisAmoakohene/atime-article/tree/main/Paper%20source%20Files) Includes LaTeX or other documentation source files related to the project.


# How to Reproduce the Figures
Each `.Rmd` file is structured to generate specific figures. To reproduce the results, follow these steps:

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-repo-name.git
   cd your-repo-name
   ```
   
2. Open the corresponding .Rmd file in RStudio or run it using:

```
rmarkdown::render("Codes/<filename>.Rmd")
# eg. rmarkdown::render("Codes/Continuous_and_Performance_Testing_Section.Rmd")
```

3. The figures will be generated and saved.

# 📊 Performance Benchmarking & Computational Analysis  


## Figures & Code Overview  

- [**Figure 1**:](https://github.com/DorisAmoakohene/atime-article/blob/main/Figures/create_subject_pattern_atime.png) Comparing PCRE vs. TRE for regex. [Rcode to replicate](https://github.com/DorisAmoakohene/atime-article/blob/main/codes/Comparative_Benchmarking_section.Rmd)
  
- [**Figure 2**:](https://github.com/DorisAmoakohene/atime-article/blob/main/Figures/create_subject_pattern_best.png) Computation time vs. input size N. Empirical timings (black), theoretical growth (purple). [Rcode to replicate](https://github.com/DorisAmoakohene/atime-article/blob/main/codes/Comparative_Benchmarking_section.Rmd)
  
- [**Figure 3**:](https://github.com/DorisAmoakohene/atime-article/blob/main/Figures/create_subject_pattern_pred.png) Maximum regex subject/pattern size processed within 0.01s.  [Rcode to replicate](https://github.com/DorisAmoakohene/atime-article/blob/main/codes/Comparative_Benchmarking_section.Rmd)
  
- [**Figure 4**:](https://github.com/DorisAmoakohene/atime-article/blob/main/Figures/vec.mat.result.plot.png) Memory usage, object length, and execution time for vector, dense, and sparse matrices. [Rcode to replicate](https://github.com/DorisAmoakohene/atime-article/blob/main/codes/Comparative_Benchmarking_section.Rmd)
  
- [**Figure 5a**:](https://github.com/DorisAmoakohene/atime-article/blob/main/Figures/data.table-atime_versions.png) Profiling `shallow()` copy in data tables—constant time in **Fast** vs. **Slow** versions, validated via GitHub PR checks [**Figure 5b**:](https://github.com/DorisAmoakohene/atime-article/blob/main/Figures/data.table-atime_test.png).  [Rcode to replicate](https://github.com/DorisAmoakohene/atime-article/blob/main/codes/Continuous_and_Performance_Testing_Section.Rmd)

