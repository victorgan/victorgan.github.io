---
layout: post
title: Useful Sites for Research
---

A list of various sites for research, catered towards computer science. A lot of
them I haven't read yet; it's mostly for my sake.

<!--end excerpt-->
Last updated Sept 15, 2014.

## How I Organize Papers and Research

### Saving Papers
If there's a paper I've read or want to read, I: 

1. add it to my library on Google Scholar and add labels. 
2. download a copy of the PDF into Google Drive with the naming convention
   "(first author last name) (date) (first word of title)", eg.  gan2014title.
   This is also the naming convention Google scholar uses for BibTeX citations,
   so it acts as a unique ID for the paper both in my head and whenever I
   reference it. I find it's a good balance of conciseness and memorability.  
3. I automate the PDF downloading with Pocket (tagging each document with its
   name/date/title unique ID) and IFTTT. Ideally Scholar would be more elegantly
   integrated with IFTTT or RSS. Microsoft Academic Search has a public API that
   could be more elegant, but they don't index enough papers right now.

This works well because:

- I now have a google-powered content-searchable list of all the papers I've read
- I have an offline version of the PDFs
- All the benefits of data in the cloud
- Doesn't require Mendeley or other desktop software
- Easy: I search Google Scholar for papers and BibTeX citations anyway.

But it still has problems:

- The paper lists and tags are locked into Google Scholar. Google Scholar
  doesn't have an "export data" option, and it's not available in Google
  Takeout. This is worrisome, although it looks easy to scape if I need to
  migrate.
- There might be ID clashes if two first authors publish a paper the same year
  with the same first word in the title. 
- This doesn't elegantly incorporate slides from talks, project files and other
  supplementary material to the papers.
- Pocket + IFTTT is slow to update.
- What's the best way to take notes on the papers?
- Batch labelling papers could be easier

### Writing Notes
Right now I use OneNote: I have two notebooks. One for Concepts, where I
summarize ideas and see how they connect, and one for Papers, where I take notes
on individual papers. Ideally the notes in the "Papers" notebook will migrate to
the "Concepts" section. In practice it's very messy; the effort to visually
align things in OneNote isn't worth the time. It's great for quick and messy
thoughts: whenever I see something that relates to a concept, I take a
screenshot and add it to the page. It's easy to re-organize notes, so I don't
care if my notes on are in the wrong category.

OneNote also allows you to import PDFs to annotate, but the ease of annotation
isn't outweighed by the potential for bit rot. I haven't tried Evernote.

Good:

- It's in the cloud.
- It supports screenshots, web clippings, hand-drawn math and figures, and pdf printouts.
- The user interface makes it quick to access everything.
- I can include hand-drawn notes 
- The search is good
- It makes me summarize notes instead of highlighting it, which helps with
  understanding (or so I think)

Bad:

- It's a proprietary, complex file format
- The notes can only be in one category, instead of a tag-based system where it could be in multiple
- My notes on a paper should ideally be with the paper
- Slow to load and crashes from time to time
- It's not plain text

## Links

### Initially Useful
- [WikiCFP](http://www.wikicfp.com/cfp/): Has RSS feeds and notifications of
  call for papers.
- [Metacademy](http://www.metacademy.org/): Goes through various machine
  learning concepts


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
- [Microsoft Academic Search](http://academic.research.microsoft.com/): Ranks people, conferences, universities, and publication by field of research
- [Rankings for common computer vision datasets](http://rodrigob.github.io/are_we_there_yet/build/)
- [http://en.wikipedia.org/wiki/List_of_algorithms#Sequence_algorithms](http://en.wikipedia.org/wiki/List_of_algorithms#Sequence_algorithms)
- [Most cited papers from CVPR](http://scholar.google.ca/citations?hl=en&vq=eng_computervisionpatternrecognition&view_op=list_hcore&venue=l60tToE7K3UJ.2014)
- [Most cited papers from ICCV](http://scholar.google.ca/citations?hl=en&vq=eng_computervisionpatternrecognition&view_op=list_hcore&venue=PotJioSyHM8J.2014)
- [Most cited papers from ECCV](http://scholar.google.ca/citations?hl=en&vq=eng_computervisionpatternrecognition&view_op=list_hcore&venue=sRZyLQvTcTQJ.2014)
- [Most cited papers from PAMI](http://scholar.google.ca/citations?hl=en&vq=eng_computervisionpatternrecognition&view_op=list_hcore&venue=FMIcylNwodUJ.2014)

### General 'Advice' Pages
- [How to learn on your own](http://www.metacademy.org/roadmaps/rgrosse/learn_on_your_own)
- [http://www.cs.cmu.edu/~jasonh/advice.html](http://www.cs.cmu.edu/~jasonh/advice.html)
- [http://vlsicad.ucsd.edu/Research/Advice/network.html](http://vlsicad.ucsd.edu/Research/Advice/network.html)
- [http://www.cs.ubc.ca/~van/upload/TenSimpleRulesCollection.pdf](http://www.cs.ubc.ca/~van/upload/TenSimpleRulesCollection.pdf)
- [The PhD Grind](http://pgbovine.net/PhD-memoir.htm): A memoir from a Stanford
  computer science PhD 
- [http://www.cs.ubc.ca/~murphyk/Teaching/guideForStudents.html](http://www.cs.ubc.ca/~murphyk/Teaching/guideForStudents.html)
- [http://www.cs.ucr.edu/~eamonn/Keogh_SIGKDD09_tutorial.pdf](http://www.cs.ucr.edu/~eamonn/Keogh_SIGKDD09_tutorial.pdf)
- [http://users.soe.ucsc.edu/~ejw/advice/](http://users.soe.ucsc.edu/~ejw/advice/)

### Writing Tips
- [https://www.cs.ubc.ca/~tmm/writing.txt](https://www.cs.ubc.ca/~tmm/writing.txt)

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

### Datasets
- [https://www.quandl.com/](https://www.quandl.com/)
- [Google Dataset Search](https://www.google.com/cse/publicurl?cx=002720237717066476899:v2wv26idk7m)
- [http://rs.io/100-interesting-data-sets-for-statistics/](http://rs.io/100-interesting-data-sets-for-statistics/)
- [Computer vision datasets](http://homepages.inf.ed.ac.uk/rbf/CVonline/Imagedbase.htm)

### Matlab
It's useful to have Matlab with the following toolboxes:

- Image Processing Toolbox
- Parallel Processing Toolbox
- Statistics Toolbox
- Computer Vision Toolbox (if only for the plotting functions)

- [VLFeat](http://www.vlfeat.org/matlab/matlab.html)
- [Piotr's Matlab Toolbox](http://vision.ucsd.edu/~pdollar/toolbox/doc/index.html)
- [Other useful Matlab Resources](http://www.csse.uwa.edu.au/~pk/research/matlabfns/othersites.html)
- [http://graphics.cs.msu.ru/ru/science/research/machinelearning/adaboosttoolbox](http://graphics.cs.msu.ru/ru/science/research/machinelearning/adaboosttoolbox)
- [http://asi.insa-rouen.fr/enseignants/~arakotom/toolbox/index.html](http://asi.insa-rouen.fr/enseignants/~arakotom/toolbox/index.html)
- [http://svmlight.joachims.org/](http://svmlight.joachims.org/)
- [http://gaussianprocess.org/gpml/](http://gaussianprocess.org/gpml/)
- [https://sites.google.com/site/alainrakotomamonjy/](https://sites.google.com/site/alainrakotomamonjy/)

### Additions
If there's anything you think would fit here, feel free to comment below (check 'I'd rather post as guest' and put a bogus
email if you'd rather keep anonymous) 
