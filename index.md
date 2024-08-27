---
layout: default
title: Home
rank: 1
---

Welcome to the [MetaLab!](http://metacoglab.org/)


We are based primarily at the [Department of Experimental Psychology](https://www.ucl.ac.uk/pals/research/experimental-psychology/) and embedded in both the [Department of Imaging Neuroscience](https://www.fil.ion.ucl.ac.uk/) (also known as the FIL - Functional Imaging Laboratory) and the MPC, or [Max Planck Centre for Computational Psychiatry](https://www.mps-ucl-centre.mpg.de/)), all parts of University College London (UCL). We hope you have an excellent and productive time during your stay in the lab! This manual was developed by the lab PI, Steve Fleming together with other group members, and is a rough outline of how Steve expects the lab to function within the wider WCHN and UCL infrastructure (who’s rules and policies should take precedence). 


It’s inspired by several others (particularly the lab manuals of [Anne Urai](https://github.com/anne-urai/lab_wiki), [Liad Mudrik](https://people.socsci.tau.ac.il/mu/mudriklab/lab-philosophy-and-procedures/), [Mariam Aly](https://osf.io/mdh87/wiki/home/), [Trina MacMahon](https://d1uqjtzsuwlnsf.cloudfront.net/wp-content/uploads/sites/163/2016/11/McMahon_UW_Compact_Example.pdf), [Brad Voytek](https://voyteklab.com/philosophy), [Nancy Kanwisher]() and [Michael Beyer](https://docs.google.com/document/d/1Y1wzFVdp-FCoGM47okaW5eYdOOfpgXD5nM9Q7DpwAMo/edit)). In turn, we would be glad for others to make use of this manual when setting up their own groups, and have made it available under a CC-BY 4.0 license. If you can think of anything that is missing, or things that are unclear, then please let us know - ideas are always welcome!

### First steps

For details about our team, research and publications see [metacoglab.org](metacoglab.org). It is highly recommended that you read our key publications as soon as you join the lab, to get an idea of the type of questions that interest us and the different ways we approach them. You will find a list of key publications in the reading section [here](getting_started).


The work we do is strongly influenced by computational approaches to the brain and mind. As such, it’s useful to at least familiarise yourself with some of the common modeling tools and frameworks. Not all of these will be relevant to your project, but it’s likely that they will touch upon shared assumptions. In particular, Bayesian modeling of stochastic percepts, decisions and confidence estimates is a common theme, so investment here will pay dividends. An excellent starting point for these topics is the [Neuromatch Academy online course materials]( https://compneuro.neuromatch.io/tutorials/intro.html), in particular, Linear Algebra, Statistics and Bayesian Decisions. The [Neuromatch NeuroAI course](https://neuroai.neuromatch.io/tutorials/W2D5_Mysteries/student/W2D5_Intro.html) also now has a section on computational approaches to consciousness, partly taught by Steve, which is a useful starting point.


For an introduction to fMRI analysis, a good starting point is the [Handbook of Functional MRI Analysis by Poldrack, Mumford and Nichols](https://www.cambridge.org/core/books/handbook-of-functional-mri-data-analysis/8EDF966C65811FCCC306F7C916228529). This will provide the core concepts that are a feature of most analysis pipelines and packages such as SPM.


For most cognitive computational neuroscience, being able to program is also important. We use a range of programming languages for different projects (Matlab, Python, R, Julia), and try to use free open-source tools where we can. That said, Matlab is still a workhorse for many of our projects, particularly neuroimaging data analysis using SPM. Fluency in at least one core language that you can use for analysis, simulation and plotting is essential. We also often use probabilistic programming languages (STAN, JAGS, Turing) for model fitting - again, fluency in one language often means you can easily switch between different packages.

### Have a question?
![Decision tree](https://github.com/anne-urai/lab_wiki/blob/main/lab_decision_tree.png?raw=true)
_Adapted from [Jonathan Peelle](https://github.com/jpeelle/peellelab_manual/blob/master/figures/lab_decision_tree.pdf)_

### Contributing to this wiki
1. Fork the [repository](https://github.com/metacoglab/lab_wiki).
2. Clone your own fork to local
3. Edit existing `.md` files, or create a new one with the following header:
```
--- 
layout: default
title: Shortest route to the coffee machine
rank: 1
---
```
4. Add, commit and push to your fork
5. Create a PR: go to Pull Requests / New / Compare across forks and select your fork. Explain what you've added, and
 I'll incorporate your edits in the wiki.
