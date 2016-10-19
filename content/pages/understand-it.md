Title: Understand It
url: understand-it
save_as: understand-it.html
section: understand
index: 0

Understand It
==========

What is Arrebol?

------

Arrebol has three main components:
Submission service: The submission service is the deamon responsible for receiving job submission and monitoring requests and interacting with the fogbow middleware to execute the jobs in the federated cloud resources. The submission services runs a REST interface acessed by two clients: Arrebol CLI and Arrebol Dashboard.
Arrebol CLI: CLI is a bash script to easy interaction with the submission service in UNIX enviroments. It allows to submit jobs, retrieve status information about running jobs, and cancel them.
Arrebol Dashboard: Dashboard is a web application that shows status information about the jobs controlled by a submission service.
This document provides a short guide to use the Arrebol CLI to interact with the Submission Service. It also describes how to install and configure the Submission Service and the Arrebol Dashboard.


