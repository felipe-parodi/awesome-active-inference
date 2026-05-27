# Awesome Active Inference [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated reading list for **Active Inference** and the **Free Energy Principle (FEP)**, spanning both **cognitive science / neuroscience** and **artificial intelligence / machine learning**. It is built to take you from zero to research literacy.

Active Inference is a "first-principles" account of perception, action, and learning in which agents act to minimize *variational free energy* (a bound on surprise) under a generative model of their world. It grew out of Karl Friston's work in theoretical neuroscience and is now used across neuroscience, psychology, robotics, and AI.

**How to use this list.** If you are new, start with [Start Here](#start-here), which gives two short on-ramps: one for readers from neuroscience/cognitive science, one for readers from AI/ML. After that, each thematic section is ordered **chronologically (oldest first)** so you can follow how the ideas developed. Books are noted as such; everything else is a paper unless stated otherwise.

## Contents

- [Start Here](#start-here)
- [Textbooks](#textbooks)
- [Tutorials and Reviews](#tutorials-and-reviews)
- [Foundational Papers: The Free Energy Principle](#foundational-papers-the-free-energy-principle)
- [Predictive Coding](#predictive-coding)
- [Active Inference: Discrete State-Spaces](#active-inference-discrete-state-spaces)
- [Active Inference: Continuous Time, Control, and Robotics](#active-inference-continuous-time-control-and-robotics)
- [Deep Active Inference and AI](#deep-active-inference-and-ai)
- [Neuroscience and Computational Psychiatry](#neuroscience-and-computational-psychiatry)
- [Philosophy and Foundations](#philosophy-and-foundations)
- [Courses, Lectures, and Videos](#courses-lectures-and-videos)
- [Software and Libraries](#software-and-libraries)
- [Blogs, Explainers, and Visualizations](#blogs-explainers-and-visualizations)
- [Communities, People, and Organizations](#communities-people-and-organizations)
- [Useful Resources and Related Lists](#useful-resources-and-related-lists)
- [Contributing](#contributing)
- [License](#license)

## Start Here

New to the topic? Pick the on-ramp that matches your background. Both converge on the same core: the [textbook](#textbooks) and the [process-theory paper](#foundational-papers-the-free-energy-principle).

**Coming from neuroscience / cognitive science:**

1. Bogacz (2017), *A tutorial on the free-energy framework for modelling perception and learning* — the gentlest mathematical introduction, with MATLAB code. [PMC](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5341759/)
2. Friston (2009), *The free-energy principle: a rough guide to the brain?* — accessible high-level framing. [PDF](https://www.fil.ion.ucl.ac.uk/~karl/The%20free-energy%20principle%20-%20a%20rough%20guide%20to%20the%20brain.pdf)
3. Friston (2010), *The free-energy principle: a unified brain theory?* — the influential synthesis. [Nature](https://www.nature.com/articles/nrn2787)
4. Parr, Pezzulo, and Friston (2022), *Active Inference* (textbook, Part I). [MIT Press, open access](https://direct.mit.edu/books/oa-monograph/5299/Active-InferenceThe-Free-Energy-Principle-in-Mind)

**Coming from AI / machine learning:**

1. Sajid et al. (2021), *Active inference: demystified and compared* — relates active inference to RL and control. [arXiv](https://arxiv.org/abs/1909.10863)
2. Da Costa et al. (2020), *Active inference on discrete state-spaces: a synthesis* — the canonical algorithmic reference. [arXiv](https://arxiv.org/abs/2001.07203)
3. Build a discrete agent yourself with [pymdp](https://github.com/infer-actively/pymdp).
4. Tschantz et al. (2020), *Reinforcement learning through active inference* — the bridge to deep RL. [arXiv](https://arxiv.org/abs/2002.12636)

## Textbooks

- Parr, Pezzulo, and Friston (2022). *Active Inference: The Free Energy Principle in Mind, Brain, and Behavior*. The standard, comprehensive textbook; open access. [MIT Press](https://direct.mit.edu/books/oa-monograph/5299/Active-InferenceThe-Free-Energy-Principle-in-Mind)
- Namjoshi (2024). *Fundamentals of Active Inference: Principles, Algorithms, and Applications of the Free Energy Principle for Engineers*. Engineering-focused, conversational, light on proofs. [MIT Press](https://mitpress.mit.edu/9780262050951/fundamentals-of-active-inference/)

## Tutorials and Reviews

- Bogacz (2017). *A tutorial on the free-energy framework for modelling perception and learning*. The recommended first stop, with worked math and MATLAB code. [PMC](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5341759/)
- Buckley, Kim, McGregor, and Seth (2017). *The free energy principle for action and perception: a mathematical review*. A full continuous-time derivation; serious but rewarding after Bogacz. [arXiv](https://arxiv.org/abs/1705.09156)
- Sajid, Ball, Parr, and Friston (2021). *Active inference: demystified and compared*. Compares active inference to reinforcement learning and control for an ML audience. [arXiv](https://arxiv.org/abs/1909.10863)
- Smith, Friston, and Whyte (2022). *A step-by-step tutorial on active inference and its application to empirical data*. Hands-on POMDP modeling and model-fitting with MATLAB. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC8956124/)

## Foundational Papers: The Free Energy Principle

The historical spine, from Friston's early work to the most general formulation.

- Friston (2005). *A theory of cortical responses*. The predictive-coding roots of the framework. [Royal Society](https://royalsocietypublishing.org/doi/10.1098/rstb.2005.1622)
- Friston, Kilner, and Harrison (2006). *A free energy principle for the brain*. Often cited as the earliest statement of the FEP. [PDF](https://www.fil.ion.ucl.ac.uk/~karl/A%20free%20energy%20principle%20for%20the%20brain.pdf)
- Friston (2009). *The free-energy principle: a rough guide to the brain?*. Accessible high-level framing. [PDF](https://www.fil.ion.ucl.ac.uk/~karl/The%20free-energy%20principle%20-%20a%20rough%20guide%20to%20the%20brain.pdf)
- Friston (2010). *The free-energy principle: a unified brain theory?*. The widely cited Nature Reviews Neuroscience synthesis. [Nature](https://www.nature.com/articles/nrn2787)
- Friston, FitzGerald, Rigoli, Schwartenbeck, and Pezzulo (2017). *Active inference: a process theory*. The bridge from the abstract principle to a concrete agent; open access. [MIT Press](https://direct.mit.edu/neco/article/29/1/1/8207/Active-Inference-A-Process-Theory)
- Friston et al. (2019). *A free energy principle for a particular physics*. The most general, and most demanding, statement. [arXiv](https://arxiv.org/abs/1906.10184)

## Predictive Coding

The perception-side precursor and close cousin of active inference.

- Rao and Ballard (1999). *Predictive coding in the visual cortex*. The seminal hierarchical predictive-coding model. [Nature](https://www.nature.com/articles/nn0199_79)
- Spratling (2017). *A review of predictive coding algorithms*. A short, concise survey of the algorithms. [PDF](https://kclpure.kcl.ac.uk/ws/files/99028009/A_review_of_predictive_coding_algorithms_SPRATLING_Accepted13November2015.pdf)
- Millidge, Seth, and Buckley (2021). *Predictive coding: a theoretical and experimental review*. A comprehensive modern review bridging neuroscience and ML. [arXiv](https://arxiv.org/abs/2107.12979)

See also the dedicated [Predictive_Coding_Papers](https://github.com/BerenMillidge/Predictive_Coding_Papers) list.

## Active Inference: Discrete State-Spaces

POMDP-style agents, planning as inference, and expected free energy.

- Da Costa, Parr, Sajid, Veselic, Neacsu, and Friston (2020). *Active inference on discrete state-spaces: a synthesis*. The go-to mathematical reference for discrete agents. [arXiv](https://arxiv.org/abs/2001.07203)
- Smith, Friston, and Whyte (2022). *A step-by-step tutorial on active inference and its application to empirical data*. The hands-on companion for building and fitting discrete models. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC8956124/)

## Active Inference: Continuous Time, Control, and Robotics

Generalized coordinates, dynamic expectation maximization, and physical control.

- Friston, Trujillo-Barreto, and Daunizeau (2008). *DEM: a variational treatment of dynamic systems*. Introduces dynamic expectation maximization, the generalized-coordinates scheme underpinning continuous-time active inference. [PubMed](https://pubmed.ncbi.nlm.nih.gov/18434205/)
- Friston, Daunizeau, Kilner, and Kiebel (2010). *Action and behavior: a free-energy formulation*. The foundational derivation of action as free-energy minimization. [Springer](https://link.springer.com/article/10.1007/s00422-010-0364-z)
- Pezzulo, Rigoli, and Friston (2015). *Active inference, homeostatic regulation and adaptive behavioural control*. Links active inference to homeostatic and associative-learning accounts of behavior. [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0301008215000908)
- Oliver, Lanillos, and Cheng (2019). *Active inference body perception and action for humanoid robots*. First deployment of an active inference perception-action model on a humanoid (iCub). [arXiv](https://arxiv.org/abs/1906.03022)
- Baioumy et al. (2021). *Fault-tolerant control of robot manipulators with sensory faults using unbiased active inference*. Active inference for unbiased state estimation and principled fault detection. [arXiv](https://arxiv.org/abs/2104.01817)
- Lanillos et al. (2021). *Active inference in robotics and artificial agents: survey and challenges*. The definitive survey of active inference for state estimation, control, planning, and learning in robotics. [arXiv](https://arxiv.org/abs/2112.01871)

## Deep Active Inference and AI

Scaling active inference with deep generative models, and its relationship to deep RL.

- Ueltzhöffer (2018). *Deep active inference*. The first deep-learning instantiation. [arXiv](https://arxiv.org/abs/1709.02341)
- Millidge (2020). *Deep active inference as variational policy gradients*. Connects active inference to policy-gradient methods. [arXiv](https://arxiv.org/abs/1907.03876)
- Tschantz, Baltieri, Seth, and Buckley (2020). *Reinforcement learning through active inference*. Bridges active inference and deep RL. [arXiv](https://arxiv.org/abs/2002.12636)
- Fountas, Sajid, Mediano, and Friston (2020). *Deep active inference agents using Monte-Carlo methods*. Scales planning with Monte-Carlo tree search and deep networks. [arXiv](https://arxiv.org/abs/2006.04176)
- van der Himst and Lanillos (2020). *Deep active inference for partially observable MDPs*. Learns policies directly from high-dimensional observations. [arXiv](https://arxiv.org/abs/2009.03622)

## Neuroscience and Computational Psychiatry

Modeling brain function, behavior, and psychiatric conditions.

- Adams, Stephan, Brown, Frith, and Friston (2013). *The computational anatomy of psychosis*. Recasts psychotic symptoms as aberrant precision-weighting in hierarchical Bayesian inference. [Frontiers](https://www.frontiersin.org/journals/psychiatry/articles/10.3389/fpsyt.2013.00047/full)
- Friston, Schwartenbeck, FitzGerald, Moutoussis, Behrens, and Dolan (2014). *The anatomy of choice: dopamine and decision-making*. Derives utility, exploration, and choice from free-energy minimization and links precision updates to dopamine. [Royal Society](https://royalsocietypublishing.org/doi/10.1098/rstb.2013.0481)
- Schwartenbeck, FitzGerald, Mathys, Dolan, and Friston (2015). *The dopaminergic midbrain encodes the expected certainty about desired outcomes*. fMRI evidence that midbrain dopamine tracks the precision of beliefs about policies. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC4585497/)
- Seth and Friston (2016). *Active interoceptive inference and the emotional brain*. Frames emotion and selfhood as predictive regulation of bodily states. [Royal Society](https://royalsocietypublishing.org/doi/10.1098/rstb.2016.0007)
- Parr and Friston (2017). *Working memory, attention, and salience in active inference*. Distinguishes attention (precision over evidence) from salience (epistemic value of actions). [Scientific Reports](https://www.nature.com/articles/s41598-017-15249-0)
- Smith, Friston, and Whyte (2022). *A step-by-step tutorial on active inference and its application to empirical data*. The practical guide to fitting active-inference models to behavioral data. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC8956124/)

## Philosophy and Foundations

Markov blankets, self-organization, the Bayesian brain, and the conceptual debates.

- Clark (2013). *Whatever next? Predictive brains, situated agents, and the future of cognitive science*. The landmark, accessible target article on the brain as a prediction machine. [Cambridge](https://www.cambridge.org/core/journals/behavioral-and-brain-sciences/article/whatever-next-predictive-brains-situated-agents-and-the-future-of-cognitive-science/33542C736E17E3D1D44E8D03BE5F4CD9)
- Friston (2013). *Life as we know it*. Shows that any ergodic system with a Markov blanket will appear to minimize free energy, founding the self-organization account. [Royal Society](https://royalsocietypublishing.org/doi/10.1098/rsif.2013.0475)
- Hohwy (2013). *The Predictive Mind* (book). A book-length philosophical defense of prediction-error minimization. [OUP](https://global.oup.com/academic/product/the-predictive-mind-9780199682737)
- Clark (2016). *Surfing Uncertainty: Prediction, Action, and the Embodied Mind* (book). Extends predictive processing to embodied, action-oriented cognition. [OUP](https://global.oup.com/academic/product/surfing-uncertainty-9780190217013)
- Hohwy (2016). *The self-evidencing brain*. Argues that prediction-error minimization makes the brain self-evidencing. [Wiley](https://onlinelibrary.wiley.com/doi/10.1111/nous.12062)
- Kirchhoff, Parr, Palacios, Friston, and Kiverstein (2018). *The Markov blankets of life: autonomy, active inference and the free energy principle*. Uses nested Markov blankets to define biological autonomy across scales. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC5805980/)
- Ramstead, Badcock, and Friston (2018). *Answering Schrödinger's question: a free-energy formulation*. Integrates the FEP with Tinbergen's four questions into "variational neuroethology." [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S1571064517301409)
- Constant, Ramstead, Veissière, Campbell, and Friston (2018). *A variational approach to niche construction*. Formalizes niche construction (organisms reshaping their own environment) as free-energy minimization, extending the FEP toward evolution and culture. [Royal Society](https://royalsocietypublishing.org/doi/10.1098/rsif.2017.0685)
- Constant, Ramstead, Veissière, and Friston (2019). *Regimes of expectations: an active inference model of social conformity and human decision making*. Models social conformity through "deontic value," showing how shared expectations shape decisions. [Frontiers](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2019.00679/full)
- Constant, Clark, and Friston (2021). *Representation wars: enacting an armistice through active inference*. Uses active inference to broker a truce between representationalist and enactivist accounts of cognition. [Frontiers](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2020.598733/full)
- Constant, Clark, Kirchhoff, and Friston (2022). *Extended active inference: constructing predictive cognition beyond skulls*. Extends active inference beyond the individual, casting cognitive niche construction as optimization of the agent's generative model. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC9292365/)
- Bruineberg, Dołęga, Dewhurst, and Baltieri (2022). *The Emperor's New Markov Blankets*. Critically distinguishes the inferential use of Markov blankets from their contested metaphysical use as agent-world boundaries. [Cambridge](https://www.cambridge.org/core/journals/behavioral-and-brain-sciences/article/abs/emperors-new-markov-blankets/715C589A73DDF861DCF8997271DE0B8C)

## Courses, Lectures, and Videos

- [Active Inference Institute: Courses](https://www.activeinference.institute/courses). Structured courses and recurring textbook reading groups built around the Parr, Pezzulo, and Friston textbook.

## Software and Libraries

- [pymdp](https://github.com/infer-actively/pymdp). Python; discrete active inference for POMDPs and MDPs. The most common starting point for building agents.
- [RxInfer.jl](https://github.com/ReactiveBayes/RxInfer.jl). Julia; reactive message-passing Bayesian inference on factor graphs (the successor to ForneyLab).
- [ForneyLab.jl](https://github.com/biaslab/ForneyLab.jl). Julia; message-passing inference on Forney-style factor graphs.
- [SPM / DEM](https://www.fil.ion.ucl.ac.uk/spm/software/). MATLAB; the Friston lab toolbox with dynamic expectation maximization and active-inference demos.

## Blogs, Explainers, and Visualizations

- Jared Tumiel (2020). *Spinning Up in Active Inference and the Free Energy Principle*. A "syllabus for the curious" that maps out prerequisites and resources to learn the FEP from scratch. [blog](https://jaredtumiel.github.io/blog/2020/10/14/spinning-up-in-ai.html)
- Jared Tumiel (2020). *Friston's Free Energy Principle Explained (Part 1)*. A friendly but rigorous walkthrough of surprisal and free energy. [blog](https://jaredtumiel.github.io/blog/2020/08/08/free-energy1.html)
- Oleg Solopchuk (2018). *Tutorial on Active Inference*. An accessible tutorial building up the discrete POMDP and planning formulation. [Medium](https://medium.com/@solopchuk/tutorial-on-active-inference-30edcf50f5dc)
- Tasshin (2024). *Active Inference and the Free Energy Principle*. A deliberately non-technical, diagram-driven conceptual introduction. [blog](https://tasshin.com/blog/active-inference-and-the-free-energy-principle/)

## Communities, People, and Organizations

**Organizations**

- [Active Inference Institute](https://www.activeinference.institute/) ([activeinference.org](https://activeinference.org/)). A volunteer-led nonprofit running courses, the *Active Inference Journal*, and an open community.
- [VERSES](https://www.verses.ai/). A company applying active inference at scale.

**People** (a non-exhaustive starting point)

Karl Friston, Thomas Parr, Giovanni Pezzulo, Maxwell Ramstead, Axel Constant, Lancelot Da Costa, Noor Sajid, Conor Heins, Alexander Tschantz, Christopher L. Buckley, Ryan Smith, Pablo Lanillos, Beren Millidge.

## Useful Resources and Related Lists

Other curated lists and hubs, acknowledged here as both sources and complements to this list:

- [BerenMillidge/FEP_Active_Inference_Papers](https://github.com/BerenMillidge/FEP_Active_Inference_Papers). The most comprehensive thematic paper list for FEP and active inference (roughly 100+ annotated papers). The research-grade companion to this more beginner-friendly list.
- [BerenMillidge/Predictive_Coding_Papers](https://github.com/BerenMillidge/Predictive_Coding_Papers). A companion list focused on predictive coding.
- [github.com/topics/active-inference](https://github.com/topics/active-inference). All GitHub repositories tagged `active-inference`.
- [Active Inference Institute on GitHub](https://github.com/ActiveInferenceInstitute). Community code, the Active Inference Journal, and related projects.
- [activeinference.github.io](https://activeinference.github.io/). A hub of Free Energy Principle papers and resources.

## Contributing

Contributions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md). In short: place each entry in the right section, keep sections ordered chronologically, add a one-line note explaining why the resource matters, and prefer stable or open-access links.

## License

Released under [CC0 1.0](LICENSE) (public domain dedication).
