# Awesome Computational Psychiatry [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of resources for computational psychiatry — the application of computational and mathematical frameworks to understand, diagnose, and treat mental illness.

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

Computational psychiatry uses reinforcement learning, Bayesian inference, dynamical systems, and machine learning to model the mechanisms underlying psychiatric disorders. This list collects the papers, tools, datasets, courses, and communities that define the field.

**See also:** [comp-psych-syllabus](https://github.com/comp-psych/comp-psych-syllabus) — A 20-paper undergraduate reading list | [rl-model-zoo](https://github.com/comp-psych/rl-model-zoo) — Reference implementations of RL models used in psychiatry research

---

## Contents

- [Foundational Papers](#foundational-papers)
- [Review Papers](#review-papers)
- [Textbooks](#textbooks)
- [Online Courses & Tutorials](#online-courses--tutorials)
- [Software & Tools](#software--tools)
  - [Reinforcement Learning & Decision Modeling](#reinforcement-learning--decision-modeling)
  - [Bayesian Modeling & Probabilistic Programming](#bayesian-modeling--probabilistic-programming)
  - [Neuroimaging](#neuroimaging)
  - [EEG & Electrophysiology](#eeg--electrophysiology)
  - [Experiment Building](#experiment-building)
  - [Digital Phenotyping](#digital-phenotyping)
  - [General Scientific Computing](#general-scientific-computing)
- [Open Datasets](#open-datasets)
- [Active Research Labs](#active-research-labs)
- [Conferences & Workshops](#conferences--workshops)
- [Journals](#journals)
- [PhD Programs](#phd-programs)
- [Funding Opportunities](#funding-opportunities)
- [Community](#community)

---

## Foundational Papers

*The papers that established computational psychiatry as a field.*

- [Computational psychiatry (Montague et al., 2012)](https://doi.org/10.1016/j.tics.2011.11.018) — The manifesto that defined the field: psychiatric disorders as aberrant computations across biological scales.
- [Computational psychiatry as a bridge from neuroscience to clinical applications (Huys et al., 2016)](https://doi.org/10.1038/nn.4238) — Assesses how RL, Bayesian inference, and dynamical systems illuminate psychiatric mechanisms.
- [Computational approaches to psychiatry (Stephan & Mathys, 2014)](https://doi.org/10.1016/j.conb.2013.12.007) — Introduces "computational assays" and the Hierarchical Gaussian Filter for clinical modeling.
- [From reinforcement learning models to psychiatric and neurological disorders (Maia & Frank, 2011)](https://doi.org/10.1038/nn.2723) — Maps RL model parameters to symptoms in Parkinson's, ADHD, schizophrenia, and addiction.
- [Towards a mathematically informed understanding of mental illness (Adams et al., 2016)](https://doi.org/10.1136/jnnp-2015-310737) — Technical walkthrough of RL and predictive coding as applied to depression and schizophrenia.
- [A roadmap for the development of applied computational psychiatry (Paulus et al., 2016)](https://doi.org/10.1016/j.bpsc.2016.05.001) — Pragmatic roadmap for moving computational models from research to clinical tools.
- [Computational modeling in psychiatry: a brief introduction (O'Doherty et al., 2007)](https://doi.org/10.1016/j.tics.2007.02.009) — An early tutorial on applying decision-making models to psychiatric questions.

## Review Papers

*Comprehensive reviews spanning subfields and methods.*

- [Reinforcement learning and Tourette syndrome (Maia & Frank, 2011)](https://doi.org/10.1016/j.conb.2011.01.008) — Computational account of aberrant action selection in Tourette syndrome via basal ganglia circuits.
- [Computational and mathematical models of psychopathology (Huys et al., 2011)](https://doi.org/10.1016/j.jmp.2011.02.003) — Foundational review of formal models applied to anxiety, depression, and psychosis.
- [Depression, stress, and anhedonia: toward a synthesis and integrated model (Pizzagalli, 2014)](https://doi.org/10.1146/annurev-clinpsy-050212-185606) — Reviews how stress disrupts dopamine-based reward learning in depression.
- [Neuroscience of apathy and anhedonia: a transdiagnostic approach (Husain & Roiser, 2018)](https://doi.org/10.1038/s41583-018-0029-9) — Bridges RL models to effort-based decision-making tasks for motivational deficits.
- [Hallucinations and strong priors (Corlett et al., 2019)](https://doi.org/10.1016/j.tics.2018.12.001) — Predictive coding account of hallucinations as overweighted prior beliefs.
- [Machine learning approaches for clinical psychology and psychiatry (Dwyer et al., 2018)](https://doi.org/10.1146/annurev-clinpsy-032816-045037) — Honest review of where ML has succeeded and failed in psychiatric classification.
- [Dissecting racial bias in an algorithm used to manage the health of populations (Obermeyer et al., 2019)](https://doi.org/10.1126/science.aax2342) — Landmark study on algorithmic bias in healthcare with direct implications for computational psychiatry.
- [Whatever next? Predictive brains, situated agents, and the future of cognitive science (Clark, 2013)](https://doi.org/10.1017/S0140525X12000477) — Theoretical foundation for predictive coding and the Bayesian brain hypothesis.
- [Computing schizophrenia: ethical challenges for machine learning in psychiatry (Starke et al., 2020)](https://doi.org/10.1017/S0033291720001683) — Ethics of algorithmic psychiatry: false positives, stigma, and bias.
- [Invasive computational psychiatry (Saez & Gu, 2023)](https://doi.org/10.1016/j.biopsych.2022.09.032) — Using intracranial recordings to model neural computations underlying psychiatric symptoms.

## Textbooks

- [Computational Psychiatry: New Perspectives on Mental Illness — Redish & Gordon, eds. (2016, MIT Press)](https://mitpress.mit.edu/9780262035422/computational-psychiatry/) — The first textbook dedicated to the field.
- [An Introduction to Model-Based Cognitive Neuroscience — Forstmann & Wagenmakers, eds. (2015, Springer)](https://doi.org/10.1007/978-1-4939-2236-9) — Mathematical foundations for cognitive modeling.
- [Bayesian Cognitive Modeling: A Practical Course — Lee & Wagenmakers (2014, Cambridge)](https://bayesmodels.com/) — Bayesian modeling with code exercises and companion site.
- [Reinforcement Learning: An Introduction — Sutton & Barto (2018, MIT Press)](http://incompleteideas.net/book/the-book-2nd.html) — The standard RL textbook, freely available online.
- [Statistical Rethinking — McElreath (2020, CRC Press)](https://xcelab.net/rm/statistical-rethinking/) — Bayesian statistics with practical R and Stan examples.
- [Pattern Recognition and Machine Learning — Bishop (2006, Springer)](https://www.microsoft.com/en-us/research/publication/pattern-recognition-machine-learning/) — Classic ML textbook covering probabilistic graphical models and inference.
- [Theoretical Neuroscience — Dayan & Abbott (2001, MIT Press)](https://mitpress.mit.edu/9780262541855/theoretical-neuroscience/) — Foundational computational neuroscience textbook.

## Online Courses & Tutorials

- [Neuromatch Academy — Computational Neuroscience](https://compneuro.neuromatch.io/) — Full computational neuroscience curriculum with interactive Python tutorials, free and annual.
- [Coursera — Computational Neuroscience (University of Washington)](https://www.coursera.org/learn/computational-neuroscience) — Introductory course covering neural coding, networks, and learning.
- [Computational Models of Behavior — Wilson & Collins (2019)](https://doi.org/10.1038/s41562-019-0732-0) — Essential tutorial on fitting RL models to behavioral data.
- [Hitchhiker's Guide to fMRI (Andy's Brain Book)](https://andysbrainbook.readthedocs.io/) — Practical fMRI analysis tutorials covering FSL, SPM, FreeSurfer, and AFNI.
- [Stan User's Guide and Reference Manual](https://mc-stan.org/users/documentation/) — Complete documentation for Bayesian modeling in Stan.
- [MNE-Python Tutorials](https://mne.tools/stable/auto_tutorials/index.html) — Step-by-step EEG/MEG analysis tutorials.
- [Nilearn Tutorials](https://nilearn.github.io/stable/auto_examples/index.html) — Machine learning for neuroimaging with worked examples.
- [jsPsych Tutorials](https://www.jspsych.org/latest/tutorials/hello-world/) — Getting started with browser-based behavioral experiments.
- [PyMC Examples Gallery](https://www.pymc.io/projects/examples/en/latest/gallery.html) — Annotated examples for Bayesian modeling in Python.

## Software & Tools

### Reinforcement Learning & Decision Modeling

- [hBayesDM](https://ccs-lab.github.io/hBayesDM/) — Hierarchical Bayesian modeling of decision-making tasks with Stan backend (R/Python).
- [TAPAS (HGF Toolbox)](https://www.tnu.ethz.ch/en/software/tapas) — Hierarchical Gaussian Filter for computational modeling of perception and learning (MATLAB).
- [VBA Toolbox](https://mbb-team.github.io/VBA-toolbox/) — Variational Bayesian Analysis for model inversion, comparison, and simulation (MATLAB).
- [RLax](https://github.com/google-deepmind/rlax) — JAX-based library of reinforcement learning building blocks from DeepMind.
- [Gymnasium](https://gymnasium.farama.org/) — Standard API for reinforcement learning environments, successor to OpenAI Gym.
- [Stable-Baselines3](https://stable-baselines3.readthedocs.io/) — Reliable implementations of RL algorithms in PyTorch.
- [comp-psych/rl-model-zoo](https://github.com/comp-psych/rl-model-zoo) — Reference implementations of RL models used in computational psychiatry research.

### Bayesian Modeling & Probabilistic Programming

- [Stan](https://mc-stan.org/) — Probabilistic programming language for Bayesian inference with MCMC and variational methods.
- [PyMC](https://www.pymc.io/) — Probabilistic programming in Python with MCMC and variational inference.
- [brms](https://paul-buerkner.github.io/brms/) — Bayesian regression modeling in R using a Stan backend.
- [ArviZ](https://python.arviz.org/) — Exploratory analysis and diagnostics for Bayesian models (Python).
- [NumPyro](https://num.pyro.ai/) — Probabilistic programming with JAX for fast Bayesian inference.
- [Turing.jl](https://turinglang.org/) — Bayesian inference and probabilistic programming in Julia.
- [BayesFlow](https://github.com/stefanradev93/BayesFlow) — Amortized Bayesian inference with neural networks for simulation-based models.

### Neuroimaging

- [fMRIPrep](https://fmriprep.org/) — Standardized, robust fMRI preprocessing pipeline.
- [MRIQC](https://mriqc.readthedocs.io/) — Automated quality control for structural and functional MRI data.
- [Nilearn](https://nilearn.github.io/) — Machine learning for neuroimaging in Python — decoding, connectivity, atlas-based analysis.
- [FreeSurfer](https://surfer.nmr.mgh.harvard.edu/) — Cortical surface reconstruction and subcortical segmentation.
- [FSL](https://fsl.fmrib.ox.ac.uk/) — Comprehensive fMRI and diffusion analysis suite (FEAT, MELODIC, TBSS).
- [SPM](https://www.fil.ion.ucl.ac.uk/spm/) — Statistical Parametric Mapping for voxelwise GLM, DCM, and VBM (MATLAB).
- [AFNI](https://afni.nimh.nih.gov/) — Neuroimaging analysis suite from NIMH — preprocessing, statistics, visualization.
- [NiMARE](https://nimare.readthedocs.io/) — Neuroimaging meta-analysis in Python (ALE, MKDA, BrainMap).
- [CONN](https://web.conn-toolbox.org/) — Functional connectivity analysis toolbox for fMRI (MATLAB/SPM).
- [ANTsPy](https://antspy.readthedocs.io/) — Advanced normalization tools for neuroimaging in Python.
- [Templateflow](https://www.templateflow.org/) — Archive of brain templates and atlases in standard formats for neuroimaging.

### EEG & Electrophysiology

- [MNE-Python](https://mne.tools/) — EEG/MEG analysis — preprocessing, source localization, time-frequency, connectivity.
- [EEGLAB](https://sccn.ucsd.edu/eeglab/) — EEG analysis toolbox with ICA, time-frequency, and plugin ecosystem (MATLAB).
- [FieldTrip](https://www.fieldtriptoolbox.org/) — MATLAB toolbox for MEG, EEG, and intracranial electrophysiology analysis.
- [Brainstorm](https://neuroimage.usc.edu/brainstorm/) — Collaborative platform for MEG/EEG analysis with GUI and scripting support.

### Experiment Building

- [PsychoPy](https://www.psychopy.org/) — Build behavioral experiments in Python — timing-precise, fMRI/EEG compatible.
- [jsPsych](https://www.jspsych.org/) — Run behavioral experiments in the browser for online data collection.
- [Prolific](https://www.prolific.com/) — Recruit diverse, vetted participants for online behavioral studies.
- [Gorilla](https://gorilla.sc/) — No-code online experiment builder and hosting platform.
- [Pavlovia](https://pavlovia.org/) — Online hosting for PsychoPy experiments with built-in participant management.
- [oTree](https://www.otree.org/) — Framework for interactive behavioral experiments, games, and surveys.
- [Lab.js](https://lab.js.org/) — Free, open-source online experiment builder with a visual interface.

### Digital Phenotyping

- [mindLAMP](https://www.digitalpsych.org/lamp) — Digital phenotyping platform for smartphone-based psychiatric research.
- [Beiwe](https://www.beiwe.org/) — Research platform for smartphone-based digital phenotyping with passive data collection.
- [AWARE](https://awareframework.com/) — Open-source context instrumentation framework for mobile sensing research.

### General Scientific Computing

- [NumPy](https://numpy.org/) — Fundamental package for numerical computing in Python.
- [SciPy](https://scipy.org/) — Scientific computing library for optimization, integration, interpolation, and statistics.
- [pandas](https://pandas.pydata.org/) — Data manipulation and analysis library for Python.
- [scikit-learn](https://scikit-learn.org/) — Machine learning library for classification, regression, clustering, and dimensionality reduction.
- [Matplotlib](https://matplotlib.org/) — Comprehensive 2D plotting library for Python.
- [seaborn](https://seaborn.pydata.org/) — Statistical data visualization built on Matplotlib.
- [Jupyter](https://jupyter.org/) — Interactive computing environment for reproducible research notebooks.
- [R](https://www.r-project.org/) — Statistical computing language widely used in psychology and neuroscience.

## Open Datasets

### Psychiatric & Clinical

- [DAIC-WOZ](https://dcapswoz.ict.usc.edu/) — 189 clinical interviews with PHQ-8 depression scores, audio, video, and transcripts.
- [STAR*D](https://www.nimh.nih.gov/funding/clinical-research/practical/stard) — 4,041 MDD patients with sequential treatment outcomes — the largest antidepressant trial.
- [COBRE](http://fcon_1000.projects.nitrc.org/indi/retro/cobre.html) — 72 schizophrenia + 75 healthy controls with resting-state fMRI and clinical assessments.
- [UCLA CNP (ds000030)](https://openneuro.org/datasets/ds000030) — 272 subjects with task fMRI across schizophrenia, bipolar, ADHD, and healthy controls.
- [PhysioNet](https://physionet.org/) — Physiological signal databases (EEG, ECG, EMG) and clinical datasets including MIMIC-IV.

### Brain Imaging Repositories

- [OpenNeuro](https://openneuro.org/) — 900+ neuroimaging datasets (fMRI, EEG, MEG) in BIDS format.
- [Human Connectome Project (HCP)](https://www.humanconnectome.org/) — 1,200 subjects with high-resolution fMRI, diffusion imaging, and behavioral data.
- [UK Biobank](https://www.ukbiobank.ac.uk/) — 500K participants with brain imaging, genetics, and health records.
- [NeuroVault](https://neurovault.org/) — Repository of unthresholded statistical brain maps from published studies.
- [NeuroSynth](https://neurosynth.org/) — Automated meta-analysis platform with 15K+ studies and coordinate-based maps.
- [ENIGMA Consortium](https://enigma.ini.usc.edu/) — Meta-analytic neuroimaging consortium spanning 50+ disorders.

### Developmental & Longitudinal

- [ABCD Study](https://abcdstudy.org/) — 12,000 adolescents with longitudinal brain, behavioral, and environmental data.
- [Philadelphia Neurodevelopmental Cohort (PNC)](https://www.med.upenn.edu/bbl/philadelphianeurodevelopmentalcohort.html) — 9,498 youth (8–21) with neuroimaging, genetics, cognitive, and clinical phenotyping.
- [Healthy Brain Network](https://healthybrainnetwork.org/) — 10,000 children (5–21) with EEG, MRI, behavioral, clinical, and digital phenotyping data.

### Genomics & Transcriptomics

- [PsychENCODE](https://www.psychencode.org/) — Transcriptomic and epigenomic data from human brains across psychiatric conditions.
- [All of Us (NIH)](https://allofus.nih.gov/) — 1M+ diverse participants with genomics, EHR, wearables, and surveys.
- [NIMH Data Archive (NDA)](https://nda.nih.gov/) — Central repository for NIMH-funded research data including imaging, genomics, and clinical measures.
- [Psychiatric Genomics Consortium](https://pgc.unc.edu/) — Large-scale GWAS meta-analyses for psychiatric disorders.

## Active Research Labs

*Labs with active computational psychiatry research programs, organized by institution.*

### ETH Zurich / University of Zurich
- [Translational Neuromodeling Unit (Klaas Stephan)](https://www.tnu.ethz.ch/) — Generative modeling, computational assays, TAPAS toolbox.

### Harvard University
- [Niv Lab — Yael Niv (Princeton, now Harvard)](https://nivlab.princeton.edu/) — Reinforcement learning, attention, and latent-state inference in psychiatric populations.

### Icahn School of Medicine at Mount Sinai
- [Center for Computational Psychiatry (Xiaosi Gu)](https://www.mountsinai.org/profiles/xiaosi-gu) — Interoception, social decision-making, computational modeling of psychiatric symptoms.

### Max Planck Institute for Biological Cybernetics
- [Computational Psychiatry Group (Christoph Mathys)](https://www.aesthetics.mpg.de/en/the-institute/people/christoph-mathys.html) — Hierarchical Gaussian Filter, Bayesian learning models.

### Princeton University
- [Computational Memory Lab (Ken Norman)](https://compmem.princeton.edu/) — Memory, context reinstatement, and their links to psychopathology.

### UCL (University College London)
- [Max Planck UCL Centre for Computational Psychiatry (Ray Dolan)](https://www.mpc-ucl.com/) — Foundational computational psychiatry center.
- [Emotion and Decision-Making Lab (Quentin Huys)](https://www.quentinhuys.com/) — Computational models of depression, learning, and planning.

### University of Cambridge
- [Brain Mapping Unit (Ed Bullmore)](https://www.psychiatry.cam.ac.uk/groups/brain-mapping-unit/) — Network neuroscience and computational approaches to psychiatric disorders.

### University of Oxford
- [Wellcome Centre for Integrative Neuroimaging](https://www.win.ox.ac.uk/) — Advanced neuroimaging methods with applications to psychiatry.

### University of Pittsburgh
- [Laboratory of Computational and Translational Psychiatry (Alexandre Bhatt)](https://lncd.pitt.edu/) — Developmental computational psychiatry and decision-making.

### University of Texas at Austin
- [Computational Psychiatry Unit (Maia & O'Doherty's collaborators)](https://liberalarts.utexas.edu/psychology/) — RL-based computational approaches to psychopathology.

### Yale University
- [Corlett Lab (Phil Corlett)](https://medicine.yale.edu/lab/corlett/) — Computational models of belief, delusions, and hallucinations.
- [Computational Psychiatry Lab (Alan Anticevic)](https://medicine.yale.edu/lab/anticevic/) — Large-scale neural circuit modeling in psychosis and mood disorders.

## Conferences & Workshops

- [Computational Psychiatry Conference (CPC)](https://www.cpconf.org/) — Annual conference dedicated to computational psychiatry, hosted by Xiaosi Gu's group.
- [Society for Biological Psychiatry (SOBP)](https://sobp.org/) — Annual meeting with computational psychiatry tracks.
- [Society for Neuroscience (SfN)](https://www.sfn.org/) — Nanosymposia and themed sessions in computational approaches to psychiatry.
- [Organization for Human Brain Mapping (OHBM)](https://www.humanbrainmapping.org/) — Annual meeting covering neuroimaging methods applied to psychiatry.
- [Cognitive Computational Neuroscience (CCN)](https://ccneuro.org/) — Conference bridging computational neuroscience and cognitive science.
- [Neuromatch Conference](https://conference.neuromatch.io/) — Open, online computational neuroscience conference.
- [ACNP (American College of Neuropsychopharmacology)](https://acnp.org/) — Annual meeting covering neuropharmacology with computational sessions.

## Journals

- [Computational Psychiatry](https://computationalpsychiatry.org/) — Dedicated journal for the field (Editor-in-Chief: Xiaosi Gu).
- [Biological Psychiatry: Cognitive Neuroscience and Neuroimaging](https://www.journals.elsevier.com/biological-psychiatry-cognitive-neuroscience-and-neuroimaging) — Leading journal for neuroimaging and computational approaches in psychiatry.
- [Biological Psychiatry](https://www.journals.elsevier.com/biological-psychiatry) — Premier biological psychiatry journal.
- [Nature Neuroscience](https://www.nature.com/neuro/) — High-impact neuroscience journal publishing computational psychiatry work.
- [PNAS](https://www.pnas.org/) — Broad-scope journal with influential computational psychiatry papers.
- [Psychological Medicine](https://www.cambridge.org/core/journals/psychological-medicine) — Clinical psychiatry journal with computational modeling papers.
- [JAMA Psychiatry](https://jamanetwork.com/journals/jamapsychiatry) — Top-tier clinical psychiatry journal.
- [Nature Reviews Neuroscience](https://www.nature.com/nrn/) — Authoritative review journal covering computational approaches to the brain.
- [Neuron](https://www.cell.com/neuron/home) — Leading neuroscience journal publishing computational work relevant to psychiatry.
- [eLife](https://elifesciences.org/) — Open-access journal publishing rigorous computational neuroscience research.

## PhD Programs

*Programs with faculty and infrastructure supporting computational psychiatry research.*

- [UCL Max Planck Centre for Computational Psychiatry & Ageing Research](https://www.mpc-ucl.com/) — Dedicated computational psychiatry PhD program in London.
- [ETH Zurich — Neural Systems and Computation](https://www.ini.uzh.ch/en/teaching/phd.html) — PhD program at the Institute of Neuroinformatics with computational psychiatry faculty.
- [Yale University — Interdepartmental Neuroscience Program](https://medicine.yale.edu/inp/) — Access to computational psychiatry labs (Corlett, Anticevic).
- [Princeton Neuroscience Institute](https://pni.princeton.edu/) — PhD program with strong computational foundations and clinical collaborations.
- [Harvard/MIT — Computational and Systems Biology](https://csb.harvard.edu/) — Quantitative PhD with pathways into computational psychiatry.
- [Mount Sinai — Neuroscience PhD Program](https://icahn.mssm.edu/education/phd/neuroscience) — Home of the Center for Computational Psychiatry.
- [University of Cambridge — MRC Cognition and Brain Sciences Unit](https://www.mrc-cbu.cam.ac.uk/) — PhD opportunities with computational psychiatry supervision.
- [Karolinska Institutet — Doctoral Programme in Clinical Neuroscience](https://ki.se/en/research/doctoral-education) — European hub for computational approaches to psychiatry.

## Funding Opportunities

- [NIMH (National Institute of Mental Health)](https://www.nimh.nih.gov/funding) — Primary US funder of computational psychiatry research.
- [NIMH Intramural Research Program — Summer Internship (SIP)](https://www.nimh.nih.gov/research/training/summer-internship-program) — Summer research positions at NIMH for undergrads and post-bacs.
- [NIH BRAIN Initiative](https://braininitiative.nih.gov/) — Funding for brain research technologies including computational approaches.
- [Wellcome Trust — Mental Health Priority Area](https://wellcome.org/what-we-do/mental-health) — Major international funder of mental health research including computational methods.
- [NSF — Cognitive Neuroscience Program](https://www.nsf.gov/funding/pgm_summ.jsp?pims_id=5316) — US funding for computational approaches to cognition and brain function.
- [European Research Council (ERC)](https://erc.europa.eu/) — Competitive grants supporting computational psychiatry research in Europe.
- [Brain & Behavior Research Foundation (NARSAD Grants)](https://www.bbrfoundation.org/) — Young Investigator and Independent Investigator grants for mental health research.

## Community

- [Neurostars](https://neurostars.org/) — Q&A forum for neuroimaging, computational neuroscience, and analysis tools.
- [Neuromatch](https://neuromatch.io/) — Global computational neuroscience community with courses, conferences, and mentorship.
- [OHBM BrainHack](https://ohbm.github.io/hackathon/) — Annual hackathon for neuroimaging tool development and collaboration.
- [BrainHack Global](https://brainhack.org/) — Worldwide hackathon series for neuroscience tool development and open science.
- [Open Science Framework (OSF)](https://osf.io/) — Platform for sharing research data, preprints, and preregistrations.
- [ReproNim](https://www.repronim.org/) — Center for reproducible neuroimaging computation.
- [INCF (International Neuroinformatics Coordinating Facility)](https://www.incf.org/) — Organization promoting open and FAIR neuroscience.

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on adding resources, suggesting categories, or reporting broken links.

## Related Lists

- [comp-psych-syllabus](https://github.com/comp-psych/comp-psych-syllabus) — A 20-paper undergraduate syllabus for computational psychiatry
- [rl-model-zoo](https://github.com/comp-psych/rl-model-zoo) — Reference implementations of RL models used in computational psychiatry
- [awesome-neuroscience](https://github.com/analyticalmonk/awesome-neuroscience) — Curated list of neuroscience libraries, software, and resources

---

**Curated by [Peter Zhou](https://github.com/peterzhou)** — Founder, PRAXIS (Psychiatry Research, Analytics & eXperimental Innovation Society) at USC | NIH Summer Intern, NIMH ETPB

*Licensed under [CC BY 4.0](LICENSE). Last updated: June 2026.*
