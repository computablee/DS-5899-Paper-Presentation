# Emergent Abilities of Large Language Models
Large language models (LLMs) often feature *emergent abilities*.
An emergent ability is a phenomenon where LLMs will perform effectively randomly on a task up until the number of model parameters exceeds some critical threshold, at which point performance skyrockets to significantly better than random.
The transition from *random performance* to *better-than-random* performance is called a phase transition.

One of the emergent behaviors discussed in our course this semester is in-context learning, which begins to emerge around 6-7 billion parameters.
Under this threshold, models display no capabilities to perform in-context learning. However, once this threshold is passed, the behavior emerges.
It is impossible to predict emergent abilities without empirical observation via training increasingly large models, because emergent abilities do not follow traditional scaling laws.

## Few-Shot Prompted Tasks

Few-shot prompting is where an LLM is given a small handful of examples of a task, after which point it must perform on new data and perform said task.
This paper uses BIG-Bench, a benchmark suite of over 200 benchmarks for evaluating LLMs. This paper uses four benchmarks from BIG-Bench:

* **Mod. arithmetic** - 2-digit and 3-digit addition and subtraction, 2-digit multiplication
* **IPA transliterate** - transliteration of the international phonetic alphabet
* **Word unscramble** - unscrambling words
* **Persian QA** - question answering in Persian

The following figure displays accuracy on all of these tasks vs. random for several differnt parameter counts.

![Figure 1](assets/figure1.png)

GPT-3 begins to exceed random performance around 13B parameters, and LaMDA exceeds random performance around 68B parameters.

**Q1:**
