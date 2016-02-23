---
layout: post
title: Emacs on Windows
---
Documenting steps to install spacemacs and magit on Windows, in GIF
form! 

Step 1: Download emacs binaries from http://sourceforge.net/projects/emacsbinw64/
![Download]({{ site.url }}/assets/posts/2016-02-23-downloademacs.gif)

Step 2: Install by extracting it into C:\Program Files\emacs, or a similar
folder.
![Install]({{ site.url }}/assets/posts/2016-02-23-installemacs.gif)

Step 3: Create a start menu shortcut of C:\Program Files\emacs\bin\runemacs.exe
in C:\Users\USERNAME\AppData\Roaming\Microsoft\Windows\Start Menu\Programs
by holding alt and dragging it in the explorer window.
![Create Shortcut]({{ site.url }}/assets/posts/2016-02-23-createshortcut.gif)

Okay..this is more of an experiment to test the viability of making
buzzfeed-like Gyazo tutorials. Too much effort. Here's the rest of the steps to
get spacemacs set up.

- Add an environment variable %HOME% to be C:\Users\vigan\
    - search environment in start
    - put value as HOME, without %'s
    - check in command prompt: echo %HOME%
- Install spacemacs by creating a hard link between C:\Users\USERNAME\ .emacs.d and
  a cloned folder of the spacemacs repository.
- Start emacs. Choose VIM-style and standard distribution
