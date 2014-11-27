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
[KDD Tutorial]({{ site.url }}/assets/posts/2014-09-17-kdd.pdf) and 
[This presentation]({{ site.url }}/assets/posts/2014-09-17-cvprpapers.pdf) [todo include this]

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
- Supplementary material:
    - Add clarification tables that would otherwise be too trivial

## Writing Correctness and Style Pet Peeves
Tamara Munzner

Correctness

- whether to hyphenate a noun phrase depends on how it is used. Use
  "foo bar" when a noun phrase is used as a noun, and "foo-bar" when
  the phrase is used as an adjective. Correct: "we lay out elements
  end to end in a line" (noun), "we make an end-to-end argument as in
  networking" (adjective).

- "lay out" is a verb. "layout" is a noun. Correct: "we lay out the
  graph splendidly" (verb use), "the layout is splendid because" (noun
  use).

- citations are grammatically invisible, you shouldn't use them for
  nouns.

- "it's" is a contraction for "it is", not a possessive

- avoid contractions in formal technical writing

- every figure must be referenced in the main body text

- please get principal/principle right. principal = main, principle =
  idea. PCA stands for Principal Components Analysis. PI stands for
  Principal Investigator.



References

- in a bibliography, always always hand-check bibtex that you get off
  the web. it's usually inconsistent or incomplete. 

  be consistent with journal/conference names. no need for publisher
  address unless it's someplace obscure, and no need for publisher if
  it's implicit in the conf/journal name (i.e. ieee/acm). always
  doublecheck that the pages are in there (both the start and end
  page!).

  also be concise and consistent: 'Trans.' not 'Transactions', 'Symp.'
  not 'Symposium', 'Conf.' not 'Conference'. don't include words like
  "of the" or "on". Don't ever say 'pages', just 'p.'

  do include the accepted nickname/shortname for conferences in
  parentheses after the long name. don't include the year after that
  nickname, it's already communicated by the year that comes at the
  end of the citation. 

  example of bad bibliography snarfed off the web:

  "M. Wattenberg. A note on space-filling visualizations and space-filling 
  curves. In Proc. of the IEEE Symposium on Information Visualization 
  (INFOVIS'05), volume 0, page 24, Los Alamitos, CA, USA, 2005. IEEE 
  Computer Society."

  after fixing: 

  "M. Wattenberg. A note on space-filling visualizations and
  space-filling curves. In Proc. IEEE Symp. Information Visualization
  (InfoVis), p 181-186, 2005"

  if you're pressed for space, change long author lists to
  'FirstAuthor et al'. I normally do full names for four or less, and
  switch to et al for five or more. The way to do this in latex is
  "John Smith and others" for author list. 

  make sure that you've got the right capitalization in titles using
  curly braces to escape stuff. Main offenders are "D" (3D, ND),
  acronyms, and camelcase names. 

  in short: check your bibliography *very carefully*. do not be sloppy
  and inconsistent. be assured that i will notice.


Style

The issues below are stylistic choices - I'm not saying the other way
is technically incorrect, I'm saying I have such a strong preference
for this way that I will change it whenever I edit.

- avoid parentheses whenever possible, they interrupt flow. It's OK to
  use them when defining acronyms, but otherwise I try to hold myself
  to only one parenthetical remark per paper. 

- avoid e.g. and i.e., spell out "such as" or "for example" instead.
  Again, it's a flow issue. 

- minimize use of possessives with nouns. So instead of "feature's
  sequences", say "sequences of a feature". it's easier to parse.

- avoid "this" without a noun after it, especially at the beginning of
  a sentence. Instead of "This shows that we are fabulous", say "This
  situation shows that we are fabulous", to make the referent
  unambiguous. 

  in more detail from Ullman, on "Avoid non-referential this"

  While it sounds pedantic at first, you get a huge increase in clarity
  by chasing the "nonreferential this" from students' writing. Many
  students (and others) use "this" to refer to a whole concept rather
  than a noun. For example: "If you turn the sproggle left, it will
  jam, and the glorp will not be able to move. This is why we foo the
  bar." Now the writer of this prose fully understands about sproggles
  and glorps, so they know whether we foo the bar because glorps do
  not move, or because the sproggle jammed. It is important for
  students to put themselves in the place of their readers, who may be
  a little shaky on how sproggles and glorps work, and need a more
  carefully written paragraph. 

  Source: Jeffrey D. Ullman, Advising students
  for success, CACM 52(3):34-37, March 2009

- always use the Oxford/serial comma with lists. instead of "we have
  apples, oranges and bananas for sale", say "we have apples, oranges,
  and bananas for sale". The final comma is critical for resolving
  ambiguity in some situations. Like this one:
  http://www.outsidethebeltway.com/merle-haggard-and-the-gay-serial-comma/

- avoid the passive voice, use active voice. passive voice makes your
  text too ambiguous about who is the agent of action.

- must have some prose between section and subsection header

- avoid "in this section we do XXX". just *do* XXX!

- emphasize a word when you first *define* it, not when you first
  *use* it. ideally the definition and the first use are the same. but
  it might be a sentence or two later. 

- firstly vs. first is admittedly an issue of personal preference. i
  strongly prefer the latter. let me bring your attention to a quote
  from Elements of Style: "Do not dress words up by adding 'ly' to
  them, as though putting a hat on a horse."

- avoid double negatives, use a positive instead because it's easier to parse

- use parallel structure when possible, both at the level of sentences
  in a paragraph and at the level of section naming. Correct: Naming
  Foo, Linking Bar, Adding Bat. Incorrect: Name Foo, Linking Bar, Bat
  Additions.

- avoid switching between tenses unless you have a very good reason to
  do so. usually what you're reporting on in the paper should stay in
  the present tense (Correct: "the system is designed to do foo".
  Incorrect: "the system was designed to do foo".) past tense should
  be reserved for things truly in the past, like what users did during
  a user study.

- for captions, use boldface type then colon to distinguish subfigure
  labels {"Top Right:"}. Always have a (possibly short) bit saying
  what the full figure does before starting with subfigure
  descriptions. Each subfigure should have its own label, rather than
  having a continuing sentence where you mention subfigure bits as you
  go. Correct: "Key aspects of foobar. {\bf Top Left:} The first
  thing. {\bf Top Right:} The second thing." Incorrect: "The first
  thing (top left), and the second thing (top right)".

- plus everything that John Owens says here: http://www.ece.ucdavis.edu/~jowens/commonerrors.html

- plus everything in the splendid grammar book _Bugs in Writing_ by
  Lyn Dupre
