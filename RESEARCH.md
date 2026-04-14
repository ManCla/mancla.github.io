# Research Overview

My current research revolves around my Marie Skłodowska-Curie Actions Postdoctoral Fellowship: _Control Theoretical Testing of Cyber-Physical Systems (ConTestCPS)_. The project is building a bridge between software and control engineering for the V&V of CPS on two levels: (i) the testing of control-theoretical design assumptions, and (ii) the frequency-domain extension of CPS specification languages.

## Testing of Cyber-Physical Systems

My main contribution in the area of Testing of CPS is the concept of _design-assumptions testing_. This approach aims at integrating control-theoretical guarantees and models into the CPS testing process. When developing control algorithms, control engineers can offer formal guarantees about the system's behaviour. However, these guarantees depend on the validity of the mathematical models used to represent the CPS's physical dynamics and control algorithms. Design-assumptions testing aims to generate execution scenarios that intentionally violate these models. The core hypothesis is that, when the models are valid, control-theoretical guarantees suffice, and testing is unnecessary. Conversely, when the models are invalidated, no a priori guarantees can be provided, and empirical verification through testing becomes essential. This approach avoids redundant test cases where control engineering already provides performance guarantees and instead focuses testing efforts on scenarios where the system's behaviour cannot be predicted in advance.

 * If you want a thorough discussion of what are the control-theoretical design assumptions and a testing proof of concept, have a look at [Stress Testing Control Loops in Cyber-Physical Systems](https://github.com/ManCla/mancla.github.io/blob/main/assets/pdfs/journal/2023_tosem_b.pdf).
 * If you are interested in a fully-developed testing approach, that merges design-assumptions, metamorphic testing, and genetic programming, have a look at [Testing CPS with Design Assumptions-Based Metamorphic Relations and Genetic Programming](https://github.com/ManCla/mancla.github.io/blob/main/assets/pdfs/journal/2025_tse.pdf).

During my PhD at Lund University, in Sweden, I collaborated with [Bitcraze](https://www.bitcraze.io) to investigate the impact of using different testing setups (model-, software-, hardware-, real-world-, in-the-loop) on the testing of CPS.

 * [Testing Abstractions for Cyber-Physical Control Systems](https://github.com/ManCla/mancla.github.io/blob/main/assets/pdfs/journal/2023_tosem_a.pdf).

## Frequency-Domain Enhancement of CPS V&V

In my [Stress Testing Control Loops in Cyber-Physical Systems](https://github.com/ManCla/mancla.github.io/blob/main/assets/pdfs/journal/2023_tosem_b.pdf) paper, I was the first to exploit the use of the frequency-domain representation of signals to enhance test-case generation for CPS. Now I am continuing my work on this direction as part of my ConTestCPS project.

## Design of Controllers Robust to Timing Faults

Control algorithms are traditionally designed under the assumption that they execute at a fixed, constant rate (_yes, this is closely related to the design-assumptions mentioned above!_).
However, to ensure timing guarantees, this assumption can lead to overly conservative design of the underlying real-time system, while still leaving systems vulnerable to timing faults that degrade performance.

 * If you are curious about how to design controllers that work a a low sampling rate and intentionally miss some deadlines, while still improving performance, have a look at [Deadline-Miss-Adaptive Controller Implementation for Real-Time Control Systems](https://github.com/ManCla/papers/blob/main/assets/pdfs/conference/2022_rtas.pdf).
 * If you are interested in an push-button approach to make your control algorithm a lot more robust to timing faults, have a look at [DMAC: Deadline-Miss-Aware Control](https://github.com/ManCla/papers/blob/main/assets/pdfs/conference/2019_ecrts.pdf).

## Testing of Self-Adaptive Systems

Self-adaptive software systems (SAS) are software systems capable of monitoring their own behaviour and autonomously taking actions to maintain stable performance under changing conditions. Testing such systems is difficult because of the intrinsic uncertainty that characterises their execution. I have explored how to test such systems by leveraging scenario theory, a mathematical framework for solving optimization problems under uncertainty and obtain probabilistic guarantees on SAS performance.

 * [Testing Self-Adaptive Software with Probabilistic Guarantees on Performance Metrics: Extended and Comparative Results](https://github.com/ManCla/papers/blob/main/assets/pdfs/journal/2021_tse.pdf)
 * [Testing Self-Adaptive Software with Probabilistic Guarantees on Performance Metrics](https://github.com/ManCla/papers/blob/main/assets/pdfs/conference/2020_fse.pdf)
