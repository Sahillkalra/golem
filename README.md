Golem - Test Automation Framework 
[![Build Status](https://travis-ci.org/lucianopuccio/golem.svg?branch=master)](https://travis-ci.org/lucianopuccio/golem)
[![Documentation Status](http://readthedocs.org/projects/golem-framework/badge/?version=latest)](http://golem-framework.readthedocs.io/en/latest/?badge=latest)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
==================================================


Intro
--------------------------------------

>Automate end to end tests in minutes, not hours.


Golem is a complete test automation tool and framework for end-to-end testing. It creates powerful, robust and maintainable test suites, yet it is easy to pick up and learn even without a lot of programming knowledge. It is based on Selenium Webdriver and it can be extended using Python.

**It can:**
* Use the Page Object pattern
* Write tests with multi data sets (data-driven)
* Run tests in parallel.
* Test APIs
* Run tests remotely (Selenium Grid or a cloud testing provider)
* It can be executed from Jenkins or any other CI tool 


**It has:**
* A complete GUI module (a web application) to write and execute tests
* A reporting engine and a web reports module
* An interactive console


***

## Contents

* [Screen Captures](#screen-captures)
* [Pre-requisites](#pre-requisites)
* [Installation](#installation)
* [Quick Start](#quick-start)
* [Documentation](#documentation)
* [Example Projects](#documentation)
* [Roadmap](#roadmap)
* [License](#license)


Screen Captures
--------------------------------------

**Project Dashboard**
<p align="center">
    <img width="700" style="border: 1px solid #d3d3d3; padding: 5px" src="./images/project-dashboard.png" />
</p>

**Test Editor**
<p align="center">
    <img width="700" style="border: 1px solid #d3d3d3; padding: 5px" src="./images/test-case.png" />
</p>


**Test as Pure Python Code**
<p align="center">
    <img width="700" style="border: 1px solid #d3d3d3; padding: 5px" src="./images/example-test-code.png" />
</p>


**Report Dashboard**
<p align="center">
    <img width="700" style="border: 1px solid #d3d3d3; padding: 5px" src="./images/report-dashboard.png" />
</p>

**Execution Report**
<p align="center">
    <img width="700" style="border: 1px solid #d3d3d3; padding: 5px" src="./images/execution-report.png" />
</p>


Pre-requisites
--------------------------------------

Basic knowledge of Selenium Webdriver is required. Check out [this docs](golem-framework.readthedocs.io/en/latest/installation.html) first.


Installation
--------------------------------------

Golem works with Python 3.4+

```
pip install golem-framework
```

Read the full installation guide here: [http://golem-framework.readthedocs.io/en/latest/installation.html](golem-framework.readthedocs.io/en/latest/installation.html)


Quick Start
--------------------------------------

**Create a test directory anywhere in your machine**

```
golem-admin createdirectory <test_directory>
```

**Download the latest webdriver executables** 
Note: Golem needs the latest webdrivers in order to work, by default, it will pick up the executables placed in the <test_directory>/drivers directory, this setting can be overriden from the settings.
The latests versions of the webdrivers can be found here:
* Chrome: (https://sites.google.com/a/chromium.org/chromedriver/)
* Firefox: (https://github.com/mozilla/geckodriver/releases)

For more information check [this page](http://golem-framework.readthedocs.io/en/latest/web-drivers.html) of the documentation.

**Start the Web Module**

```
cd <test_directory>
python golem.py gui
```


The Web Module can be accessed at http://localhost:5000/

By default, the following user is available: username: *admin* / password: *admin*


Documentation
--------------------------------------

Read the full documentation here: [http://golem-framework.readthedocs.io/](http://golem-framework.readthedocs.io/)


Example Projects
--------------------------------------

Here is a repo with example working projects usign Golem: [https://github.com/lucianopuccio/golem-demo](https://github.com/lucianopuccio/golem-demo)

Roadmap
--------------------------------------

Integrate with Appium for mobile testing


License
--------------------------------------

[MIT](https://tldrlegal.com/license/mit-license)