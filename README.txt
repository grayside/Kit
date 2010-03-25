$Id$

# KIT

Kit is a compilation of tools and best practices for site builders.

Kit is not actually a library of tools like for instance Chaos Tools [1], it is
a collection of modules and themes together with a set of guidelines that
facilitate site building. The goal is to offer a straightforward base package
for building state-of-the-art Drupal sites while specifying how Features built
on top of Kit can be compatible.

*Dedicated to Beth MacWright.*

## Specification

- KIT Feature Specification (kitf 1.0-draft) [2]
- KIT Theme Specification (kitt 1.0-draft) [3]

## Modules

Modules are captured in the included drupal-org.make file. This collection
represents a

## Themes

Kit is currently tracked as a module project on drupal.org as install profiles
do not support inheritance (your site cannot run more than one install profile).
This allows adding Kit to additional site builds without limiting the use of
install profiles.

Being technically a module on drupal.org, Kit cannot contain themes. Here is a
list of themes in drush make format commonly used with Kit (currently only one
theme):

; Kit-compliant base theme with hard resets and simplified templating.
projects[tao][download][type] = "get"
projects[tao][download][url] = "http://code.developmentseed.org/sites/code.developmentseed.org/files/fserver/tao-6.x-1.8.tgz"
projects[tao][directory_name] = "tao"
projects[tao][type] = "theme"

[1] http://drupal.org/project/ctools
[2] http://drupalcode.org/viewvc/drupal/contributions/modules/kit/kitf.txt?view=co
[3] http://drupalcode.org/viewvc/drupal/contributions/modules/kit/kitt.txt?view=co
