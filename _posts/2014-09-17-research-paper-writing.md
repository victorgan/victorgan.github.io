---
layout: post
title: Research Paper Writing
---

## Algorithm

1. Find problem/data
2. Start writing
3. Do research/solve problem
4. Finish 95% draft
    - Make a working title
    - Introduce the topic/define terminology
    - Motivation: emphasize why the topic is important
    - Relate to current knowledge: what's been done
    - Indicate the gap: what needs to be done?
    - Formally pose research questions
    - Explain any necessary background material
    - Introduce formal definitions
    - Introduce your novel algorithm/representation/data structure etc.
    - Describe experimental set-up, explain what the experiments show
    - Describe the datasets
    - Summarize results with figures/tables
    - Discuss results
    - Explain conflicting results, unexpected findings and discrepancies with other research
    - State limitations of the study
    - State importance of findings
    - Announce directions for further research
    - Acknowledgements
    - References
5. Send preview to mock reviewers
6. Send preview to the rival authors (virtually or literally) (Now is about one
   month before the deadline)
7. Revise using checklist
8. Submit

## Checklist
Here's a checklist, mainly based off this 
[KDD Tutorial]({{ site.url }}/assets/posts/2014-09-17-kdd) and 
[This presentation]({{ site.url }}/assets/posts/2014-09-17-cvprpapers)

- Research Problem
    -  Can you write the research statement in one sentence?
    -  Is it falsifiable
    -  Is this a real problem? Does this problem actually exist?
- Data
    -  Real-world data?
    -  Is the data set an appropriate size?
- Related work
    -  Context compared to current solution
    -  Explain differences with our solution / why their solutions don't apply
    -  How this solution fits in to current topics
    -  Indicate what needs to be done
- Solving the Problem
    -  Is this is the simplest solution to get results this good?
    -  Have you eliminated all simpler ideas?
    -  Are all complexities justified
    -  Have you looked to other fields for solutions?
    -  Are you sure the results from papers you've cited are correct?
- Is the solution brittle?
    -  For every parameter (by logic, reason or experiment):
    -  Is there some way to set a good value for the parameter
    -  The exact value of the parameter makes little difference
    -  Are all choices justified
    -  If choice was arbitrary, explicitly state. "we tried multiple, found no
      differences, so omitted results for brevity" Additional criteria in
      additional tech report
- Figures, tables and pictures whenever possible
    -  Do all figures clearly communicate the idea?
    -  Are all figures as polished as possible?
    -  Labels in figures do not conver data
    -  Is psuedocode too long?
- Have some variance estimate on performance measures (do everything 10 times)
- Avoid "Laundry list" citations
    -  Read every single paper referenced
    -  Broad reference bundles [a, b, c, d] needed?
    -  If paper A says something about paper B, don't just copy paper A's opinion
- This paper is in scope of the conference, eg. KDD
    -  Did you read/reference KDD papers?
    -  Is it framed as KDD paper
    -  Is it tested on KKD datasets?
    -  Did you use common KDD evaluation metrics?
    -  Write explicit section that says "at first glance, this might seem like problem X, but…"
- The experiments are reproducable
    -  Webpage for data and paper itself
    -  Using just the webpage, can you recreate all experiments in the paper?
- Is it too similar to your last paper?
    -  Did you reference previous work
    -  Did you explicitly spend at least a paragraph explaining how you are extending your work
    -  Redo intro text/figures
    -  Did you include last work in comparisons?
- Did you acknowledge all weaknesses?
    -  Explain why the work is still useful even with weaknesses, and how it might be fixed
- Did you unfairly diminish work by others?
    -  Send a preview to rival authors: "Dear Sue, we are trying to extend your idea and wanted to make sure we represented your work correctly and fairly, would you mind taking a look…"
- Is there an easier way to solve this problem?
    -  Include strawmen ("while we do not expect X to work well because of Y, we include it for completeness…")
    -  Explicitly write explanation as to why other methods won't work (don't just say [1] says it)
- Referenced related work/idea is already known?
    -  Detailed literature search
    -  Write a longer tech report and say in paper: "see our tech report on full literature"
    -  "In our paper we reintroduced an obscure result and show…"
- Interesting and important problem
    -  Test on real data
    -  Domain expert/collaborator help with motivation
    -  Explicitly state why problem is important
    -  Estimate value "$40,000 in annual savings" "crimes solved" lived saved"
- Is it polished?
- Can I do anything to stop the reviewer from having to think?
- First page: is it clear
    -  What is the problem
    -  Why is it interesting and important
    -  Why is it hard? Why do naïve approaches fail?
    -  Why hasn't it been solved before? What's wrong with previous proposed solutions?
    -  What are the key components of my approach and results? Any limitations?
    -  Summary of contributions: Major points in bulleted form, references to sections
- Is it reproducible
    -  Explicitly: give data, parameter settings
    -  Implicitly: can reproduce in reasonable time, annotated, clear
    -  Is code provided (say in a mock google drive/dropbox account for double-blind studies)
- Check Word meanings:
    -  Optimal
    -  Proved
    -  Significant
    -  Complexity
    -  Correlated
    -  Etc
    -  Mined
    -  Define acronyms before they are used
- Remove unnecessary phrases:
    -  "In this paper" remove
    -  Actual (no meanings in sentence, remove)
    -  Theoretically (no meaning, remove)
- Avoid weak language:
    -  Prefer "it will" vs "might" or "has been shown"
    -  Do not say "attempt", "aiming"
    -  We do not try to do this, we do this
- Avoid overstating
- Directly quote other papers
- Active voice
- Use all the space available (no trailing space in last page)
- Use colour in the text if appropriate
- References: Uses standard conference acronyms to save space?
