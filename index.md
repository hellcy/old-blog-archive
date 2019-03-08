## Welcome to GitHub Pages

* All IT related details will be put in here.

## What is a Web Server?

* a web server is the software that receives your request to access a web page. It runs a few security checks on your HTTP request and takes you to the web page. Depending on the page you have requested, the page may ask the server to run a few extra modules while generating the document to serve you. It then serves you the document you requested.

* Apache is the most widely used web server software. Developed and maintained by Apache Software Foundation, Apache is an open source software available for free. It runs on 67% of all webservers in the world. It is fast, reliable, and secure. It can be highly customized to meet the needs of many different environments by using extensions and modules. Most WordPress hosting providers use Apache as their web server software.

* A web server like Apache, is also the Maitre D’ of the restaurant. It handles your communications with the website (the kitchen), handles your requests, makes sure that other staff (modules) are ready to serve you. It is also the bus boy, as it cleans the tables (memory, cache, modules) and clears them for new customers.

## What is the differences between .NET Framework and .NET Core?

* In 2002, Microsoft released .NET Framework 1.0 as a proprietary software framework for Windows platform. It has been updating the .NET Framework regularly to meet the emerging trends in software development. But Microsoft recently redesigned the core architecture of the .NET Framework to simplify development, testing, and deployment of modern software applications. The company released .NET Core 1.0 in June, along with ASP.NET Core 1.0 and Entity Framework.

* Unlike .NET Framework, .NET Core is both open source and cross-platform. It further comes with several new features to simplify development and testing of desktop, web, cloud, and mobile applications. Also, it allows developers to deploy the applications in a number of ways. But .NET Core does not support all features and functionalities of .NET Framework. Hence, it becomes essential for developers to understand the major differences between .NET Framework and .NET Core before switching to the most recent version of the popular software framework.

## What is Spring Framework

* 1) You can use Spring Framework for writing web applications:

If your project would be available from the browser, it is a web application. Spring Framework has a module called Spring MVC that you can leverage to develop web pages.

You will get validation, security, templating, internationalization and several other things either as built-in or easily available for integration.

* 2) You can use Spring Framework for exposing RESTful services:

If you decide to use JavaScript based frameworks (Angular JS, Ember JS, BackBone etc) for building web pages, they will need data. You can then use Spring MVC to send them this data via RESTful URL.

* 3) You can use Spring Framework to secure your web applications.

I am sure your project / product will have users and they will have some roles. Roles define things they can do that others can't.

With Spring Security subproject of Spring Framework, you can plug and play just about any authentication and/or authorization mechanism to include in your project.

I have used it to authenticate facebook users (spring-social, spring security and OAuth2).

I have used it to authenticate LDAP users.

I have used it to authenticate database users.

I have used it to authenticate users from a database table. Some of the databases I used: Oracle, MySQL, MongoDB.

* 4) You can use Spring Framework for communicating with databases.

I used Spring Framework to talk to Oracle, MySQL, MongoDB, Redis. I used it with Hibernate, MyBatis (and previously iBatis), Spring Data (another subproject) and Spring JDBC (spring module).

* 5)You can use Spring Framework for handling long running jobs.

Your project may not even be a web application to use Spring Framework. I used Spring Batch (subproject) to handle long running jobs. These could be anything that takes a long time and you want to be able to run them without waiting for it.

I used it to run long running SQL that updated millions of rows in the database.

* 
