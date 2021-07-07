# Examining the Literature from 1990 to 2020 on Off-line Handwritten Document Analysis

## Purpose

This repository provides the material accompanying the paper:

*Victoria Ruiz, Ruben Heradio, Ernesto Aranda-Escolastico, Ángel Sánchez, and José F. Vélez. Examining the Literature from 1990 to 2020 on Off-line Handwritten Document Analysis.*

Submitted for publication to the [Pattern Recognition Journal](https://www.journals.elsevier.com/pattern-recognition).

## Bibliometric Analysis

To examine systematically the literature from 1990 to 2020 on off-line handwritten document analysis, we followed a workflow structured in three phases:

1. **Data retrieval**. The following query was run on [Scopus](https://www.scopus.com/) to gather [a sample of 5,389 papers](https://github.com/rheradio/OfflineHandwrittenDocumentAnalysis/tree/main/scopus_raw_data) representative of the research area:
```
TITLE(
  (hand-writ* OR handwrit* OR hand-print* OR handprint*)
  AND (recognition  OR  verification  OR  spotting  OR  identification  OR  
      analysis  OR  segmentation)
  AND NOT( (on-line OR online) AND NOT(off-line OR offline) )
) AND (
  LIMIT-TO(SUBJAREA, "COMP") OR LIMIT-TO(SUBJAREA, "ENGI") OR
  LIMIT-TO(SUBJAREA, "MATH")
)
```

2. **Data cleaning and standardization**. Bibliographic data sometimes involves typographical errors and ambiguities that need to be corrected. In particular, the following bibliographic information was standardized:

  * **Keywords**. Our analysis is built upon a bibliometric technique that processes keywords, and so it is mandatory to standardize them. For example, in the context of our study, the following keywords: *NN*, *NEURAL-NETWORKS*, *ARTIFICIAL-NEURAL-NETWORKS*, *NEURAL-NETWORK-MODEL*, etc. correspond to the same concept, and thus they were grouped as *NN*. The file [keyword_standardization.xml](https://github.com/rheradio/OfflineHandwrittenDocumentAnalysis/blob/main/standardization/keyword_standardization.xml) specifies the keyword standardization as follows: 
  ```
  <group name="NN" stop="false">
      <word>NEURAL-NETWORKS</word>
      <word>ARTIFICIAL-NEURAL-NETWORKS</word>
      <word>NEURAL-NETWORK-MODEL</word>
      ...
  </group>
  ```
  
  * **Authors' names**. 
  
3. Lo que sea




### SciMAT Database

### Standardization

## Results

### Most Influential Papers

### Exhaustive Detailed Results


