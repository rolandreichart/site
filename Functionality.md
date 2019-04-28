# Functionality

As a general purpose automation software platform, Cloudomation provides a wide range of low-level functionality that is generically applicable to software automation in different contexts. Here, we will try to give an overview of that range of functionality Cloudomation offers. For more details on individual functions, please refer to the [documentation](/documentation/Tutorial).

## Control other software
At the core of Cloudomation sit a range of functions that allow to control and therefore automate other software solutions. The only prerequisite a software solution has to fulfil so that it can be automated with Cloudomation is that it has to have some kind of application programming interface (API).  

APIs are standard interfaces that allow communication between software solutions. Cloudomation can work with different kinds of APIs. One very common type of API are REST APIs. These are web APIs that allow to send commands to or request information from software platforms, servers, or web services. As one example of Cloudomation functionality, the REST task type allows interaction with REST APIs through Cloudomation.

As an example, you can use Cloudomation to automatically look for and install security updates for your IT infrastructure every night, so that your infrastructure is always up to date and you are not disturbed in your work by the updates.

Being able to interact with APIs through Cloudomation enables you to issue commands and request information from a large number of software solutions - as long as it has an API, it can be automated with Cloudomation.

## Communicate with software and systems
Communicating with different software solutions and systems allows you to build intelligent automation workflows that can react to their environment. Your automation workflows can react to changes in your environment, or be triggered by specific events, or ask for input and execute different automations depending on what input they receive.

As an example, you can automate a cleanup task that compresses some files and moves them to an archive whenever the disk space on your system is filled up to a limit you define.

As another example, you can use Cloudomation to automate the exchange of information between your warehousing solution, your cash register software, and your web shop: Cloudomation can make sure that sales via the cash register or your web shop are synchronised with your warehousing software so that your stock counts are always correct.

Cloudomation offers functionality that allows you to use a range of standard communication protocols that allow structured exchange of information between systems. APIs are one method for communicating with other systems that we already mentioned. Other methods available in Cloudomation are websockets, ssh connections, and more.

## Access, process, and write data
Another central aspect to software automation is the ability to securely and efficiently process data.
Data play a central part in many software processes. As such, automatic access to, processing, and writing of data are essential features that an automation software must fulfil.

Cloudomation offers functionality that allows you to access file systems - for example via the SSH task - and databases - for example using the REDIS task.

As an example, your automation could include queries to a relational database and a data web service, then trigger an [ETL](https://en.wikipedia.org/wiki/Extract,_transform,_load){ext} process to combine and structure the data so that it is fit for processing, which could be done with an R script prepared by your data scientists. Cloudomation can collect the data, trigger the ETL, wait for the results to be ready, trigger the R script once the data preparation is complete, collect the restults from the R script and write them back into a relational database.  
As a next step, Cloudomation could trigger an automated campaign, defined in your campaigning tool, which uses scores produced by the R script to select customers for the campaign target group.

Another important feature enabled by Cloudomation's data processing functions is the ability to closely monitor and log all processes automated in Cloudomation. Cloudomation can write all intermediate results of an automated workflow into a log file or a database, and clean them up if and when the automation workflow concludes successfully. If the workflow fails, you have a complete audit trail to support root cause analysis.

Or you can use Cloudomation to periodically access other systems, check some metrics, and collect them into a report - this can be used for automatic health monitoring of servers, or to ensure the proper loading of data into a database, etc.

## Involve users in automated processes
As important as automation is, we are not yet at a point where everything can be automated - and even if you could, you might not always want to. Therefore, Cloudomation offers functionality that allows you to involve users into automated workflows.

One example are decisions: your flow script could include certain decision points, or conditions under which a user has to make a decision. For example, you could have a fully automated workflow for sending out invoices to your customers. However you might want to include thresholds for invoice amounts, above which invoices are not sent out without a human giving the go-ahead. This can help you identify your most valuable customers.

Another example would be automatic set-up of workstations for new colleagues in your organisations. You might want to enable them to pick and choose between different options of browsers, for example, or enable them to pick some additional tools that not everybody might need.

Apart from Cloudomation functionality that you can directly use in flow scripts to request input from users, it is possible to use the Cloudomation REST API to build your own, customised user interface on top of Cloudomation flow scripts. This enables you to use Cloudomation for automations in the background of any application you use in your organisation, such as your website or an internal self-service portal. The buttons your users click do not have to be on the Cloudomation platform itself - they can be on your website or app, which trigger an API call to the Cloudomation platform to start a flow script.

## Modularise: manage interaction between automations
So far, we have looked at Cloudomation functionality that enables you to build powerful automations. Now, we will look at functionality that enables you to build automations that are beautiful, stable, easily maintainable, and extendable, so that they can grow with your business and your needs.

Cloudomation supports you in building high quality automations by providing a range of functionality to manage the interaction of individual automations with each other. This enables you to build atomar, small flow scripts that manage individual tasks, or well defined aspects of a process, which interact with other flow scripts to complete the automation of complex processes.

As an example, we can think of software you have installed in the cloud. Maybe you have your own cloud subscription with Amazon Web Services, Azure, Google Cloud, or any other provider. You have some software installed on that platform that your colleagues use for their work. Now, during the weekend, your colleagues don't usually work, so you don't need to keep the cluster at full size, or might even be able to shut it down completely during the weekends to save cost. With Cloudomation, you can automate the installation of all components, so that creating a new cluster with all your software only takes a few minutes and automatically happens every Monday morning.

You have a certain set of software installed there right now. But that will change in the future. You might want to add more components, you might remove others, or install other versions of the software you use. In Cloudomation, you would define the installation and configuration of components in individual flow scripts that interact with each other - one flow script will trigger others, which install and configure individual components.

In this way, it becomes very easy for you do just add another small flow script to your workflow, or change a configuration, or remove one step. Cloudomation enables you to keep track of the big picture, make changes simple, and allows you to easily see which flow scripts interact with which other flow scripts and configurations, so that you always know where to apply your changes.

In this way, Cloudomation allows you to automate very complex processes, and makes them maintainable.
