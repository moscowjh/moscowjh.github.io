---
layout: post
title:  "Development Machines"
---

Setting up one's development environment on a personal laptop requires a surprising amount of intellectual effort and focus.  This requires among other things setting up a virtual machine (or machines) in order to run different operating systems, libraries or applications - and to separate development technologies from the operations of your local machine.

Sometimes, after configuring a tool and getting it to function, it stops working suddenly "on its own."  There is always some kind of an underlying change that causes this ghost - often a component of the larger system has been updated universally as part of a general 'upgrade.'

The Vagrant virtual machine that is used by the Udacity online education system suddenly stopped working and this has become and unplanned 'time sink' for me.  I  updated the virtualization software which appeared to be working, but the system is not finding the Linux vm. So next step now was to figure out how to reinstall from the Udacity documentation.

The problem, it turned out, was that when I had moved development work from one machine to another, I had changed my folder structure.  I did not copy all of the configuration files from one folder on the old machine: this had prevented some of the key technologies from downloading from the internet onto my machine.  Figuring out that I had made this error, caused me no fewer than four hours work.
