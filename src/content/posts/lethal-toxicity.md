---
title: "Acute Lethal Toxicity of Recreational Drugs"
description: "A visualization of of \"safety ratios\" for non-medical use of 20 common drugs."
date: 2026-04-20
tags: ["data visualization"]
draft: false
---

![test](/images/lethal-toxicity-vis.png)

## Discussion

In his 2003 study ["Comparison of acute lethal toxicity of commonly abused psychoactive substances"](https://www.researchgate.net/profile/Robert-Gable/publication/14984972_Toward_a_Comparative_Overview_of_Dependence_Potential_and_Acute_Toxicity_of_Psychoactive_Substances_Used_Nonmedically/links/557613d908aeb6d8c01aea8d/Toward-a-Comparative-Overview-of-Dependence-Potential-and-Acute-Toxicity-of-Psychoactive-Substances-Used-Nonmedically.pdf) Robert S. Gable estimates the relative acute lethal toxicity of 20 common recreational drugs. What Gable calls a "safety ratio" is very similar to a therapeutic index, which is defined by TI = LD50 / ED50, where LD50 is the lethal dose that would kill 50% of the population, and ED50 is the effective dose where the desired effects become present in 50% of the population. Gable uses the term safety ratio because "the intended application is not therapeutic."

Information about drug scheduling in the US can be found [on the DEA website](https://www.dea.gov/drug-information/drug-scheduling). The schedules for each drug in the visualization were retrieved from [this DOJ](https://www.deadiversion.usdoj.gov/schedules/orangebook/c_cs_alpha.pdf). Though safety ratio is a narrow and limited metric of harm, this visualization repeats the theme that US drug schedules do a poor job reflecting the actual danger of drugs.

Also, shoutout to [this visualization](https://64.media.tumblr.com/tumblr_l0h1njIdpX1qbw00mo1_500.jpg) of similar data that I borrowed some design elements of.

### How was lethal dose determined?

The LD50 values for the study were estimated from a combination of postmortem blood concentrations from compiled fatality databases, the administered doses reported in overdose cases, and pharmacokinetic modeling. Fatality data for a drug involving co-intoxicants or trauma were excluded.
> The LD50 values cited in Table 1 are the estimates of a customary dose for a normally healthy 70-kg adult who has not developed tolerance to the substance in question, and who does not have residues of the substance in the body from previous administrations. The estimates do not take into account factors such as environmental stressors or individual differences with respect to sex or ethnicity.

>The estimated human lethal dose of all substances was corroborated by non-human animal studies; however, for six of the substances (DMT, ketamine, LSD, marijuana, mescaline and psilocybin) fewer than three reports of human fatality were located. In this situation, the lethal dose in Table 1 is extrapolated from the animal studies. The extrapolated value, reduced by a factor of 10, is noted in the table, and a question-mark follows the related safety ratio. The clinical validity of animal models is always suspect, but the data probably provide a justifiable estimate in the absence of direct evidence.

### Limitations

The original paper is detailed in its limitations and I recommend reading it for a complete list, but below I've quoted those that I find are the most relevant and/or interesting.

> Due to inherent imprecision in toxicity assessments, it would be a flagrant misinterpretation of
the numbers ... to assume that they could be
mathematically manipulated. None the less, the range of
safety ratios is so wide that the data appear to have the
attributes of an ordinal scale. For example, we can be reasonably
sure that the safety ratio of nitrous oxide is larger
than the safety ratio of GHB. We need not assert that the
safety ratio of nitrous oxide is 20 times greater than GHB
in order to make a valid ranking.

> Acute effects do not, by definition, take into account
the health effects of chronic use. Direct acute lethality
from alcohol or nicotine is quite rare, given prevalence of
use. However, alcohol and tobacco use, along with obesity,
are among the leading long-term causes of preventable
death (WHO 2002).

> A safety ratio does not reflect serious non-lethal
sequelae that may burden the user and society. At relatively
low non-toxic levels, psychoactive substances may
induce dangerous performance decrements. LSD has a
larger safety ratio than codeine, but it would certainly not
be the drug-of-choice while operating machinery.

> The safety ratios in Table 1 do not reflect metabolic or
functional tolerance that a user might have developed. In
situations where tolerance to the reinforcing effects of the
drug increases more rapidly than to the metabolic effects
of the same or a concomitant drug, the safety ratio will
narrow.

In other words, these ratios are for otherwise healthy people without tolerances, so the level of safety reflected is most relevant to "discuss the risks associated with initial use", and "probably have less application
to treatment programs where participants tend to be
chronic users."