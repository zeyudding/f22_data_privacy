---
layout: page
permalink: /review/
title: Review
description: 
nav: false
nav_order: 5
---

**These reviewing guidelines are borrowed from a number of top conferences, including ACM CCS, SIGMOD and others.**

---

### Overview

When you prepare your reviews, please consider that they serve two critical purposes:
1. To provide authors with feedback on how to improve their paper and proceed with their work, regardless of the paper decision;
2. To justify and document final decisions regarding publication of this version of the paper.
Regardless of whether a review marks a paper as accept or reject, it should be **thoughtful**, **civil**, and provide **constructive** feedback.

Novelty can manifest in many ways that go beyond the traditional requirement of having a new algorithm or new system design. When reviewing papers, we would like to consider many additional aspects of novelty such as having a novel result, novel engineering, or a novel benchmark. That is, even if the algorithms used and the problem itself are not dramatically new, a paper might still be providing new and useful insights.

Papers that have not gone through peer-review and are not formally published can be brought up if a reviewer feels it is relevant to inform the authors, but such papers cannot be considered in a way that diminishes the novelty of the submitted work or in order to ask the authors to compare explicitly against them, e.g., with experiments. This includes papers on arXiv and white papers.

---

#### Review template

Please follow this structure:

* Summary
    * What is the problem setting? Is the problem setting realistic, or contrived (the authors creating a  problem)?
    * Given the problem, what would be the natural solution? What are existing solutions from the literature? Have the authors considered and compared against these?
    * What is the proposed solution? Is it technically sound (e.g., if there is any proof, is it correct)?

* Strength
    * One to five bullet points summarizing what you like about the paper, e.g., the paper is well written and well structured, the problem is important, the solution is effective, etc.

* Weaknesses
    * One to five bullet points summarizing what you don’t like about the paper, e.g., the paper is not well written or not well structured, the problem is contrived, existing solutions/the solution is effective, etc.

* Detailed comments
    * Detailed questions for authors to respond, and more constructive suggestions.

---

#### Review length

A good review should cover at least the following aspects of the paper in detail: problem focus and motivation, technical contributions, experimental evaluation, related work, and overall presentation. Please elaborate with regards to strong and weak points on all these fronts with detailed comments. We expect an ideal review to span at least 4-5 paragraphs, discussing these aspects. A very short review is very likely a bad review. Recall, that one of the purposes of your review is to give authors constructive feedback, and a short review does not accomplish that.

---

#### Critiquing the paper’s motivation and focus

A good review should evaluate the importance and relevance of the problem that the authors list. The authors may not agree with your conclusion, but it is vital that they understand your rationale. For this reason, criticisms on the motivation of the problem should be clearly explained and justified.

##### Examples to avoid:

* “The motivation of the paper is weak”
    * It is not clear to the authors whether you were dissatisfied with their presentation or with the problem they focus on.
* “This problem is not interesting” “I don’t think anyone will use this”
    * Avoid basing your critique on personal opinions and biases. Perhaps the paper’s focus is not interesting to you, but that does not mean that it is not important. Give specific arguments to explain why you believe it is not practical. It is also not sufficient to simply state that you didn’t find the problem motivation convincing. You should explain why you believe the paper’s focus is unrealistic / too narrow / too broad / no longer relevant.

##### More constructive:

* “The introduction tries to establish the problem motivation by citing prior work, but the paper should stand more on its own. The motivation would improve by discussing real-world examples of this problem and the challenges of current technology.”

* “The introduction of the paper attempts to explain the problem the paper intends to address. However, the introduction makes several self-contradicting statements (such as….) and thus the current presentation makes it sheer impossible to adequately understand the actual problem the paper addresses….”

---

#### Critiquing the technical contributions

A big part of your review is to evaluate the technical contributions of the work. Examine the claims made in the paper, judge if they are applicable to the problem, and evaluate their expected importance, applicability, and usefulness. If you believe that some assumptions of the paper are too restrictive and make the problem unrealistic or narrow, explain that. However, you should avoid tainting your evaluation with personal opinions. Judge the work that the authors are presenting, rather than the work that you would have preferred to see.

##### Examples to avoid:

* “The paper makes strong theoretical contributions in this domain, but it doesn’t test them in a real-world, large-scale deployment”
* “Algorithm A is really interesting and insightful, but what about algorithm B that I just came up with?”
* “The paper solves the problem for setting A, but what about setting B?”

It is great to bring up additional contributions that you would like to see and ideas that could extend the presented work. But write them as suggestions, rather than a basis of criticism. Your review should judge the contributions that the paper makes, rather than the contributions it does not make.

##### More constructive:

* “Algorithm A is non-trivial and has low time complexity. However, it requires maintaining a very large data structure in memory, which might make it impractical for large datasets. Perhaps the algorithm can be improved or shown to be applicable to large datasets?”

---

#### Critiquing the evaluation

Your review should evaluate whether the experiments validate the claims of the paper. If the paper claims that the proposed algorithm improves on the state-of-the-art, discuss whether the experiments compare the proposed approach with the appropriate methods, and against all expected metrics (e.g., efficiency, accuracy, scalability). Your review should note whether there are any inconsistencies in the results and whether there are observations that are not explained, justified, or discussed. Also judge whether the experimental methods and datasets are appropriate, or if they introduce biases in the results.

##### Examples to avoid:

* “The experiments compare the proposed approach with methods A, B, and C, but method D could also be applicable if one made these parameters flexible”
    * This is more often than not an unfair criticism. If a method needs non-trivial adjustments to apply in this work, and the paper already compares with suitable techniques, this should not be a basis of criticism.
* “Larger-scale experiments are needed”
    * This comment by itself is not sufficient criticism. Communicate to the author what scale of experiments you would consider satisfactory and why.

##### More constructive:

* “The experiments do not include comparisons with other methods, because this is the first work that addresses problem X. However, I believe that Algorithm ABC for problem Y could be applicable here with the following minor modifications:…”

In addition, as you consider such remarks, please consider space restrictions. For example, are there any of the existing experiments that you think are less useful and can be dropped?

---

#### Critiquing the writing and presentation

You may often find the presentation of a paper unsatisfactory. Please list specific points of possible improvement such as repetitiveness, poor structure, confusing notation, missing examples, or lack of formalism. However, make sure that you provide concrete examples and pointers for your criticisms. For example, explain what notation confused you, which terms were not properly defined, and which statements should be made more rigorous. Communicating vague discontent about the readability of the paper is not constructive, because it doesn’t explain to the authors how they can improve it.

##### Examples to avoid:

* “The paper is unreadable”
    * Only OK if the paper is actually written in a foreign language. Otherwise, give some examples of the readability issues that you experienced.
* “The notation is confusing”
    * Be more explicit about what you found problematic, and what you think might help.

##### More constructive:

* “I found section 4.1 hard to follow. I believe that it would help if the authors moved the discussion at the end of section 4.3 to the beginning of section 4.1, as it gives the intuition behind the definitions”

* “There is a clash of notation: sometimes $\alpha$ is used to represent a query answer, but it is also the approximation factor in Algorithm 1.”

---

#### Critiquing the related work

You should ensure that the paper includes sufficient discussion of the related work, explains similarities and differences, and does not omit obvious connections. Keep in mind however that, unless you are reviewing a survey paper, there will always be some citations that could have been added but weren’t. Do not criticize a paper for the omission of a particular citation if it already includes sufficient discussion of the related work in the particular area. Do point out though glaring omissions and important connections that were missed.

##### Examples to avoid:

* “This work seems very similar to [X]”
    * This claim is vague and unsubstantiated. Provide clear discussion on whether particular claims have been demonstrated before in prior work.

* “There is a large body of related work on problem X that the paper does not discuss”
    * You should make such a criticism more concrete by including particular references that you expected to see discussed. Suggest to the authors a few specific citations that they should include and explain why.

##### More constructive:

* “The authors mention connections to [X] in the related work, but they do not explain why [X] is not directly applicable and why a new approach is needed.”

---

#### Inclusive language

In keeping with efforts on Diversity and Inclusion in our conference and community, please check the paper for language that may further the marginalization, stereotyping, or erasure of any group of people, especially historically marginalized and/or under-represented groups (URGs) in computing. Authors have been given detailed guidelines and examples on this front. Please read this page if you have not already done so.

If you find exclusionary or hurtful language or examples (even if unintentional), point them out in your review and ensure the authors change the text accordingly. Please also be mindful of using inclusive language in your own review text, as well as during the discussion phase.