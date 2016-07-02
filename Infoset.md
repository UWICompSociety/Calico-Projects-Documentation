#Infoset Documentation

#Purpose
Infoset provides status reports on the operations of computer equipment connected to the internet. It is ideal for network admins and system admins that uses snmp to walk through the network, dumps snmp data, parses it and presents it as an api/interface.

It can be described as a Python3 inventory system that reports and tabulates status of network connected devices.Eg.Network port names ,speed,state,neighbours,VLANS,802.11,ARP. For more information http://wiki.palisadoes.org/index.php/Infoset#Introduction 

#Overall Architecture

To be added

#Folder Structure
All packages reside in the lib directory. It has the following structure
* getdata: Classes that retrieve data
* getdata/snmp: Contains classes that retrieve data via SNMP
* getdata/files: Contains classes that retrieve data from files
* web: Classes that render web pages
* web/snmp: Classes that render web pages from snmp data

#Order of Reading Source Files
When reading the source files it is recommended to start with server.py and www/views.py. For anyone who wants to work on the backend then start with toolbox.py.

#Style guides
For ease of readability and maintainability infoset code must follow these guidelines. Code that does not comply will not be added to the master branch.
* infoset uses the Google Python Style Guide for general style requirements
* infoset uses the The Chromium Projects Python Style Guidelines for docstrings.
* Indentations must be multiples of 4 blank spaces. No tabs.
* All strings must be enclosed in single quotes
* In addition to being pylint compliant, the code must be PEP8 and PEP257 compliant too.
* There should be no trailing spaces in files

#Examination of key batches of key code

To be done

#Helpful Videos

* https://www.youtube.com/playlist?list=PLJ5-XuEkSCDk30ui3EowvW6TzXF2Hp4-5

* https://www.youtube.com/watch?v=ZX-XGQoISHQ

* https://www.youtube.com/watch?v=RD8hnhGCFcY

#Challenges

* It is very rooted in network technologies, (snmp, network gear, and networking concepts) much of you might not be familiar with.

* The learning curve is a bit steep.

#Tips

* Read on snmp and snmp in python and it's facets (OID numbers and MIB filed  and spend as much time getting familiar with the codebase, code style used.

* Ask your mentor for help.


#How do I contribute

* Below is the workflow for having your contribution accepted into the infoset repository.
* Create an Issue or comment on an existing issue to discuss the feature
* If the feature is approved, assign the issue to yourself
* Fork the project
* Clone the fork to your local machine
* Run make setup to install dependencies to virtualenv (information about virtualenv found further below in this doc)
* Add the original project as a remote (git remote add upstream https://github.com/UWICompSociety/infoset, check with: git remote -v)
* Create a topic branch for your change (git checkout -b branchName)
* you may create additional branches if modifying multiple parts of the code
* Write code and Commit your changes locally. Example proper git commit message below:
* Make the example in CONTRIBUTING imperative and concrete ...
* Without this patch applied the example commit message in the CONTRIBUTING document is not a concrete example. This is a problem because the contributor is left to imagine what the commit message should look like based on a description rather than an example. This patch fixes the problem by making the example concrete and imperative.
* The first line is a real life imperative statement with a ticket number from our issue tracker. The body describes the behavior without the patch, why this is a problem, and how the patch fixes the problem when applied.
* Resolves Issue: #123 See also: #456, #789
* When you need to synch with upstream (pull the latest changes from main repo into your current branch), do: git fetch upstream -> -> git merge upstream/master. (or run make synch to let the project's makefile handle syncing)
* Check for unnecessary whitespace with git diff --check.
* Write the necessary unit tests for your changes.
* Run all the tests to assure nothing else was accidentally broken (run: make test)
* Push your changes to your forked repository (git push origin branch)
* Perform a pull request on github
* Your code will be reviewed
If your code passes review, your pull request will be accepted

The make contribute command encapsulates steps 8 to 12 when you are ready to make a pull request. The make synchcommand will sync your repository

#Descriptions






  




