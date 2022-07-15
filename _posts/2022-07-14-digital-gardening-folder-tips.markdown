---
layout: post
title: Digital Gardening Folder Tips
---

I started experimenting with  [zettelkasten](https://en.wikipedia.org/wiki/Zettelkasten)-style note taking. This meant I quickly made hundreds of files and needed to organize them somehow. 

I could have a single folder and just search, but I often can't remember an appropriate query and I like browsing through files sometimes for discoverability because I don't know exactly what I'm looking for.  So here's 👏 3 👏  tips 👏  that I've found useful for making folders.

## Put a digit in front of the folder name
I have a couple rules for folders:
- Folder names are prefixed by a single digit, eg. `2 Projects`.
- Digits go from 0 to 9 in order with no repeated numbers (0,1,2,3... not 0,5,2,7... or 0,0,3,3...)
- A folder has either files or folders, never both [^1] 

This leads to some cool nuances.

- There's a maximum of ten folders inside one folder. This is kinda nice for browsing since each folder level is guaranteed to be a manageable size.
- I lazily create the folder hierarchy. When I'm first making the folders, I don't try to make comprehensive sections, just something satisfactory. When it's getting close to ten folders, I try and find patterns and refactor the folders to something that better fits the files - for example, I might make a new folder encompassing three existing folders, and put those three folders inside it because it they are logical taxonomic children. It's kind of a pain to manually re-number them, but it avoids the temptation of over-organizing before necessary.
- Forcing myself to think about hierarchies during reorganization feels like it helps me understand how files relate to each other better. Often, I'll start making new files inspired by a folder reorganization revealing a pattern.
- The folder names are aestheticly pleasing :).

Overall, this is a lot of words to describe a simple way to control ordering: put a digit in front of it.

## Types over Topics
The problem with folders is they work best when they're mutually exclusive to each other - every file has a single appropriate folder to live in.

But designing a mutually exclusive folder hierarchy is *hard work*, and you often don't know if it's worth it for quick off-the-cuff ideas.

One thing I do is have folders describing a file's grammatical type, instead of a specific topic. For example I have something similar to this:

```
- 0 Nouns
- 1 Opinions
- 2 Assertions
- 3 Questions
```

where:
- `0 Nouns` contain notes that well, are a noun, like `Abundant Attitude`. The note describes a named concept.
- `1 Opinions` contain notes that start with an imperative verb, like `Aim Low at First`. The note describes an notable action or mindset.
- `2 Assertions` contain notes that are a falsifiable assertion written as a full sentence, like `A Bluff is a Mathematical Phenomenon`. The note describes an assertion.
- `3 Questions` contain notes of questions I have or once had, like `How Do I Organize My Thoughts`.

Since the title of the note *must* have some grammatical structure, it will be instantly clear what folder it fits into. 

With time, I've added more nuanced folders (eg. a quote folder) that may not technically be mutually exclusive to others (a quote could also be in `2 Assertions`), which leads into...

## Curate Folders for Large Groups of Related Files
I started writing notes for a strategy game. It included one note per hero, skill, item, objective, and so on. Clearly, each of the game's items best fit in the same folder, and there were enough of them that keeping them in the `0 Nouns` folder would be unruly.

If there are a large cluster of files that share a same "type", what I do is split them out into their own subfolders, which may include folders of (*gasp*) specific topics, such as this strategy game. Within the topical folder, "type" folders are still preferred, but it just makes sense to keep them all together to be easily browsed [^2]. Here's what this could look like:

```
- 0 Uncurated
	- 0 Nouns
	- 1 Opinions
	- 2 Assertions
	- 3 Questions
- 1 Curated
	- 0 Fictional Strategy Game
		- 0 Heroes
		- 1 Skills
		- 2 Items
		- 3 Objectives
```


With this uncurated/curated folder split, often I first put random thoughts in the `0 Uncurated` section, and then migrate it to a subfolder in the `1 Curated` section when the thoughts mature and become part of a larger system of notes.

## Fit the Structure to the Data
Anyway, that's all I have, I hope some of these ideas are useful to you. One big underlying idea here is to evolve the folder structure with the notes, that way you're not held back by any dogmatic constraints.

Please note this works for my files, my thinking and my current workflow; as with all digital gardening make sure you adopt what works for you and let go of things that don't.



[^1]: In practice in a folder of folders, sometimes I have a single file of the same name of the parent folder.
[^2]: Tags could be used here, but who wants to tag every single page? And what if a page forgets to include a tag?
