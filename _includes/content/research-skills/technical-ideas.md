# **Working with Technical Ideas**

## Engaging Meaningfully with Technical Ideas

**Literature**

- Identify intellectual and research trends.
- Identify differences and similarities.
- Identify trade-offs between different approaches.
- Identify gaps, open questions, and opportunities.

**Logic and argumentation**

- Develop fluency in the rules of logical deduction (e.g. second-order logic).
- Extract arguments from writing.
- Evaluate empirical or analytic evidentiary support by applying the rules of logical deduction.
- Write clearly and precisely.

**Symbolic formalism**

- Losslessly translate English statements into mathematical formalism, and vice versa.
- Identify ambiguities in translation (when the translated result is not unique).
- Map formalism to high-level intuition (a level higher than saying in English what the symbols literally mean).

**Impact**

- Identify methodological design choices.
- Unfold the potential impact of methodological design choices.
- Identify appropriate metrics for downstream tasks.
- Identify design choices in metrics.
- Unfold the potential impact of metric choices.

## How to Write a Machine Learning Research Paper

**Start with the introduction.** Write **one** sentence for each of the following points. Each comes with a check for whether you got it right.

1. **The problem motivation.** What is the real-life (or other) motivation for your problem? What is the setting for your problem?

   *Check:* Does the reader care about your problem (i.e. feel that your problem is important) after reading your motivation?

2. **The problem statement.** What exactly is the problem you are solving in this paper?

   *Check:* Does your method completely and thoroughly solve the problem?

3. **The existing work and gaps.** What are the existing approaches to solving your problem, and why are they insufficient? Where do they fall short?

   *Check:* Does your method outperform all existing approaches in the areas where they fall short?

4. **The method.** What is your solution to the problem?

   *Check:* Does your reader have a clear sense of how your method is put together (e.g. its major technical pieces, the major components in your pipeline, major innovative changes to existing methods)?

5. **The evidence.** What are the empirical and theoretical evaluations or validations of your method?

   *Check:* Do your experiments and theoretical analyses show that your method outperforms all existing approaches in the areas where they fall short? Do they show that your method works for the right reasons?

**Turn your introduction into a paper.**

1. **Lay out a skeleton.** Start with bullet points for an introduction, laying out a skeleton for your argument. Make sure your logic is sound. Check with other people that your argument is convincing.

2. **Outline the body.** Using the skeleton in your introduction, create an outline for the body of your paper by naming your sections and subsections. Section and subsection names should be informative: tell the reader what the section is about.

3. **Synthesize as results come in.** As your literature survey, theoretical analyses, and experimental results come in:
   - Synthesize information by outlining each subsection: write down the title and the key take-away (last sentence) of each paragraph. Paragraph titles should be informative, telling the reader what the paragraph is about. The key take-away should be informative too: if the reader skipped the entire paragraph and only read the last sentence, they should get a sense of the main insight highlighted in that paragraph.
   - Summarize results by adding tables and figures with informative captions. Each caption should state which methods, datasets, and metrics are visualized by which aspects of the table or figure, and should end with the main take-away of the table or figure.

4. **Flesh it out.** Once you have added most of the main content, start fleshing out your paper with full sentences, without losing the tight logical structure of the bullet-point version:
   - *Put in structure to guide the reader and highlight the logic:* at the beginning of each section or subsection, outline its key points or results and its logic; at the end, summarize its key points or results.
   - *Make your paper skimmable:* make sure each paragraph has a bolded title and a bolded take-away; bold important insights and conclusions; make sure important information gets its own paragraph rather than being buried in a long discussion.

   At this point, don't worry too much about page limits or about being repetitive. Write for clarity, accuracy, and ease of understanding.

5. **Polish.** Once your paper is mostly fleshed out, begin polishing:
   - Observe the elements of good technical writing as you edit (refer to the book on writing we discuss in group meetings).
   - Always favor clarity of logic over literary style: err on the side of short, clear sentences, and spell out conclusions explicitly rather than implying them.
   - Read for ambiguity: is every definition of jargon or a concept, and every description of a method, concrete and detailed enough to rule out multiple interpretations? Test this adversarially: what else could satisfy your definition or description, other than the intended concept or process?
   - Add connectors and transitions that highlight the relationships between ideas and insights:
     - informative transitions and connectors between consecutive paragraphs and blocks of text (e.g. "because of the concern we raised in Section 1.2.1, we now do the following analysis…");
     - useful references to terms, concepts, and insights in other parts of the paper (e.g. "surprisingly, this result contradicts what we predicted in Theorem 3 in Section 3.1…");
     - signposts that anticipate and prepare the reader for what is to come (e.g. "this approximate inference method works well only if our choice of approximate posteriors is expressive; we study the relationship between the choice of approximate posteriors and performance in Section 5…").

6. **Shorten last.** Once your paper has been polished for clarity, you may shorten it to improve concision or to meet page limits. However, you must do this without losing:
   - technical clarity in the definitions and descriptions of concepts and processes;
   - structure that guides the reader and highlights the logic;
   - skimmability.
