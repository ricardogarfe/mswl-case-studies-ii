==============================
Thunderbird Quality Assurance 
==============================

"Community Talk":http://blip.tv/mswl/case-studie-ii_quality-assurance-in-thunderbird-and-mozilla-5906218 by Ludovic Hirliman (http://perso.hirlimann.net/~ludo/)

Quality Assurance 
==================

why where how 

QA you must write as simple as you know

Unit test, integration test between Frontend Server SQL.


Test Driven Development
========================

Wrinting Test cases has three ways:

* Test Cases - What the specs are ? button -> circle.
* Ad-hoc testing - Test by yourself without test spec. Creativity but not a good thing to do because only fits to one solution. Has to become Test case to test in every version.
* Unit Testing - Not at every build.

For each test type you have:

* Functional Testing - press button A -> Red circle, Web Service - 1K Users/ 10K Users/ 100K Users % working. Email client sends emails.
* Load Testing - 2m emails - No unit test.

QA
===

Maintain Tests
---------------

If you have 1000 test cases, maintain all could be a suffer. If software changes a lot and often, difficulty increases.

* Accuracy - compare test results between version 1 and version 2.
* Managing bugs - Make sure that exists and replicate it.
    * Exists ?
    * Bug description. Figure out steps to reproduce.

work with some test aren't

Tools
======

Test case manager
------------------

Be able to:

* Record test cases.
* Test associated by every version.

Create Charts from Test results: applies, success % and why (tested, fail, ok).

Have a bug in 1.1 - fixed in 1.2 - test again 1.3

Bug report tools - JIRA (why Java), Bugzilla, Trac, etc.

"Testing Tools your hand, your brain and time."

Scripting functional testing - Selenium - integration web tests.

Projects
=========

* Web app easy - url and parameters.
* Desktop Software - ie pdf readers. Difficult to emulate a human, antivirus, graphic card drivers, windows versions, multiple versions and environments.

QA in Mozilla
==============

What do we do at Mozilla ?

* Firefox
* Fennec
* Thunderbird ?
* Some web apps: Sync, browserId, etc...

30 people and one QA per project. In Firefox there are QA teams per versions.

All is FLOSS. 

Best QA: "Using our users to make the product better".

Test days: Different team every Friday. Debug new functionalities with users communicating via irc and replicate test cases with users. Volunteers for build and run tests for some applications but in thunderbird nobody build one :(

Development Tools
==================

Bug Tracking Sustem - Bugzilla - Everyone could post a bug and how to replicate a bug there.
Test case mangament software - Litmus (https://mail.mozilla.org/pipermail/thunderbird-testers/2012-October/000111.html) to Moztrap.
  * Limus - (http://litmus.com/) Test interactively with real email clients.
  * Moztrap - (http://moztrap.wordpress.com/) Test Case Management from Mozilla.
Continuous Integration - Boildbot (http://trac.buildbot.net/) - Checkout, run make, run make test, read log file and automate a build in every commit. Running unit test to build after each commit.
Documentation - Wiki to develop extensions and a real user Wiki.
Communication - IRC as main communication channel, group chats, history.
Testing Tool - Selenium - (http://docs.seleniumhq.org/) Framework to automate browser testing.

After trow away all spaghetti code in 2009, next QA goal in January 2010 was: "To add code to Thunderbird developers have to develop tests". After those steps the project obtain more volunteers. The code you write matters and its easy to contribute, collaborate and test.

How to Contribute
==================

Development - Reporting bugs, patches and contributing with code.
QA - After failling Friday test, they change the question: "Do you want to contribute with test ?" Thus they manage people and explain what and how they 'have to' test. Its an easier way to start to collaborate instead of "Someone wants to test ? go to url, test and report bugs". Better and easy as human way.
Support - Translations and localizations.
Marketing - Mozilla products Evangelist. Spreading the goods and benefits of MOFO products.

What we do in Mozilla
======================

MOFO Mozilla Foundation.

Bugzilla.

