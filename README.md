[![Build Status](http://runbot.odoo.com/runbot/badge/flat/1/master.svg)](http://runbot.odoo.com/runbot)
[![Tech Doc](http://img.shields.io/badge/master-docs-8f8f8f.svg?style=flat)](http://www.odoo.com/documentation/master)
[![Help](http://img.shields.io/badge/master-help-8f8f8f.svg?style=flat)](https://www.odoo.com/forum/help-1)
[![Nightly Builds](http://img.shields.io/badge/master-nightly-8f8f8f.svg?style=flat)](http://nightly.odoo.com/)

The gov-ngo Branches Readme
-------------------------

All odoo S.A. Branches have a build in phone home functionality by default and show the odoo S.A. branding on multiple places in the frontend, which is not suitable for most governmental-, official-, non governmental organisational- and even for projetcs of companies and anybody who cares about the privacy of their users (internal and external).

Often NDA's needs to be signed, which state very clearly, that no information is allowed to be given to a third party without prior consent etc. Unfortunately until now this requirements can not be met with the current odoo S.A. branches.

Debranding and non phoning home deactivations usually get implemented by additional modules. They overwrite the given functionality from the original odoo S.A Branches and need to be installed separately.

Problem: 
If the module is not working or for any other reason not doing its job, the fall back would be always the build in Phone Home to Odoo S.A. and Branding Functionality of Odoo S.A. - This is for us a No-Go Situation! Therefore all code of this kind need to get removed entirely from the actual code base, without exception. 

The default should always be NO BRAND - NO PHONING HOME!

Our goal is to create a non-branded and non-phoning back edition which is full compatible to odoo 9.0 as well as for odoo 8.0. Previous Versions will not be affected from this and will still contain a branding links and phoning back functionality.

Please report to us (issues) if you can find more places which contain phoning back functionality of any kind or Odoo S.A. branding of any kind which gets displayed to users in Versions 9 and 8). Thanks! 

Branding which only affects the code stays as is (i.e. copyright notices) according to AGPL v.3 / LGPL v.3

Beside that for many official use cases the systems used need to be accessible for people with disabilities. Also this is not the case with the standard odoo S.A. branches. 

* http://www.g3ict.org/resource_center/country_profiles/G3ict_White_Paper_-_Accessibility_Policy_Making/Germany

We will try to follow and implement the German Standards - which are one of the strongest in the world - 

* https://de.wikipedia.org/wiki/Barrierefreie-Informationstechnik-Verordnung
* http://www.barrierefreies-webdesign.de/bitv/bitv-2.0.html. 
* http://www.barrierefreies-webdesign.de/wcag2/
* http://www.bitvtest.de/bitvtest.html
* http://www.chemnitzer-14.de/accessibility-checkliste/ 

Odoo
----

Odoo is a suite of web based open source business apps.

The main Odoo Apps include an <a href="https://www.odoo.com/page/crm">Open Source CRM</a>, <a href="https://www.odoo.com/page/website-builder">Website Builder</a>, <a href="https://www.odoo.com/page/e-commerce">eCommerce</a>, <a href="https://www.odoo.com/page/project-management">Project Management</a>, <a href="https://www.odoo.com/page/accounting">Billing &amp; Accounting</a>, <a href="https://www.odoo.com/page/point-of-sale">Point of Sale</a>, <a href="https://www.odoo.com/page/employees">Human Resources</a>, Marketing, Manufacturing, Purchase Management, ...  

Odoo Apps can be used as stand-alone applications, but they also integrate seamlessly so you get
a full-featured <a href="https://www.odoo.com">Open Source ERP</a> when you install several Apps.


Getting started with Odoo
-------------------------
For a standard installation please follow the <a href="https://www.odoo.com/documentation/8.0/setup/install.html">Setup instructions</a>
from the documentation.

If you are a developer you may type the following command at your terminal:

    wget -O- https://raw.githubusercontent.com/odoo/odoo/master/odoo.py | python

Then follow <a href="https://www.odoo.com/documentation/8.0/tutorials.html">the developer tutorials</a>


For Odoo employees
------------------

To add the odoo-dev remote use this command:

    $ ./odoo.py setup_git_dev

To fetch odoo merge pull requests refs use this command:

    $ ./odoo.py setup_git_review

