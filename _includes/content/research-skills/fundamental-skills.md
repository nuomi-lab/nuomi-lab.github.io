# **Four Fundamental Skills of Research**

Research rests on four fundamental skills:

1. **Finding, defining, and scoping a research question**
2. **Surveying related work**
3. **Sustaining incremental progress on your research question**
4. **Communicating results**

## 1. Defining and Scoping a Research Problem

Turn a vague or general real-life question into actionable technical questions that are valuable to answer. This involves learning:

- what makes a question **useful** to answer, i.e. of interest to some community;
- how to **narrow down** a vague or general question into concrete, actionable questions;
- how to **translate** goals in the application or task setting into machine learning formalism.

Questions to ask yourself:

- What application domains or research subfields does your research question impact? How does your research question advance these domains or subfields?
- What aspects of your research question can be formulated as a machine learning problem, and what framework of formulation should you choose?
- What aspect of your research question is solvable given your background and timeline?

> **What we expect:** It will take many years of experience for you to be able to do the above independently. In the meantime, observe with care how your mentors define and scope research problems, and learn from their examples.

## 2. Surveying Related Work

Understand how your proposed approach to a problem relates to existing work. This involves learning to:

- **collect** representative works that use *different methods to tackle the same problem*, works that use *similar methods for different problems*, and works that demonstrate the significance of the problem;
- **synthesize** related works into conceptual categories, exposing different frameworks or schools of thinking;
- **situate** your approach to the problem within the literature: what do you intend to contribute, and why is this contribution novel and significant?

How do you build up a representative collection of related works?

- Read other people's literature surveys, and explore the works referenced there.
- Start with a set of "seed works", and explore their references as well as the works that cite them.
- Explore works in adjacent fields that solve similar problems or use similar methods.

How do you summarize related works?

- Group related works by conceptual framework, modeling assumptions, inference techniques, types of data, space-time complexity, limitations, etc.
- Identify how your work is different from each group of related works, and why that difference means your approach is better.

> **What we expect:** You will maintain a succinct summary of related works, and be able to clearly articulate your contribution in relation to these works, as well as build on existing knowledge.

## 3. Sustaining Progress

Maintain piecewise-small, concrete, consistent progress towards your research goal. This involves learning to:

- **design** experiments to test specific hypotheses;
- **analyze and synthesize** experimental results to inform new hypotheses;
- **align** short-term hypotheses with long-term goals.

In practice:

- Keep detailed research notes, and keep these notes updated and organized.
- For blind experiments, keep track of the parameters that vary versus those that are fixed.
- For targeted experiments:
  - State the hypothesis the experiment tests (there should be only one per experiment).
  - State how you will summarize the results (e.g. a table or a graph).
  - State how the result would give support for or against the hypothesis: describe how the graph of a positive result would look versus a negative result.
  - Consider alternative explanations for your results (e.g. are there confounding variables?).
- Generate new hypotheses. Every experiment, regardless of the result, yields insight.
- Periodically summarize your results, and ask what remains to be shown with respect to your research goal.

> **What we expect:** Every team keeps a single, well-organized document, updated weekly, containing its research notes as well as feedback from meetings.

## 4. Communicating Results

A sequence of results is not a paper! Communicating research is the act of creating a single, scientifically honest narrative to fit your results. This involves learning to:

- **create a single coherent narrative** from your experimental results;
- **curate experimental results** that support the claims in your narrative;
- **evaluate** to what degree you've solved the problem, and identify limitations and future steps.

Questions to ask yourself:

- What does the body of your experiments say about your research question as a whole?
- Are your experiments sufficient to support your claims?
- Do the results from different experiments support the same conclusion or different conclusions?
- What are the limitations of your experiments (what can you *not* conclude from the results)?
- What are some interesting directions for future research suggested by your experiments?

> **What we expect:** Every team produces a conference-style paper summarizing its work. The process of writing is what turns facts into knowledge. See [How to Write a Machine Learning Research Paper](#technical-ideas) below.
