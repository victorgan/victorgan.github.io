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
Download Vagrant: www.vagrantup.com/downloads.html
Download VirtualBox: www.virtualbox.org/wiki/Downloads
On Windows, I recommend downloading Git for Windows for its bash-like command
prompt (enable linux tools): http://git-scm.com/downloads

Then, from a command prompt in the project directory, spin up a VM using the
settings specified in `Vagrantfile`:

```
vagrant up
vagrant ssh
cd /vagrant
jekyll serve --host 0.0.0.0
```
In your own regular web browser, view the site at http://localhost:4000

When finished, exit jekyll with a `ctl+c` and exit the vm with `exit`. When you
want to compile again, do everything after `vagrant up` again. Finally
you can `vagrant destroy` to remove all traces of the virtual machine.

# References
[Stackoverflow](http://stackoverflow.com/questions/27617217/cannot-reach-jekyll-server-on-vagrant-from-outside) on 0.0.0.0.
[Github Pages Installation](https://help.github.com/articles/using-jekyll-with-pages/)
