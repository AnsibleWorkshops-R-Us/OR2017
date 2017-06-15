# OR2017
## OR2017 Workshop: Getting Started with Ansible and ServerSpec
June 27, 2017, half day workshop, afternoon
* Facilitated by:
  * *Hardy Pottinger*, UCLA Library ([orcid.org/0000-0001-8549-9354](https://orcid.org/00000001854993540000000185499354))
* Additional collaborators:
  * *Alicia Cozine*, Data Curation Experts
  * *Anthony Vuong*, UCLA Library
  * *Francis Kayiwa*, Princeton University Library

## Abstract

Let's face it, repositories are services, no matter your definition of service.
To offer a service like a repository, you need people: repository management
staff, developers and operations staff (aka sysadmins). Many repositories scrape
by with just a developer or two, maybe a shared sysadmin. A legendary few try to
get by with a single staff member, who wears many hats. This isn't an uncommon
challenge for IT professionals. But it's particularly common among people tasked
with delivering a repository service. We do more with less.

One way to do more with less is with automation. There are tools to help you
manage the task of delivering a service in a more organized fashion. This
workshop will walk you through how to use [Ansible](https://www.ansible.com/),
one such tool, to set up a new service on a new machine. The focus will be on
hands-on learning, walking through the common mistakes one can make when using
Ansible. You'll gain a confidence in the tool, and learn that the error
messages Ansible returns are actually useful in finding those mistakes. You
will quickly discover that using Ansible is pretty similar to what you've
previously done by hand. You may even have shell scripts written to help you
with provisioning; those existing scripts can easily be modified to work with
Ansible. We will also make use of [Serverspec](http://serverspec.org/), a tool
which allows you to characterize the services running on an existing server,
and then use this specification to test and verify the results of your efforts
with Ansible.

## Pre-Requisites

At a minimum, you will need:
* a notebook computer
* an account with admin privileges on this computer, so that you can install
software

Ideally, you will have already installed the following software packages before
you arrive at the workshop space:
* [Ruby](https://www.ruby-lang.org/en/downloads/), version 2.0.x or higher (see note below)
* the ServerSpec gem: `gem install serverspec`
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [Vagrant](https://www.vagrantup.com/downloads.html)

Optionally, if you think you'd like to explore more with Ansible after the
workshop, it would be a good idea to have [Ansible already installed](https://docs.ansible.com/ansible/intro_installation.html).

However, for the workshop, we will be utilizing a VirtualBox VM with Ansible
already configured and ready for you to play. You will take this VM home
with you and will be able to continue using it to learn more. So, don't worry
too much about installing Ansible on your own.

* Note: opinions differ on the "best way" to install Ruby on your computer. This
really only matters if you plan to use Ruby extensively, if you already have Ruby
installed, and it's version 2.0.x or higher, you will be fine for this workshop.
However, you may have heard something about this "discussion" and the details
might be confusing. Our recommendation is to use a Ruby version manager of some
sort, either [RVM](https://rvm.io/) or [rbenv](http://www.rubyinside.com/rbenv-a-simple-new-ruby-version-management-tool-5302.html). We recommend rbenv, as it's a very light-weight/easy way to manage Ruby
installations. RVM can be a bit strange. :-\

## Additional Ansible Resources
* [Alicia Cozine's Ansible for Hydra tutorial](https://github.com/curationexperts/ansible-hydra/wiki/Ansible-for-Hydra) *we make use of this material in our workshop, but you might want to star this repository for later*
* [UCLA Library's Ansible Role Template](https://github.com/UCLALibrary/uclalib_role_template) *we will mention this towards the end of our workshop, but you might want to star this repository for later*
* [Mr. Nice's blog post on Understanding Ansible](https://gist.github.com/MrNice/89a3bbe44e218c9d2309)
*a concise introduction to Ansible*
* [Ansible Tutorial by ServersForHackers.com](https://serversforhackers.com/an-ansible-tutorial) *another concise description of what Ansible is and how to use it, written mostly for devs*
* [Ansible Best Practices](https://www.ansible.com/blog/ansible-best-practices-essentials) *the official best practices guide from Ansible*
* [book: Ansible for Devops by Jeff Geerling](https://github.com/geerlingguy/ansible-for-devops)
* [code: Jeff Geerling's GitHub repositories](https://github.com/geerlingguy)

## Additional ServerSpec Resources
* [video: a ServerSpec tutorial](https://www.youtube.com/watch?v=o_90_W7Btwo)

## Combining ServerSpec and Ansible
Here are two great articles on testing with ServerSpec and combining it with Ansible, however, a warning: save these for after you have gotten your bearings with Ansible and ServerSpec, do not let this more complex information scare you away from trying these tools out. *You do not have to get any of this perfect, you are learning.*
* [Infrastructure Testing with Ansible and Serverspec - Part 1](https://sharknet.us/2014/02/04/infrastructure-testing-with-ansible-and-serverspec-part-1/)
* [Infrastructure Testing with Ansible and Serverspec - Part 2](https://sharknet.us/2014/02/04/infrastructure-testing-with-ansible-and-serverspec-part-2/)

And the example repository from those two articles:
* [Ansible Sample TDD](https://github.com/volanja/ansible-sample-tdd)

## License

[Apache 2.0](https://opensource.org/licenses/Apache-2.0)
