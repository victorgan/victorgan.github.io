# Victor Gan's Personal Website

A quick site generated from:

- [Jekyll](http://jekyllrb.com), a static site generator.
- [Poole](http://getpoole.com), an HTML/CSS template.


# License

Open sourced under the [MIT license](LICENSE.md).


# Use
This site requires Jekyll to compile. On a unix-based system, the
[quickstart](http://jekyllrb.com/docs/quickstart/) guide recommends installing
it using rubygems:

```
gem install jekyll
cd this-folder
jekyll serve 
# => Now browse to http://localhost:4000
```

If you'd rather keep your system clean or want to compile on a Windows computer,
the easiest way is to use a virtual machine.

- Download VirtualBox: www.virtualbox.org/wiki/Downloads or `sudo apt-get
  install virtualbox`
- Download Vagrant: www.vagrantup.com/downloads.html or `sudo apt-get install
  vagrant`
- On Windows, I recommend downloading Git for its bash-like command
prompt (enable linux tools): http://git-scm.com/downloads

Then, from a command prompt in the project directory, spin up a VM using the
settings specified in `Vagrantfile`, like so:

```
vagrant up
vagrant ssh
cd /vagrant
jekyll serve --host 0.0.0.0 --watch 4000
```

`--watch 4000` enables auto-regeneration when the site is modified, and 
`--host 0.0.0.0` is a hack to deal with localhost issues. You can also append
`--drafts` to include posts in the drafts folder.
In your own regular web browser, view the site at http://localhost:4000

When finished, exit jekyll with a `ctl+c` and exit the vm with `exit`. When you
want to compile again, do everything after `vagrant up` again. Finally
you can `vagrant destroy` to remove all traces of the virtual machine.

# References

- [Stackoverflow](http://stackoverflow.com/questions/27617217/cannot-reach-jekyll-server-on-vagrant-from-outside) on 0.0.0.0.
- [Github Pages Installation](https://help.github.com/articles/using-jekyll-with-pages/)
- [Vagrant with Github Pages](https://github.com/rjsilk/vagrant-github-pages)
- [Vagrant with Jekyll](https://dwradcliffe.com/2013/04/12/vagrant-to-compile-jekyll.html)
