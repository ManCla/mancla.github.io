# Research

My current research revolves around my Marie Skłodowska-Curie Actions Postdoctoral Fellowship: _Control Theoretical Testing of CPS (ConTestCPS)_. The project is building a bridge between software and control engineering for the V&V of CPS on two levels: (i) the testing of control-theoretical design assumptions, and (ii) the frequency-domain extension of CPS specification languages.

## Design-Assumptions Testing of Cyber-Physical Systems

The idea behind design-assumptions testing is to integrate the a priori control-theoretical guarantees on a CPS's performance with the a posteriori guarantees provided by software testing.
When developing control algorithms, control engineers can offer formal guarantees about the system's behaviour.
For instance, they may guarantee that a drone takes no more than a specified number of seconds to travel between two points at a given distance.
However, these guarantees depend on the validity of the mathematical models used to represent the CPS's physical dynamics and control algorithms.
Design-assumptions testing aims to generate execution scenarios that intentionally violate these models.
The core hypothesis is that when the models are valid, control-theoretical guarantees suffice, and testing is unnecessary.
Conversely, when the models are invalidated, no a priori guarantees can be provided, and empirical verification through testing becomes essential.
This approach avoids redundant test cases where control engineering already provides performance guarantees and instead focuses testing efforts on scenarios where the system's behaviour cannot be predicted in advance.

I first introduced the concept of design-assumptions testing in [Stress Testing Control Loops in Cyber-Physical Systems](https://github.com/ManCla/mancla.github.io/blob/main/assets/pdfs/journal/2023_tosem_b.pdf), where I classified the types of assumptions underlying control-theoretical models and demonstrated a proof of concept of the testing approach.
More recently, I developed a mature testing strategy [Testing CPS with Design Assumptions-Based Metamorphic Relations and Genetic Programming](https://github.com/ManCla/mancla.github.io/blob/main/assets/pdfs/journal/2025_tse.pdf) targeting the linearity design assumption--i.e., the assumption that the physical part of the CPS can be modelled linearly.
At the heart of this strategy is the formalization of this design assumptions as metamorphic relations.
Such relations are then used in a genetic program to automatically generate test scenarios that violate them in non-trivial ways.

## Design of Controllers Robust to Timing Faults

## Testing of Self-Adaptive Systems
