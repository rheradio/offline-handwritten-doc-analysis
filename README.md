# Examining the Literature from 1990 to 2020 on Off-line Handwritten Document Analysis

## Purpose

This repository provides the material accompanying the paper:

*Victoria Ruiz, Ruben Heradio, Ernesto Aranda-Escolastico, Ángel Sánchez, and José F. Vélez. Examining the Literature from 1990 to 2020 on Off-line Handwritten Document Analysis.*

Submitted for publication to the [Pattern Recognition Journal](https://www.journals.elsevier.com/pattern-recognition), and whose abstract is:

> Providing computers with the ability to process handwriting is both important and challenging, since many difficulties (e.g. different writing styles, alphabets, languages, etc.) need to be overcome for addressing a variety of problems (text recognition, signature verification, writer identification, word spotting, etc.).
This paper reviews the growing literature on off-line handwritten document analysis over the last thirty years. A sample of 5,389 articles published along years was examined using bibliometric techniques. This paper identifies (i) the most influential articles in the area, (ii) the most productive authors and their collaboration networks, (iii) the countries and institutions that have led research on the topic, (iv) the journals that have published most papers, and (v) the most relevant research topics and their evolution over the years.

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
  
  * **Authors' names**. The file [author_name_standardization.xml](https://github.com/rheradio/OfflineHandwrittenDocumentAnalysis/blob/main/standardization/author_name_standardization.xml)
  ```
meter aqui ejemplo de estandarizacion de autores
  ```
  
3. **Data analysis**. We performed the bibliometric analysis of the polished paper sample with the help of [SciMAT](https://sci2s.ugr.es/scimat/), which is an open-source tool (GPLv3). The file [scimat_database](https://github.com/rheradio/OfflineHandwrittenDocumentAnalysis/blob/main/scimat_database/scimat_database) stores our paper sample and the configuration of our analysis. To use it:

  * First, [download SciMAT](https://sci2s.ugr.es/scimat/download.html).
  * Then, run SciMAT and open the file [scimat_database](https://github.com/rheradio/OfflineHandwrittenDocumentAnalysis/blob/main/scimat_database/scimat_database) with the SciMAT menu option [*File -> Open Project*](https://sci2s.ugr.es/scimat/software/v1.01/SciMAT-v1.0-userGuide.pdf)

## Results

### Most Influential Papers

### Exhaustive Detailed Results


