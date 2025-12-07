# Research

This page is a work in progress. How did you find it? :-)

My current research revolves around my Marie Skłodowska-Curie Actions Postdoctoral Fellowship: _Control Theoretical Testing of CPS (ConTestCPS)_. The project is building a bridge between software and control engineering for the V&V of CPS on two levels: (i) the testing of control-theoretical design assumptions, and (ii) the frequency-domain extension of CPS specification languages.

## Design-Assumptions Testing of Cyber-Physical Systems

I first introduced the concept of design-assumptions testing in [Stress Testing Control Loops in Cyber-Physical Systems](https://github.com/ManCla/mancla.github.io/blob/main/assets/pdfs/journal/2023_tosem_b.pdf), where I classified the types of assumptions underlying control-theoretical models and demonstrated a proof of concept of the testing approach.
More recently, I developed a mature testing strategy [Testing CPS with Design Assumptions-Based Metamorphic Relations and Genetic Programming](https://github.com/ManCla/mancla.github.io/blob/main/assets/pdfs/journal/2025_tse.pdf) targeting the linearity design assumption--i.e., the assumption that the physical part of the CPS can be modelled linearly.
At the heart of this strategy is the formalization of this design assumptions as metamorphic relations.
Such relations are then used in a genetic program to automatically generate test scenarios that violate them in non-trivial ways.

## Design of Controllers Robust to Timing Faults

 * [Deadline-Miss-Adaptive Controller Implementation for Real-Time Control Systems](https://github.com/ManCla/papers/blob/main/assets/pdfs/conference/2022_rtas.pdf)
 * [DMAC: Deadline-Miss-Aware Control](https://github.com/ManCla/papers/blob/main/assets/pdfs/conference/2019_ecrts.pdf)

## Testing of Self-Adaptive Systems

 * [Testing Self-Adaptive Software with Probabilistic Guarantees on Performance Metrics: Extended and Comparative Results](https://github.com/ManCla/papers/blob/main/assets/pdfs/journal/2021_tse.pdf)
 * [Testing Self-Adaptive Software with Probabilistic Guarantees on Performance Metrics](https://github.com/ManCla/papers/blob/main/assets/pdfs/conference/2020_fse.pdf)
