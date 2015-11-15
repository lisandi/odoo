[![Build Status](http://runbot.odoo.com/runbot/badge/flat/1/master.svg)](http://runbot.odoo.com/runbot)
[![Tech Doc](http://img.shields.io/badge/master-docs-8f8f8f.svg?style=flat)](http://www.odoo.com/documentation/master)
[![Help](http://img.shields.io/badge/master-help-8f8f8f.svg?style=flat)](https://www.odoo.com/forum/help-1)
[![Nightly Builds](http://img.shields.io/badge/master-nightly-8f8f8f.svg?style=flat)](http://nightly.odoo.com/)

The gov-ngo Branches Readme
-------------------------

All odoo S.A. Branches have a build in phone home functionality and show their branding on multiple places which is not suitable for most governmental-, official-, non governmental organisational- and even for projetcs of company and anybody who cares about the privacy of their users (internal and external).

Often you have even to sign NDA's which state very clear, that no information is allowed to be given to a third party without prior consent etc. Unfortunately until now this requirements can not be met with the current odoo S.A. branches.

Often debranding and non phoning home gets done by modules which need to be installed. They overwrite the given functionality from the original odoo S.A Branches.

Problem: 
If the module is not working or for any other reason not doing its job, the fall back would be always the build in Phone Home and Branding Functionality of Odoo S.A. - This is for us a No Go Situation. Therefore all codes of this kind need to get removed from the actual code base, without exception. The default should always be NO BRAND - NO PHONING HOME!

Our goal is to create a non-branded and non-phoning back edition which is full compatible to odoo 9.0 as well as for odoo 8.0. Previous Versions will not be affected from this and will still contain a branding links and phoning back functionality.

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

