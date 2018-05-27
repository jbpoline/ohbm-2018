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
\ 
======================================================

![\ ](./images/first-slide.png){ height=260px }

Plan
=================================================================================

- what is/are the pb?
	- is Ioannidis right?
	- technical 
	- sociological

Issues of reproducibility in sciences 
=================================================================================
![Stodden, 2014](./images/credibility-crisis.png){ height=240px }

<!-- Say that still, many people do not take this seriously: this is only other researchers problem, not mine -->


- historical perspective
	- when did we start to talk of the pb


- technical: what is a p-value
	- westwall (questionaire)
	- 

- social: the life science curse
	- publications only with p<.05 
	- reviewers dont believe:
		- 
	
- examples
	- Russ meta analyses wrong paper
	- all food are cancerogene 

- consequences: Button et al
	- inflated effect sizes
	- decreased PPV 

- the reactions: 
	- APS ban
	- long list of checkboxes in nature publications
	- nature statistician review

- the solutions
	- social 
	- technical (Bayesian)
	- socio-technical 


Solutions: redefine significance
=======================================

## Abstract

\large{"We propose to change the default P-value threshold for
statistical significance for claims of new discoveries from 0.05 to 0.005."}

\tiny{Daniel J. Benjamin 1 *, James O. Berger 2 , Magnus Johannesson 3 *, Brian A.  Nose k 4, 5 , E.  - J.  W agenma k er s 6 , Richard Ber k 7, 1 0 , K enneth A.  Bollen 8 , Björn Bremb s 9 , Lawrence Brown 10 , Colin Camerer 11 , David Cesarini 12, 13 , Christopher D. Chambers 14 , Merlise Clyde 2 , Thomas D. Cook 15,16 , Paul De Boeck 17 , Zoltan Dienes 18 , Anna Dreber 3 , Kenny Easwaran 19 , Charles Efferson 20 , Ernst Fehr 21 , Fiona Fidler 22 , Andy P.  Field 18 , Malcolm Forster 23 , Edward I. George 10 , Richard Gonzalez 24 , Steven Goodman 25 , Edwin Green 26 , Donald P.  Green 27 , Anthony Greenwald 28 , Jarrod D. Hadfield 29 , Larry V.  Hedges 30 , Leonhard Held 31 , Teck Hua Ho 32 , Herbert Hoijtink 33 , James Holland Jones 39,40 , Daniel J. Hruschka 34 , Kosuke Imai 35 , Guido I mbens 36 , John P.A.  Ioannidis 37 , Minjeong Jeon 38 , Michael Kirchler 41 , David Laibson 42 , John List 43 , Roderick Little 44 , Arthur Lupia 45 , Edouard Machery 46 , Scott E. Maxwell 47 , Michael McCarthy 48 , Don Moore 49 , Stephen L. Morgan 50 , Marcus Munafó 51, 52 , Shinichi Nakagawa 53 , Brendan Nyhan 54 , Timothy H. Parker 55 , Luis Pericchi 56 , Marco Perugini 57 , Jeff Rouder 58 , Judith Rousseau 59 , Victoria Savalei 60 , Felix D. Schönbrodt 61 , Thomas Sellke 62 , Betsy Sinclair 6 3 , Dustin Tingley 6 4 , Trisha Van Zandt 6 5 , Simine Vazire 6 6 , Dun can J. Watts 6 7 , Christopher Winship 6 8 , Robert L. Wolpert 2 , Yu Xie 69 , Cristobal Young 7 0 , Jonathan Zinman 7 1 , Valen E. Johnson 7 2 *
}


Solutions: is it really? 
=======================================

![A solution?](./images/p-value-005-baysian-spectacles.png){ height=240px }


# must contain
- must contain: p-hacking, p-curve, pre-registration, reviewer blurb, 
- Dorothy Bishop slide
- 


Acknowledgements  
======================================================

* Berkeley: M. D'Esposito, M. Brett, S. Van der Walt, J.Millman
* Pasteur: R. Toro, G. Dumas, T. Bourgeron, A. Beggiato
* Neurospin: B. Thirion, G. Varauquaux, V. Frouin, others






<!--
Genetic variations: 
===========================

![Scherer 2007, Credit S. Cichon](./images/genetic-variations.png){ height=240px }

Genetic variation: SNP
========================

![Credit S. Cichon](./images/SNP.png){ height=240px }

Genetic variation: CNV
========================

![Credit S. Cichon](./images/CNV.png){ height=240px }

The imaging genetic studies
===================================

- One variant, small Ns 
- GWAS, small then large Ns
- Genome-wide-Brain-wide
- Multivariate analyses
- [Heritability] 
- Networks
- Interpretation 

Some first studies: small Ns
==============================

![Hariri et al. Science, 2002](./images/hariri.png){ height=200px }
$\vspace{-0.10cm}$

* Authors report $m_1 = .28, m_2 = .03, \textrm{SDM}_1 = 0.08, \textrm{SDM}_2 = 0.05, N_1 = N_2 = 14$ 
* How do we compute the effect size ?  

Computing effect size
========================

What is the effect ?
---------------------

$\hspace{3cm}\mu = \bar{x_1} - \bar{x_2}$

What is the standardized effect ? (eg Cohen's d)
-------------------------------------------------

$\hspace{3cm}d = \frac{\bar{x_1} - \bar{x_2}}{\sigma} = \frac{\mu}{\sigma}$

"Z" : Effect accounting for the sample size 
--------------------------------------------------

$\hspace{3cm}Z = \frac{\mu}{\sigma / \sqrt{n}}$

Computing Effect size: practice
================================

* First, compute the standard deviation of the data from the $\textrm{SDM}$ 

    - get $\sigma$ from $\textrm{SDM}$ : $\sigma = \sqrt{14-1}\times\textrm{SDM}$
    - Combine the $\sigma$ to have one estimation across the groups
        - formula easy to recompute or find
    - $\sigma = \sqrt{14-1}\times\textrm{SDM}$, $d = \frac{m_1 - m_2}{\sigma} = 1.05$ 
\pause
\vspace{.4cm}
    - What is the percentage of variance explained ? 
\pause
\vspace{.4cm}
    - Write the estimated model: $Y = [1 \ldots 1]^t [m_1-m_2] + \textrm{residual}$
    - Compute the total sum of square $Y^t Y$, then the proportion: 
\pause
\vspace{.2cm}
    - \Large{$V_e = \frac{(n_1 + n_2)(m_1-m_2)^2}{n_1 s_1^2 + n_2 s_2^2 + (n_1 + n_2)(m_1-m_2)^2} > 40\%$}

Multiple hypothesis: the curse of GWAS--wise...
======================================================

![Shen et al., 2010](./images/gwas-right-hypo-GM-N=733-shen-2010.png){ height=200px }

- \small{See also Stein et al., 2010 (SNP X Voxel), Hibar et al., 2011, (Gene X Voxel) }

Computing effect size in imaging genetics (2)
===============================================

\begin{itemize}
\item Example of Shen et al using the ADNI cohort: Association of SNPs and the amount of GM in the hippocampus.
\pause
\item N = 733 subjects,  considered a large study for imaging, but a very small one for genome wide association. 
\pause
\item only APOE gene confirmed, p =  6.63e-10: reaches GWAS significance level of 5.e-8
\pause
\item Question: How would you compute the effect size for APOE ? 
   \begin{itemize}
   \pause
   \item  What is the Z score for p =  6.63e-10 ? : p-to-Z(6.63e-10) = 6.064
   \pause
   \item  From Z score to Cohen's d ?  6.064/sqrt(733) = 0.224
   \end{itemize}
\pause
\item Question: what is the power for p=5.e-8 and d=0.22, N=733? 
\end{itemize}


Effect size in imaging genetics
=================================

\begin{itemize}
    \item BDNF val/met and hippocampal volume: genuine effect or winners curse? d=0.13, p=0.02, Molendijk (2012)
\pause
    \item Stein et al, 2012: marker is associated with 0.58\% of intracranial volume per risk allele
\pause
    \item Flint 2014: Effect size of intermediate phenotype not much greater than others !
\pause
    \item For psychiatric diseases: mean OR is 1.15, QT: variance explained by 1 locus << 0.5\% and 0.1-0.3\% for protein or serum concentration 
\pause
    \item Franke et al., 2015: volume of hippocampus: -23 mm3 per SNP allele (~0.7\%) and OR=0.94 for schizophrenia vs control.
\end{itemize}

Some example of SNP effect size
=================================

![Franke et al., 2015](./images/franke-2015-effect-size.png){ height=230px }

<!-- - \small{Franke et al., 2015 } -->

Effect size and reproducibility?
==========================================

\begin{itemize}
    \item HTTLPR and amygdala: Hariri 2002: p-value implies that locus explain > 40\% of phenotypic variance. d=1.05
    \item COMT and DLPFC: meta analysis : d = 0.55,  most studies N < 62 subjects (Meir, 2010) 
    \item KCTD8 / cortical area: Paus 2012: 21\% of phenotypic variance (250 subjects), d=1.03.
\end{itemize}

Multivariate approaches 1 
======================================================

* Why ? Effect of several genes - Effect on several regions

![J. Liu et al, 2009](./images/multivariate-snp-fMRI.png){ height=170px }

* Review: Calhoun et al., 2009. Application to Schizophrenia.

<!-- J. Liu et al., ICA guided Schizophrenia -->

Multivariate approaches 2
======================================================
<!-- $\vspace{-1.2cm}$ -->

![Vounou et al, 2010, LeFloch et al., 2012](./images/imaging-genetics-multivariate.png){ height=200px }


Multivariate analyses: what do you get 
======================================================

![Vounou et al, 2010, LeFloch et al., 2012](./images/lefloch_2012_sPLS_results.png){ height=200px }

* Then: issues of interpretation - and statistics needed to determine which region/voxel and which SNP/gene can be reported

Heritability : more constraints - more interpretable
======================================================

* Definition (simple): percentage of variance due to genetic

![Toro et al, 2014](./images/toro-gcta-heritability.png){ height=200px }


Networks
======================================================

![Network SNP/Diffusion Chiang et al 2012](./images/network-diffusion-chiang-2012.png){ height=200px }

* See also Silver et al., 2012: Pathways, Richiardi 2015

<!--
Interpretation / Validation
======================================================

![Richiardi et al, 2015](./images/richiardi-2015-connectivity.png){ height=150px }

* Resting state networks in fMRI related to Allen Brain 
	- "Validation" on SNP / fMRI  
	- "Validation" on the mouse data

-->

A few specificities of Imaging Genetics
========================================

- Combinaison of imaging and of genetics potential pre-processing issues  
- Large number of subjects is necessary for GWAS and but too costly to scan  
- The multiple comparison issues
- The flexibility of analyses / exploration
- The "trendiness" of the field
- The capacity to "rationalize findings" 
    - noise in brain images is always interpretable
    - genes are always interpretable

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






Thank you for your attention - Questions ?
======================================================

-->
