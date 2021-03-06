---
ref: dimitrov2014commutativity
title: Commutativity Race Detection 
authors: Dimitar Dimitrov, Veselin Raychev, Martin Vechev, Eric Koskinen          
year: 2014
venue: ACM PLDI
projects: core
awards:
bibtex: '@article{dimitrov2014commutativity,
  title={Commutativity race detection},
  author={Dimitrov, Dimitar and Raychev, Veselin and Vechev, Martin and Koskinen, Eric},
  journal={ACM SIGPLAN Notices},
  volume={49},
  number={6},
  pages={305--315},
  year={2014},
  publisher={ACM}}'
paper: https://files.sri.inf.ethz.ch/website/papers/pldi14-commutativity.pdf
talk: 
slides: 
---

This paper introduces the concept of a commutativity race. A commutativity race occurs in a given execution when two library method invocations can happen concurrently yet they do not commute. Commutativity races are an elegant concept enabling reasoning about concurrent interaction at the library interface.

We present a dynamic commutativity race detector. Our technique is based on a novel combination of vector clocks and a structural representation automatically obtained from a commutativity specification. Conceptually, our work can be seen as generalizing classical read-write race detection.

We also present a new logical fragment for specifying commutativity conditions. This fragment is expressive, yet guarantees a constant number of comparisons per method invocation rather than linear with unrestricted specifications.

We implemented our analyzer and evaluated it on real-world applications. Experimental results indicate that our analysis is practical: it discovered harmful commutativity races with overhead comparable to state-of-the-art, low-level race detectors.
