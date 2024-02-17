# A free biostatistics reading list :)

- Visit [www.justinbelair.ca](https://www.justinbelair.ca/?utm_source=GitHub&utm_medium=reading_list&utm_campaign=header) if you have any questions or need help with statistics.

## Fundamentals

- Misinterpretations of p-values, power analysis, and other concepts
  - [Sander Greenland, Nonsignificance Plus High Power Does Not Imply Supper for the Null Over the Alternative, 2012](https://doi.org/10.1016/j.annepidem.2012.02.007)
  - [John M. Hoenig & Dennis M. Heisey, The Abuse of Power: The Pervasive Fallacy of Power Calculations for Data Analysis, 2001](https://doi.org/10.1198/000313001300339897)

## Philosophical Questions
- [Jose D. Perezgonzalez, *Fisher, Neyman-Pearson or NHST? A tutorial for teaching data testing*, 2015](https://doi.org/10.3389/fpsyg.2015.00223)
  - An interesting overview of the two foundational classical approaches to testing in statistics: Fisher's approach and the Neyman-Pearson framework. The third approach, Null Hypothesis Significance Testing (NHST) is presented as a loose and controversial approach lacking rigour. A must read!

## Classics
- R. A. Fisher, *The Design of Experiments*, 1935 (Book)

  - Contains Fisher's famous lady-tasting tea experiment, first example I know of permutation testing, many groundbreaking examples of Analysis of Variance (ANOVA), and some disparaging (and very funny) remarks towards Pearson.
  
## Missing Data
- [Stef van Buuren, *Flexible Imputation of Missing Data*, 2018 (Book, with online version](https://stefvanbuuren.name/fimd/))
  - A must-have for any applied statistician dealing with missing data problems. This book presents the state-of-the-art in multiple imputation (MI), a field where van Buuren made his name. Contains lots of concrete examples with code, discusses trade-offs in complex situations, and gives lots of references to literature with simulation studies to back any claims up.
  
- Gert Molenberghs and Michael G. Kenward, *Missing Data in Clinical Studies*, 2007 (Book)
  - A deep and thorough exposition of missing data in clinical studies. A complex book for advanced statisticians, especially those working in clinical studies.
  
- Roderick J. A. Little & Donald B. Rubin, *Statistical Analysis with Missing Data*, 2002 (Book)
  - The first textbook put together to reflect the growing literature on missing data methodology. Still useful, although van Buuren, 2018 is probably better suited for applied statisticians

## Causal Inference

### Fundamentals
- Judea Pearl, *Causality : Models, Reasoning and Inference*, 2000, updated in 2009 (Book)
  - A true masterpiece. A technical and deep exposition of Pearl's life work on Directed Acyclic Graphs (DAGs) as Structural Causal Models (SCMs) that got me started on my causal inference journey. His viewpoint is an alternative to the Neyman-Rubin causal model based on potential outcomes. This book can also be seen as the academic version of The Book of Why, a famous general-audience book on causality.
    
- Guido W. Imbens and Donald B. Rubin, *Causal Inference for Statistics, Social, and Biomedical Sciences*, 2015 (Book)
  - A true masterpiece. The most achieved and thorough exposition of the Neyman-Rubin causal model based on potential outcomes. It is an alternative to Pearl's DAG and SCM framework (see above). A beautiful book that I find myself going back to often, for its depth and breadth of insights into thinking about causal inference. Imbens is an economist who contributed much to this field, most notably through is Local-Average Treatment Effect identification in cases of non-compliance. Rubin is one of the greatest living statisticians.
  
- Judea Pearl, Madelyn Glymour & Nicholas P. Jewell, *Causal Inference in Statistics : A Primer*, 2016
  - A gentle introduction to Directed Acyclic Graphs (DAGs) and Structural Causal Models (SCMs) at about the undergraduate in statistics level.
  
- Bill Shipley, *Cause and Correlation in Biology : A User's Guide to Path Analysis, Structural Equations and Causal Inference*, 2000 (Book)
  - A well-written introduction to causal inference for biologists, with an emphasis of Structural Equation Models (SEMs) and Path Analysis. There is also a little bit of interesting history sprinkled in. I took a class with this professor (who just retired from a University close to my home town) in 2023 and his focus on biological applications without sacrificing rigour is great for any non-statistician looking to tackle complex statistical methods!

## Clinical Prediction Modelling

When building prediction models, we are less interested about inference on the parameters and more focused on the values and uncertainty of the predictions. In clinical settings, robust prediction models can mean the difference between life and death!

- [Ewout W. Steyerberg, Clinical Prediction Models, 2010 (Book, with online content)](https://www.clinicalpredictionmodels.org/)
  - A pretty thick reference manual by a leader in the field. Aimed especially towards prediction models in clinical settings, it's a must-have for any advanced modeller looking to make a difference in healthcare with novel technologies.
  
- [Collins et al., Evaluation of clinical prediction models (part 1): from development to external validation, 2024](https://doi.org/10.1136/bmj-2023-074819)
  - Part 1 of a step-by-step tutorial on rigorous and robust clinical prediction model-building, focused on the early stages of model-building.
  
- [Riley et al., Evaluation of clinical prediction models (part 2): how to undertake an external validation study, 2024](https://doi.org/10.1136/bmj-2023-074820)
  - Part 2 of a step-by-step tutorial on rigorous and robust clinical prediction model-building, focused on conducting external validation of the model built following the steps outlined in part 1.
  
- [Riley et al., Evaluation of clinical prediction models (part 3): calculating the sample size required for an external validation study, 2024](https://doi.org/10.1136/bmj-2023-074820)
  - Part 3 of a step-by-step tutorial on rigorous and robust clinical prediction model-building, focused on power and sample size calculations. It is often difficult to know the sample-size required for adequate external validation data. This guide offers detailed instructions on conducting these estimations, once we've built a model.  

## Modeling proportions data (in the 0-1 interval)
### Beta regression

- Foundational papers
  - [Kieschnick & McCullough, *Regression analysis of variates observed on (0, 1): percentages, proportions and fractions*, 2003](https://doi.org/10.1191/1471082X03st053oa)
  - [Ferrari & Cribari-Neto, *Beta Regression for Modelling Rates and Proportions*, 2004](https://doi.org/10.1080/0266476042000214501)
    
- Regression tools
  - [Cribari-Neto & Zeilis, *Beta Regression in R*, 2010](https://doi.org/10.18637/jss.v034.i02)
    - The paper accompagnying the R package betareg
  - [Kubinec, *Ordered Beta Regression: A Parsimonious, Well-Fitting Model for Continuous Data with Lower and Upper Bounds*, 2021](https://doi.org/10.1017/pan.2022.20)
    - A paper proposing an alternative to the Zero-One Inflated Beta (ZOIB Model)
  
### Simplex Regression  
- [Zhang, Qiu & Shi, *simplexreg: An R Package for Regression Analysis of Proportional Data Using the Simplex Distribution*, 2016](https://doi.org/10.18637/jss.v071.i11)
  - Simplex Regression, an alternative to beta regression using the Simplex distribution. Incorporates both MLE and GEE techniques.
      
# Contact
- Visit [www.justinbelair.ca](https://www.justinbelair.ca/?utm_source=GitHub&utm_medium=reading_list&utm_campaign=footer) if you have any questions or need help with statistics.

![alt text](https://github.com/JB-Statistical-Consulting/biostatistics/blob/main/contact.png)
