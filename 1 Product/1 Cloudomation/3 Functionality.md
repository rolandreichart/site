# Functionality

As a general purpose automation software platform, Cloudomation provides a wide range of low-level functionality that is generically applicable to software automation in different contexts. Here, we will try to give an overview of that range of functionality Cloudomation offers. For more details on individual functions, please refer to the [documentation](/documentation/Tutorial).

## Control other software
At the core of Cloudomation sit a range of functions that allow to control and therefore automate other software solutions. The only prerequisite a software solution has to fulfil so that it can be automated with Cloudomation is that it has to have some kind of application programming interface (API).  

APIs are standard interfaces that allow communication between software solutions. Cloudomation can work with different kinds of APIs. One very common type of API are REST APIs. These are web APIs that allow to send commands to or request information from software platforms, servers, or web services. As one example of Cloudomation functionality, the REST task type allows interaction with REST APIs through Cloudomation.

Being able to interact with APIs through Cloudomation enables you to issue commands and request information from a large number of software solutions - as long as it has an API, it can be automated with Cloudomation.

## Communicate with other systems
Communicating with other systems enables you to build automation workflows that are contingent on other systems. You can create automations that react to their environment, that only happen when specific conditions are met, or that react to changes in other systems.

As an example, you can automate a cleanup task that compresses some files and moves them to an archive whenever the disk space on your system is filled up to a limit you define.

Cloudomation offers functionality that allows you to use a range of standard communication protocols that allow structured exchange of information between systems. APIs are one method for communicating with other systems that we already mentioned. Other methods available in Cloudomation are websockets, ssh connections, and more.

## Access, process, and write data
Another central aspect to software automation is the ability to securely and efficiently process data.
Data play a central part in many software processes. As such, automatic access to, processing, and writing of data are essential features that an automation software must fulfil.

Cloudomation offers functionality that allows you to access file systems - for example via the SSH task - and databases - for example using the REDIS task.

As an example, your automation could include queries to a relational database and a data web service, then trigger an ETL process to combine and structure the data so that it is fit for processing, which happens through an R script prepared by your data scientists. Cloudomation can collect the data, trigger the ETL, wait for the results to be ready, trigger the R script once the data preparation is complete, collect the restults from the R script and write them back into a relational database.  
As a next step, Cloudomation could trigger an automated campaign, defined in your campaigning tool, which uses scores produced by the R script to select customers for the campaign target group.

Another important feature enabled by Cloudomation's data processing funcions is the ability to closely monitor and log all processes automated in Cloudomation. Cloudomation can write all intermediate results of an automated workflow into a log file or a database, and clean them up if and when the automation workflow concludes successfully. If the workflow fails, you have a complete audit trail to support root cause analysis.

Or you can use Cloudomation to periodically access other systems, check some metrics, and collect them into a report - this can be used for automatic health monitoring of servers, or to ensure the proper loading of data into a databse, etc.

## Involve users in automated processes
As important as automation is, we are not yet at a point where everything can be automated - and even if you could, you might not always want to. Therefore, Cloudomation offers functionality that allows you to involve users into automated workflows.

One example are decisions: your flow script could include certain decision points, or conditions under which a user has to make a decision. For example, you could have a fully automated workflow for sending out invoices to your customers. However you might want to include thresholds for invoice amounts, above which invoices are not sent out without a human giving the go-ahead. This can help you identify your most valuable customers.

Another example of user involvement in automated workflows is the automation of tasks that need input from users. One example from the Cloudomation platform is user creation: the user needs to input their username and password. The rest is done by a flow script. Similar examples could involve automatic set-up of workstations for new colleagues in your organisations. You might want to enable them to pick and choose between different options of browsers, for exmaple, or enable them to pick some additional tools that not everybody might need.

A different aspect of user involvement are notifications that do not require a response. You can use Cloudomation functionality to let your flow script inform you of certain things via email.

For example, you might want your flow script to send you an email whenever a customer places an order on your website that exceeds a certain value. Or you might want your flow script to send you an email whenever a business critical process that runs once per month ends - with information if it completed successfully or failed.

Apart from Cloudomation functionality that you can directly use in flow scripts to request input from users, or send email notifications, it is possible to use the Cloudomation REST API to build your own, customised user interface on top of Cloudomation flow scripts. This enables you to use Cloudomation for automations in the background of any application you use in your organisation, such as your website or an internal self-service portal. The buttons your users click do not have to be on the Cloudomation platform itself - they can be on your website or app, which trigger an API call to the Cloudomation platform to start a flow script.

## Modularise: manage interaction between automations
So far, we have looked at Cloudomation functionality that enables you to build powerful automations. Now, we will look at functionality that enables you to build automations that are beautiful, stable, easily maintainable, and extendable, so that they can grow with your business and your needs.

Cloudomation supports you in building high quality automations by providing a range of functionality to manage the interaction of individual automations with each other. This enables you to build atomar, small flow scripts that manage individual tasks, or well defined aspects of a process, which interact with other flow scripts to complete the automation of complex processes.

As an example, you might want to use Cloudomation to automate the ordering process on your website. You currently have a certain set of products that your customers can order on your website. But this set of products is likely to change in the future: you might add new products to your range, or modify existing ones to include additional features, or retire products.

With Cloudomation, you can define each step in the automated ordering process to follow the same, generic overall process. The customer will select which product they want, how many pieces, and might need to input some configurations, such as color or size. Each of these aspects that are individual to a specific product, and which might change in the future, can be defined in their own flow scripts, or in separate configuration files.

Now as your customer moves through the order process, different flow scripts are triggered in the background, depending on which product they choose and maybe which payment option they select.

The flow scripts can seamlessly interact with each other, and you can extend your workflow with as many alternative process paths as you need. Adding a new product becomes the work of minutes, because all you have to do is add one more configuration file, which your flow script will pick up and guide your customer through the right process on your website.


As an example, you might want to automate the set up of workstations for new colleagues in your organisation. Currently, you might only offer your colleagues a choice of three computers, all of which run Windows as an operating system. But in the future, you might want to add Apple computers, or even Linux machines to your inventory. The general outline of the automatic set-up will have many similar parts between all these different work stations. In all of them, a user will need to provide some information such as their name and password for log in. They will need to select which software to install, and




to create complex automation workflows with many dependencies
