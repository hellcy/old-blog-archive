## Welcome to GitHub Pages

* All IT related details will be put in here.

## DOM (Document Object Model)

* The Document Object Model (DOM) is an application programming interface (API) for HTML and XML documents. It defines the logical structure of documents and the way a document is accessed and manipulated.

## JavaScript
* JavaScript is a high-level, dynamic, weakly typed, prototype-based, multi-paradigm, and interpreted programming language. It is commonly used as a part of web pages, whose implementations allow client-side script to interact with the user and make dynamic pages. It is an interpreted programming language with object-oriented capabilities.

## jQuery
* jQuery is a JavaScript library designed to simplify the scripting of HTML. It is free and open-source. The purpose of jQuery is to make it much easier to use JavaScript on your website. jQuery takes a lot of common tasks that require many lines of JavaScript code to accomplish, and wraps them into methods that you can call with a single line of code. jQuery also simplifies a lot of the complicated things from JavaScript, like AJAX calls and DOM manipulation.

* DOM manipulation: 
* Get the <button> element with the class 'continue' and change its HTML to 'Next Step...'

```
$( "button.continue" ).html( "Next Step..." )
```

* Ajax
* Call a local script on the server /api/getWeather with the query parameter zipcode=97201 and replace the element #weather-temp's html with the returned text.

```
$.ajax({
  url: "/api/getWeather",
  data: {
    zipcode: 97201
  },
  success: function( result ) {
    $( "#weather-temp" ).html( "<strong>" + result + "</strong> degrees" );
  }
});
```

## Package Manager
* NuGet focusses mainly on .NET (there are a lot of non-.NET packages on NuGet however), NPM (Node Package Manager), Yarn and Bower are JavaScript package managers.

* Yarn was created by Facebook and Open Sourced. Speed comparisons found online show that Yarn is faster than NPM. Yarn is also able to install packages from a cache and does not require a connection to the Internet (only if a package was downloaded before).

## What is a Web Server?

* a web server is the software that receives your request to access a web page. It runs a few security checks on your HTTP request and takes you to the web page. Depending on the page you have requested, the page may ask the server to run a few extra modules while generating the document to serve you. It then serves you the document you requested.

* Apache is the most widely used web server software. Developed and maintained by Apache Software Foundation, Apache is an open source software available for free. It runs on 67% of all webservers in the world. It is fast, reliable, and secure. It can be highly customized to meet the needs of many different environments by using extensions and modules. Most WordPress hosting providers use Apache as their web server software.

* A web server like Apache, is also the Maitre D’ of the restaurant. It handles your communications with the website (the kitchen), handles your requests, makes sure that other staff (modules) are ready to serve you. It is also the bus boy, as it cleans the tables (memory, cache, modules) and clears them for new customers.

## What is the differences between .NET Framework and .NET Core?

* In 2002, Microsoft released .NET Framework 1.0 as a proprietary software framework for Windows platform. It has been updating the .NET Framework regularly to meet the emerging trends in software development. But Microsoft recently redesigned the core architecture of the .NET Framework to simplify development, testing, and deployment of modern software applications. The company released .NET Core 1.0 in June, along with ASP.NET Core 1.0 and Entity Framework.

* Unlike .NET Framework, .NET Core is both open source and cross-platform. It further comes with several new features to simplify development and testing of desktop, web, cloud, and mobile applications. Also, it allows developers to deploy the applications in a number of ways. But .NET Core does not support all features and functionalities of .NET Framework. Hence, it becomes essential for developers to understand the major differences between .NET Framework and .NET Core before switching to the most recent version of the popular software framework.

## MVC (Model-View-Controller)

* Model 
 
* The Model in MVC is a set of classes or project that describe your business logic. It represents all the business logic, like manipulating of data for your business/application, and data access operations like how you connect with database and get the data. In MVC, Model directly communicates with the Controller.
 
* View 
 
* The View in MVC are pages which we display to users, i.e., UI part which may consist of HTML, CSS, jQuery, JavaScript, etc. View part is actually completely responsible for displaying data. It takes data from the Controller and also sends back data to the Controller. It does not communicate directly with the Model.
 
* Controller 
 
* The Controller in MVC is the base of MVC architecture. Every request comes first to Controller then Controller requests the required information from Model and then it sends that information (data) to View in various formats. It works as a communicator and validator between View and Model.

## Framework in Programming

* Suppose you have to make a tea on daily basis with several ingredients like sugar, tea leaves , other spices , water etc. In doing so on daily basis most of the time u will find it is really difficult to put all ingredients in right ratio all time, u can forget some times u have to open several boxes one by one , one morning u come up with idea of mixing all ingredients in one jar in one ratio , such that every spoon will serve the right ratio mix to the tea. ( Off course milk and water remain aside :) )

* This jar is your framework. When we want to do lots of things on regular basis it just consumes time and a framework will not only save time it will also provide right components in ur applications. Fast and easy.

## Framework vs Library
* To understand this, let us see how we can use GSON library and Hibernate framework.

* Framework
* Consider we have to save student object in a database using Hibernate framework.

* To do this we have to do the following things.
* Create a file with name "hibernate.cfg.xml". And fill in the DB details in "hibernate.cfg.xml".
* Make your student class a java bean.
* Create a session object. Invoke the save method of session object. In save method pass the student object as an argument.
* If you notice we made the student class a java bean because hibernate wanted that.
* Hibernate has a rule. The object that hibernate persist should be an instance of Java bean. 
* This means if we want to use a framework, we have to change our code so that it follows the rules given by that framework.
The changes can be like 
* Define a method in our class. (example write getter and setter methods in student class in hibernate)
* Make our class implement an interface.

* Library
* Consider we have to convert our student object to json format using GSON Library.
* To do this we have to do the following things.
* Gson gson = new Gson();
* String json = gson.toJson(student);
* Please note we didn't change our student class to use GSON. 
* This means if we want to use a library, we need not change our existing code.

* So the difference is
* Framework and library are the code written by some one else. This code give us a functionality.
* In framework we change the structure of our code according to the rules given by them. In order to use the functionality provided by them.
* In library we can use the functionality directly without changing our code.

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

## Hibernate

* Hibernate is a middleware used for object-relational mapping(ORM) and for performing efficient object persistence. To understand about the architecture of Hibernate, let's first take a look at how Hibernate fits in the development of an application, between an application and the database server.

* A Java application code comprises of all the classes that define the business logic of application. These classes communicate with the Hibernate.

* Next comes, the Hibernate and its core interfaces, using which we could persist(store and retrieve) the objects of our business layer classes by communicating with the database server.

* Hibernate uses the Java core API, Java Database Connectivity(JDBC), Java Transaction API(JTA), Java Naming and Directory Interface(JNDI) to communicate with database in order to persist the state of object by performing create, read, update, delete(CRUD) operations.

## JPA

* JPA is the interface while Hibernate is the implementation.

* Traditionally there have been multiple Java ORM solutions: Hibernate, TopLink, JDO
 
* each implementation defining its own mapping definition or client API. The JPA expert group gathered the best of all these tools and so they created the Java Persistence API standard.

* A standard persistence API is very convenient from a client point of view, making it relatively easy to switch one implementation with the other (although in practice it's not that simple because on large projects you'll have to use specific non-standard features anyway).

## Continuous integration and Jenkins

* Continuous Integration (CI) is a development practice where developers integrate code into a shared repository frequently, preferably several times a day. Each integration can then be verified by an automated build and automated tests. While automated testing is not strictly part of CI it is typically implied.

* One of the key benefits of integrating regularly is that you can detect errors quickly and locate them more easily. As each change introduced is typically small, pinpointing the specific change that introduced a defect can be done quickly.

* In recent years CI has become a best practice for software development and is guided by a set of key principles. Among them are revision control, build automation and automated testing.

* Additionally, Continuous Deployment and Continuous Delivery have developed as best-practices for keeping your application deployable at any point or even pushing your main codebase automatically into production whenever new changes are brought into it. This allows your team to move fast while keeping high quality standards that can be checked automatically.

* Continuous integration is a process in which all development work is integrated as early as possible. The resulting artifacts are automatically created and tested. This process allows to identify errors as early as possible.

* Jenkins is a popular open source tool to perform continuous integration and build automation. The basic functionality of Jenkins is to execute a predefined list of steps, e.g. to compile Java source code and build a JAR from the resulting classes. The trigger for this execution can be time or event based. For example, every 20 minutes or after a new commit in a Git repository.

* Possible steps executed by Jenkins are for example:

* perform a software build using a build system like Apache Maven or Gradle

* execute a shell script

* archive a build result

* running software tests

* Jenkins monitors the execution of the steps and allows to stop the process, if one of the steps fails. Jenkins can also send out notification in case of a build success or failure.

## What is POJO

* POJO stands for “Plain Old Java Object” — it’s a pure data structure that has fields with getters and possibly setters, and may override some methods from Object (e.g. equals) or some other interface like Serializable, but does not have behavior of its own. It’s the Java equivalent of a C struct

## Angular 

* Angular is an open source JavaScript framework which simplifies binding code between JavaScript objects and HTML UI elements.

* Angular JS, Node.js, Ember, Vue.js and React.js are all front end framework.

## Node.js

* NodeJS is an open source JavaScript framework which does two things: -

* It helps you to run JavaScript outside the browser. NodeJS uses the chrome JavaScript engine to execute JavaScript outside the browser so that we can create desktop and server based application using JavaScript.

* It also acts a central repository from where we can get any JavaScript framework using NPM (Node package manager).
