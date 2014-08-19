---
layout: post
title: Useful Sites for Research
---

<!--TODO: history of past sites -->

A list of various sites for research, catered towards computer science. A lot of
them I haven't read yet; it's mostly for my sake.

<!--end excerpt-->
Last updated 2014-08-19 Tue 06:04 PM

## How I Organize Papers and Research

### Saving Papers
If there's a paper I've read or want to read, I add it to my library on Google
Scholar and add an appropriate label. I download a copy of the PDF into Google
Drive with the naming convention "(first author last name) (date) (first word of
title)", eg. gan2014title. This is also the naming convention Google scholar
uses for BibTeX citations, so it acts as a unique ID for the paper both in my
head and whenever I reference it. I find it's a good balance of conciseness and
memorability.  I automate the PDF downloading with Pocket
(tagging each document with its name/date/title unique ID) and IFTTT, though
ideally Scholar would be more elegantly integrated with IFTTT or RSS. 

Microsoft Academic Search has a public API that could be more elegant, but they
don't index enough papers right now.

This works well because:

- I now have a google-powered content-searchable list of all the papers I've read
- I have an offline version of the PDFs
- All the benefits of data in the cloud
- Doesn't require Mendeley or other desktop software
- Easy: I search Google Scholar for papers and BibTeX citations anyway.

But it still has problems:

- The paper lists and tags are locked into Google Scholar. Google Scholar
  doesn't have an "export data" option, and it's not available in Google
  Takeout. This is worrisome, although it seems easily scrapable if I need to
  migrate.
- There might be ID clashes if two first authors publish a paper the same year
  with the same first word in the title. 
- This doesn't elegantly incorporate slides from talks, project files and other
  supplementary material to the papers.
- Pocket + IFTTT is slow.
- What's the best way to take notes on the papers?

### Writing Notes
Right now I use OneNote: I have two notebooks. One for Concepts, where I
summarize ideas and see how they connect, and one for Papers, where I take notes
on individual papers. Ideally the notes in the "Papers" notebook will migrate to
the "Concepts" section. In practice it's very messy; the effort to align things
in OneNote isn't worth the time.

OneNote also allows you to import PDFs to annotate, but the ease of annotation
isn't outweighed by the monolithic file format prone to bit rot.

Good:

- It's in the cloud.
- It supports screenshots, web clippings, handrawn math and figures, and pdf printouts.
- The user interface makes it quick to access everything.
- I can include hand-drawn notes on how papers are related

Bad:

- It's a proprietary, complex file format
- My notes on a paper should ideally be with the paper

## Links

### Initially Useful
- [WikiCFP](http://www.wikicfp.com/cfp/): Has RSS feeds and notifications of
  call for papers.
- [Metacademy](http://www.metacademy.org/): Goes through various machine
  learning concepts
- [The PhD Grind](http://pgbovine.net/PhD-memoir.htm): A memoir from a Stanford
  computer science PhD 

### Persistently Useful
- [Google Scholar](http://scholar.google.com/): Google for research papers. You
  also easily get BibTeX citations from it. When researching a field, find a
  paper and look at both its citations and papers who cite it to give you an
  idea of the context behind it.
    - 'Bookmark' papers and tag them
- [Google Scholar
  Rankings](http://scholar.google.com/citations?view_op=top_venues&hl=en): Ranks
  tiers of conferences
- [Conference Ranks](http://www.conferenceranks.com): Ranks tiers of
  conferences.

### General 'Advice' Pages
- [How to learn on your own](http://www.metacademy.org/roadmaps/rgrosse/learn_on_your_own)
- http://www.cs.cmu.edu/~jasonh/advice.html
- http://vlsicad.ucsd.edu/Research/Advice/network.html

### Topical Links
- [Foundations and Trends® in Machine
  Learning](http://www.nowpublishers.com/journals/MAL/5): "These are sort of
  intermediate between textbooks and research papers, and are a good way to get
  up to speed on important results of the past decade or so which haven't yet
  found their way into textbooks"
- [Recommended Courses for MIRI Math
  Researchers](http://intelligence.org/courses/): A list of free online courses
  for specific background topics.
- [List of machine learning textbooks on
  Reddit](http://www.reddit.com/r/MachineLearning/comments/1jeawf/machine_learning_books/)
- [VLFeat](http://www.vlfeat.org/matlab/matlab.html)
- [Piotr's Matlab Toolbox](http://vision.ucsd.edu/~pdollar/toolbox/doc/index.html)

