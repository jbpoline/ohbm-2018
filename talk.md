---
title: The problems associated with the use of p-values in brain imaging and their effects on reproducibility 
shortitle: Evil p-values 
subtitle: A reproducibility perspective 
date:  June 17 2018
author: JB Poline \newline
institute: McGill University, UC Berkeley

header-include:
	- \usefonttheme{professionalfonts}
	- \usepackage{fontspec}
	- \setsansfont[BoldFont = {Fira Sans Medium}]{Fira Sans}
	- \setmonofont{Fira Mono}
        - \usepackage{amsmath}
---

Plan
=================================================================================

- what is/are the pb?
	- is Ioannidis right?
	- technical 
	- sociological


# Issues of reproducibility in sciences 

## <!-- Issues of reproducibility in sciences -->

![Stodden, 2014](./images/credibility-crisis.png){ height=200px }

<!-- Say that still, many people do not take this seriously: this is only other researchers problem, not mine -->

# Historical perspective

- When did we start to talk of the pb? 
	- in a nutshell, almost at the time of the p-value was defined
- Fisher conception:
	- an indication of something about H0
- Neyman Pearson conception:
	- a decision making rule
- Which one is used today ?

# Social factors 


# Significance testing as perverse probabilistic reasoning

![Westover, 2014](./images/westover-questions.png){ height=200px }
<!--   -->

# Significance testing as perverse probabilistic reasoning

![Westover, 2014](./images/westover-table-results.png){ height=200px }

# Social: the life science curse

- Publications only with p<.05 
- Reviewers and editors dont want to publish negative results: the "impact" issue 

>   "...  whether you would be able to review the manuscript "No Evidence
>   for an Effect of XXX on Hippocampal Volume in a YYY Sample", by  \emph{some-authors},
>   submited for consideration in ..."

- reviewer story

# Social: incentives get in the way 

# Social: incentives get in the way 

![Bishop, 2015](./images/harcking-hacking-bishop.png){ height=240px }

Example 1
=================================================================================

![Westover, 2014](./images/muller-jama-psy-unipolar-depression-meta-analysis.png){ height=120px }

\vspace{-1cm}

> \small{During the past 20 years, numerous neuroimaging experiments have investigated aberrant brain activation during cognitive and emotional processing in patients with unipolar depression.}

> \small{In total, 57 studies with 99 individual neuroimaging experiments comprising in total 1058 patients were included; 34 of them tested cognitive and 65 emotional processing. Overall analyses across cognitive processing experiments ( P > .29) and across emotional processing experiments ( P > .47) revealed no significant results. }


Examples 2: All foods cause cancer ?
=================================================================================

- Of 264 single-study assessments, 191 (72%) concluded that the tested food was associated with an increased ( n = 103) or a decreased ( n = 88) risk;
- 75% of the risk estimates had weak (0.05 > P > 0.001) or no statistical ( P > 0.05) significance. 
- Meta-analyses ( n = 36) presented more conservative re- sults; only 13 (26%) reported an increased ( n = 4) or a decreased ( n = 9) risk  


Consequences: Button et al
=================================================================================
- inflated effect sizes
- decreased PPV 

The reactions: 
=================================================================================
- APS ban
- long list of checkboxes in nature publications
- nature statistician review

The solutions
=================================================================================
- social 
- technical (Bayesian)
- socio-technical 

Solutions - social 
=================================================================================
- Ban p-values ?
- Cobidas / NPRC / Best practices / ...
- Education (Editors, Reviewers, Authors, Universities, ...)
- 


Solutions - technical - redefine significance
=================================================================================

## Abstract

\large{"We propose to change the default P-value threshold for
statistical significance for claims of new discoveries from 0.05 to 0.005."}

\hspace{.5cm}

\tiny{Daniel J. Benjamin 1 *, James O. Berger 2 , Magnus Johannesson 3 *, Brian A.  Nose k 4, 5 , E.  - J.  W agenma k er s 6 , Richard Ber k 7, 1 0 , K enneth A.  Bollen 8 , Björn Bremb s 9 , Lawrence Brown 10 , Colin Camerer 11 , David Cesarini 12, 13 , Christopher D. Chambers 14 , Merlise Clyde 2 , Thomas D. Cook 15,16 , Paul De Boeck 17 , Zoltan Dienes 18 , Anna Dreber 3 , Kenny Easwaran 19 , Charles Efferson 20 , Ernst Fehr 21 , Fiona Fidler 22 , Andy P.  Field 18 , Malcolm Forster 23 , Edward I. George 10 , Richard Gonzalez 24 , Steven Goodman 25 , Edwin Green 26 , Donald P.  Green 27 , Anthony Greenwald 28 , Jarrod D. Hadfield 29 , Larry V.  Hedges 30 , Leonhard Held 31 , Teck Hua Ho 32 , Herbert Hoijtink 33 , James Holland Jones 39,40 , Daniel J. Hruschka 34 , Kosuke Imai 35 , Guido I mbens 36 , John P.A.  Ioannidis 37 , Minjeong Jeon 38 , Michael Kirchler 41 , David Laibson 42 , John List 43 , Roderick Little 44 , Arthur Lupia 45 , Edouard Machery 46 , Scott E. Maxwell 47 , Michael McCarthy 48 , Don Moore 49 , Stephen L. Morgan 50 , Marcus Munafó 51, 52 , Shinichi Nakagawa 53 , Brendan Nyhan 54 , Timothy H. Parker 55 , Luis Pericchi 56 , Marco Perugini 57 , Jeff Rouder 58 , Judith Rousseau 59 , Victoria Savalei 60 , Felix D. Schönbrodt 61 , Thomas Sellke 62 , Betsy Sinclair 6 3 , Dustin Tingley 6 4 , Trisha Van Zandt 6 5 , Simine Vazire 6 6 , Dun can J. Watts 6 7 , Christopher Winship 6 8 , Robert L. Wolpert 2 , Yu Xie 69 , Cristobal Young 7 0 , Jonathan Zinman 7 1 , Valen E. Johnson 7 2 *
}

Solutions: is it really? 
=======================================
![A solution?](./images/p-value-005-baysian-spectacles.png){ height=270px }


Must contain
=======================================
- must contain: p-hacking, p-curve, pre-registration, reviewer blurb, 
- Dorothy Bishop slide

Conclusion 1: Ioannidis again
======================================================

* Young fields tend to have less stringent criteria 
* Ioannidis 2005: When are results more likely to be false? 
    - The smaller the studies ...
    - The smaller the effect size ...
    - The larger the number of tests ...
    - The more flexibility in the analyses
    - The more trendy ...
    - The more financial interest ...

Conclusion 2: Effect-size = f(years, sample, ...)  
======================================================

![Molendijk, 2012, BDNF and hippocampal volume](./images/molendijk_2012_f4.pdf) 

$\vspace{-1.2cm}$

![Mier, 2009, COMT & DLPFC](./images/mier_2009_f4.pdf)

Acknowledgements  
======================================================

* Berkeley: M. D'Esposito, M. Brett, S. Van der Walt, J.Millman
* Pasteur: R. Toro, G. Dumas, T. Bourgeron, A. Beggiato
* Neurospin: B. Thirion, G. Varauquaux, V. Frouin, others


Thank you for your attention - Questions ?
======================================================


<!--
First slide 
======================================================

![\ ](./images/first-slide.png){ height=260px }
-->
