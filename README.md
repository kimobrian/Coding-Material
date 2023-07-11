<!-- Output copied to clipboard! -->

<!-- You have some errors, warnings, or alerts. If you are using reckless mode, turn it off to see inline alerts.
* ERRORs: 0
* WARNINGs: 0
* ALERTS: 3 -->

<p style="color: red; font-weight: bold">>>>>>  gd2md-html alert:  ERRORs: 0; WARNINGs: 0; ALERTS: 3.</p>
<ul style="color: red; font-weight: bold"><li>See top comment block for details on ERRORs and WARNINGs. <li>In the converted Markdown or HTML, search for inline alerts that start with >>>>>  gd2md-html alert:  for specific instances that need correction.</ul>

<p style="color: red; font-weight: bold">Links to alert messages:</p><a href="#gdcalert1">alert1</a>
<a href="#gdcalert2">alert2</a>
<a href="#gdcalert3">alert3</a>

<p style="color: red; font-weight: bold">>>>>> PLEASE check and correct alert issues and delete this message and the inline alerts.<hr></p>



## Technical Coding Resources

This is a document that is still WIP(Work in Progress) that will introduce a learner to computers and programming and guide them through learning programming concepts using Python. At the end of this tutorial, a learner should be able to:



* Setup a python programming environment from the editors to installing Python, git and other necessary coding tools.
* Understand basic computing functionality, define syntax, define different memories and how computers work in relation to software.
* Define version control and use most common git concepts
    * Create repos on github
    * Setup repo locally and link with github
    * Stage, commit, branch and push code
    * Extra concepts to learn should include:
        * Resetting the git history
        * Git stashing
        * Creating pull requests
        * Resolving merge conflicts
* Write fully functioning programs in python which should demonstrate their understanding of:
    * Python syntax and data types
    * Functions, arguments, parameters, args, kwargs etc
    * Python modules and packages
    * Classes(Object oriented programming)
    * Setting up and using virtual environments and using pipenv.
    * Jupyter Notebook basics
* Web and API(application programming interface) creation using FAST API and Flask


## Understanding Basics of Programming and Computers

Learn the fundamentals of computers and programming.

These links' content will introduce you to how computers work. You'll get a high level understanding of computer memory, hardware and software concepts. If you've never been to a computer science class(even if you;ve been), this is a very important intro to different concepts that will make you understand how computers work.

For example, from the top of my head I can tell you how a program works. If you've a program to add 2 numbers: 

  function addition(x, y) {

        return x+y  

  }

In programming they're called functions(old languages call them procedures). The function takes two variables(values that can change their value) and returns their sum. The computer reads the program and stores it into memory. It stores the variables you provide in memory too. When it wants to execute the function, it reads these values into RAM(temporary high speed memory where programs are stored during execution). This is like picking a task from a queue and starting to work on it. The processor(CPU) reads from RAM, performs the summation in the ALU(arithmetic and logic unit) and returns the result. These results will then be displayed to the user. There's a lot that goes on like how many tasks are on the queue, how does the processor determine the next task, what if a task is taking too long with the processor that other tasks "starve" on the queue. What if task A holds onto a resource that another task B requires while task B holds onto a resource that A requires, they're in a deadlock. The CPU has ways of scheduling these tasks using different algorithms/methods. You don't need to know everything, just the basics are enough. We defined the above function but how do we use it?

There's defining a function and using it(calling the function). And this is how we call it.

         		sum = addition(56,78)

So after this, the value of sum should be 134. Think of this like an algebraic equation. x+y=z is the function definition. Now take x = 56 and y=78, find z. Does it make sense?

The function also has different parts that you will get to learn as you proceed.



* [Absolute beginner's guide to computers and programming](https://www.educative.io/blog/beginners-guide-to-computers-and-programming)
* [Computer Science 101: hardware vs. software components](https://www.educative.io/blog/hardware-vs-software-components-computer)
* [Learn How to Code: the beginner's guide to coding and syntax](https://www.educative.io/blog/learn-how-to-code-beginners-guide)


## Version Control

**NOTE: This is a chapter you can skip(for now) and come back to after learning some coding basics but it's very crucial. The goal is you apply git all the time you write code to make it a habit.**


### Git and Github

This section will teach you a concept called version control. At some point when doing assignments in Microsoft Word, we save the first version of the document as v1, when we make changes we save as v2, v3 etc. This process is manual and cumbersome and you can't clearly tell the difference with different versions if the document is more than 2 pages. You can also not tell when a change happened or when a problem happened or who made a change in case more than one person is working on the document. With Version Control, we get to control every aspect of this. 

Note: Version Control systems can be used for more than just code. Do you want to use this with you word documents? You can. You can make a change today, add another next week, next month, next year in the same document and you'll be able to jump between all the versions of the documents even after 10 years. You can go back to when you had one page and come back to when you;ve 200 pages. You can collaborate and compare new changes and merge them, you can undo anything with no issue. For example, below is the history of code I've been working on. It clearly shows who, when and what I did. Using some command, I can jump to a certain version and the document will automatically show how it was then.



<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image1.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image1.png "image_tooltip")


**<span style="text-decoration:underline;">Objectives</span>**



* Understand version control
* What is git?
* What is github?
* What is the difference between git and github?
* Are there any other version control systems(e.g subversion, mercurial) and code hosting servers(e.g gitlab, bit bucket)
* Create a github account
* Learn basic git functionality by creating repositories, write some docs/code and push the code.

**<span style="text-decoration:underline;">Content</span>**



* Create a github account 
    * [Join GitHub · GitHub](https://github.com/join)
* Install and Setup Git
    * Windows Git Bash: 
        *  [How To Install Git Bash On Windows](https://www.stanleyulili.com/git/how-to-install-git-bash-on-windows/)
    * Linux:
        * WIP(Work in Progress)
    * Mac OS
        * WIP
    * Configuring git on your machines.
        * [Your first time with git and github](https://kbroman.org/github_tutorial/pages/first_time.html)
        * [Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
        * SSH Config
            * [How to Get and Configure Your Git and GitHub SSH Keys](https://www.freecodecamp.org/news/git-ssh-how-to/)
            * [Connecting to GitHub with SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)
    * What is VC(Version Control, git vs Github)
        * [Version Control – Programming Fundamentals](https://press.rebus.community/programmingfundamentals/chapter/version-control/)
        * [What is version control](https://www.atlassian.com/git/tutorials/what-is-version-control)
        * [Git vs. GitHub: What's the Difference?](https://blog.devmountain.com/git-vs-github-whats-the-difference/)
        * [An Intro to Git and GitHub for Beginners (Tutorial)](https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners)
* Git branching
    * [Git - Branches in a Nutshell](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell)	
    * [Learn Git Branching](https://learngitbranching.js.org/)
    * [Git Branch](https://www.atlassian.com/git/tutorials/using-branches)
* General Git Beginner Usage
    * [A step-by-step guide to Git](https://opensource.com/article/18/1/step-step-guide-git)
    * [git - the simple guide - no deep shit!](https://rogerdudler.github.io/git-guide/)
    * [An introduction to Git: what it is, and how to use it](https://www.freecodecamp.org/news/what-is-git-and-how-to-use-it-c341b049ae61/)
    * [Git and GitHub Tutorial for Beginners](https://www.analyticsvidhya.com/blog/2021/09/git-and-github-tutorial-for-beginners/)
    * [The beginner's guide to Git & GitHub](https://www.freecodecamp.org/news/the-beginners-guide-to-git-github/)
    * [An Intro to Git and GitHub for Beginners (Tutorial)](https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners)
    * README
        * [README File | What is README & Why is a README File Necessary?](https://www.mygreatlearning.com/blog/readme-file/)
        * [How to write a good README for your GitHub project?](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)
    * Commit Messages
        * [How to Write Good Commit Messages: A Practical Git Guide](https://www.freecodecamp.org/news/writing-good-commit-messages-a-practical-guide/)


## Understanding the Command Line

When writing code, we mostly move between and editor and the terminal/console/command line(The balck screen you see in most movies). An editor is just like Microsoft Word but has special abilities to handle code. It makes it easier to write code. Think of it like instead of creating tables in Microsoft Word, you use Excel because it has more functionalities to deal with tables.

The command line is where the magic happens. This is where we type commands to run code or just do some common tasks like creating a folder, changing into a folder. Normally we do this by right clicking in our computers and choosing something but it's really slow compared to typing a single command on the terminal. Here's a sample terminal with command. The ones in green are the commands.

ls - list the contents of the folder

mkdir - make a new directory/folder

touch - create a new file

cd - change into a certain directory

Commands are case sensitive, i.e ls is not the same as LS. These commands also take options and you'll learn more as you go by.

**Windows default terminal is called Command Prompt an d is not very good when coding, so install a new command line called [Git Bash](https://www.atlassian.com/git/tutorials/git-bash).**



<p id="gdcalert2" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image2.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert3">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image2.png "image_tooltip")


**<span style="text-decoration:underline;">Objectives</span>**



* Understand what the command line is.
* Know how to use basic commands
* Get accustomed to working between the editor and the command line. 

**NOTE:** With the latest version of Windows, the command line(console or terminal) is getting better and I would recommend using Gitbash if on Windows to get a Unix-like Experience on the commandline. Avoid Command Prompt(Windows Shell) as much as possible to avoid lots of programming issues.



* [Command line crash course - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Understanding_client-side_tools/Command_line)
* [What Is Command Line Interface (CLI)? Command Line for Beginners - Learn to Code With Me](https://learntocodewith.me/learn/command-line/)
* [The Linux command line for beginners | Ubuntu](https://ubuntu.com/tutorials/command-line-for-beginners#1-overview)


## Python


### Code Editors

This section shows you the different editors you can use. VS Code is the leading in the industry. You'll need to know some vim when working with git but for now, VS Code is enough. Install it an and get going.

I recommend VS Code.



* [VS code](https://code.visualstudio.com/) (Recommended)
    * [Get Started Tutorial for Python in Visual Studio Code](https://code.visualstudio.com/docs/python/python-tutorial)
* Sublime Text
* Atom
* VIM

    Learn a little bit of Vim to use in the command line

    * [https://danielmiessler.com/study/vim/](https://danielmiessler.com/study/vim/)


### Setup

This section should guide you through setting up the coding environment. By the coding environment I mean, you install Python and anything else that is needed to run python code.

At the end of this section, you should be able to write a simple python code and run it on the terminal and see the results.



* Windows:
    * [https://realpython.com/installing-python/#how-to-install-python-on-windows](https://realpython.com/installing-python/#how-to-install-python-on-windows)
    * [https://code.visualstudio.com/docs/python/python-tutorial](https://code.visualstudio.com/docs/python/python-tutorial)


### Coding Environment



* [[Python] Beginner must know, virtualEnv | by Peter Chang](https://blog.cloudboost.io/python-beginner-must-know-virtualenv-tutorial-example-5e3f82cfbd8b)
* [Virtual environments for absolute beginners — what is it and how to create one (+ examples)](https://towardsdatascience.com/virtual-environments-for-absolute-beginners-what-is-it-and-how-to-create-one-examples-a48da8982d4b)
* [Virtual Environments explained by a Python beginner. | by Monica P.](https://medium.com/@monipip3/virtual-environments-explained-by-a-python-beginner-693a79b195da)
* [How to build a Python virtual environment for Beginners](https://morioh.com/p/91aa60968585)
* [Creating a Python Virtual Environment for Beginners](https://www.ordinarycoders.com/blog/article/python-virtual-environment)
* Virtual Environment: [Python Virtual Environments: A Primer – Real Python](https://realpython.com/python-virtual-environments-a-primer/)
* [Pipenv: A Guide to the New Python Packaging Tool – Real Python](https://realpython.com/pipenv-guide/)
* [Your First Guide to Getting Started with “pipenv”](https://dev.to/yukinagae/your-first-guide-to-getting-started-with-pipenv-50bn)


### Coding conventions and Style Guides

These just define some of the conventions followed while writing code. These vary between different languages but in this case we'll be focusing on python.



* [Clean Code Syntax for Python: Introduction to PEP 8 Style Guide](https://www.earthdatascience.org/courses/intro-to-earth-data-science/write-efficient-python-code/intro-to-clean-code/python-pep-8-style-guide/)
* [Python Code Quality: Tools & Best Practices](https://realpython.com/python-code-quality/)


### Python Tutorials

**<span style="text-decoration:underline;">Objectives</span>**



* Understand the different programming concepts and apply them when writing code using python. At the end of any one of these tutorials, you should be able to write some reasonable code and display the knowledge of: 
    * Python syntax
    * Variables
    * Functions
    * Modules and packages
    * Control structures(if, for etc)
    * Data structures(tuples, lists/arrays, dictionaries etc)
    * OOP(object oriented programming using classes)

        

<p id="gdcalert3" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image3.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert4">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image3.png "image_tooltip")



        The above are the contents of[ the first link below.](https://www.programiz.com/python-programming)

* General Tuts
    * [Learn Python Programming](https://www.programiz.com/python-programming)(Recommended)
    * [Python Tutorial](https://www.w3schools.com/python/)
    * [How to Get Started With Python?](https://www.programiz.com/python-programming/first-program)
    * [How To Code in Python](https://www.digitalocean.com/community/tutorial_series/how-to-code-in-python-3)
* [Python Tutorial for Beginners: Learn Programming Basics [PDF]](https://www.guru99.com/python-tutorials.html)
* Python Repl(Interactive Shell)
* [REPL - Python Interactive Shell](https://pythonprogramminglanguage.com/repl/)
* [REPL - Python Interactive Shell - Python](https://pythonprogramminglanguage.com/repl/)
* [REPL](https://docs.pycom.io/docnotes/repl/#:~:text=REPL%20stands%20for%20Read%20Evaluate,writing%20scripts%20in%20main.py%20).
* [Using The REPL](https://www.learnpython.dev/01-introduction/02-requirements/05-vs-code/04-the-repl-in-vscode/)
* [Code with Repl.it | Python projects for beginners](https://www.codewithrepl.it/)
* [The Python REPL](https://python.land/introduction-to-python/the-repl)
* [2. Using the Python Interpreter — Python 3.10.1 documentation](https://docs.python.org/3/tutorial/interpreter.html)
* Functions and Modules
    * [Python Functions (def): Definition with Examples](https://www.programiz.com/python-programming/function)
    * [Introducing Functions](http://introtopython.org/introducing_functions.html)
    * [Python Functions](https://www.w3schools.com/python/python_functions.asp)
    * [Python Functions: How to Call & Write Functions - DataCamp](https://www.datacamp.com/community/tutorials/functions-python-tutorial)
    * [Functions 101 – Introduction to Functions in Python For Absolute Begineers](https://www.analyticsvidhya.com/blog/2021/05/functions-101-introduction-to-functions-in-python-for-absolute-begineers/)
    * [Modules and Packages - Learn Python - Free Interactive Python Tutorial](https://www.learnpython.org/en/Modules_and_Packages)
    * [Introduction to Python Modules - AskPython](https://www.askpython.com/python-modules/python-modules)
    * [Python Modules and Packages – An Introduction](https://realpython.com/python-modules-packages/)
    * [Python Modules](https://www.w3schools.com/python/python_modules.asp)
    * [Working with Modules in Python: Must Known Fundamentals for Data Scientists](https://www.analyticsvidhya.com/blog/2021/07/working-with-modules-in-python-must-known-fundamentals-for-data-scientists/)
    * [Python Modules: Learn to Create and Import Custom and Built-in Modules](https://www.programiz.com/python-programming/modules)
* Python Classes(OOP - Object oriented programming)
    * [Python Object Oriented Programming](https://www.programiz.com/python-programming/object-oriented-programming)
    * [A GENTLE INTRODUCTION TO PYTHON CLASSES FOR NEWBIES - DEV Community](https://dev.to/oluchi/a-gentle-introduction-to-python-classes-for-newbies-p46)
    * [Introduction to Python Classes. A comprehensive practical guide in the… | by Soner Yıldırım | Towards Data Science](https://towardsdatascience.com/introduction-to-python-classes-da526ff745df)
    * [Introduction to classes in Python](http://hplgit.github.io/primer.html/doc/pub/class/class-readable.html)
    * [Introduction to Classes | Codecademy](https://www.codecademy.com/learn/learn-python/modules/learn-python-introduction-to-classes-u)
    * [Object-Oriented Programming (OOP) in Python 3](https://realpython.com/python3-object-oriented-programming/)
* Jupyter Notebook

    Optional section, you can come back here later.

    * [How to Use Jupyter Notebook in 2020: A Beginner's Tutorial](https://www.dataquest.io/blog/jupyter-notebook-tutorial/)
    * [Jupyter Notebook: An Introduction – Real Python](https://realpython.com/jupyter-notebook-introduction/)
    * https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/what_is_jupyter.html#notebook-document


## Web

Now here's where we start applying the knowledge we've been learning. This is where you learn the basics of how websites actually work.

**<span style="text-decoration:underline;">Objectives:</span>**



* Understand what an API is
* Be able to create a simple API using fast API and Flask
* Understand what REST is
* Understand the different HTTP verbs used in APIs
* Understand how to call our API using cURL and Postman
* APIs
* [Absolute beginners guide to slaying APIs using Python](https://medium.com/quick-code/absolute-beginners-guide-to-slaying-apis-using-python-7b380dc82236)
* [Introduction to APIs in Python](https://towardsdatascience.com/quick-fire-guide-to-apis-in-python-891dd98c8877)
* Postman:
    * [Postman Tutorial: How to Install and use Postman for API Testing](https://www.guru99.com/postman-tutorial.html)
    * [Introduction | Postman Learning Center](https://learning.postman.com/docs/getting-started/introduction/)
    * [Postman Tutorial for Beginners to perform API Testing](https://www.toolsqa.com/postman/postman-tutorial/)
* [Python & APIs: A Winning Combo for Reading Public Data – Real Python](https://realpython.com/python-api/)
* [Python API Tutorial: Getting Started with APIs](https://www.dataquest.io/blog/python-api-tutorial/)
* [How to Build a REST API with Python](https://towardsdatascience.com/the-right-way-to-build-an-api-with-python-cd08ab285f8f)
* [Building a Basic RestFul API in Python](https://www.codementor.io/@sagaragarwal94/building-a-basic-restful-api-in-python-58k02xsiq)
* Flask
    * [Creating Web APIs with Python and Flask](https://programminghistorian.org/en/lessons/creating-apis-with-python-and-flask)
    * [Test Driven Development (TDD) with Python](https://rubikscode.net/2021/05/24/test-driven-development-tdd-with-python/)
    * [How to create a simple REST API with Python and Flask in 5 minutes](https://medium.com/duomly-blockchain-online-courses/how-to-create-a-simple-rest-api-with-python-and-flask-in-5-minutes-94bb88f74a23)
* Fast API
    * [The Ultimate FastAPI Tutorial Part 1 - Basic API Endpoints](https://christophergs.com/tutorials/ultimate-fastapi-tutorial-pt-1-hello-world/)
    * [First Steps - FastAPI](https://fastapi.tiangolo.com/tutorial/first-steps/)
    * [Tutorial - User Guide - Intro - FastAPI](https://fastapi.tiangolo.com/tutorial/)
    * [Using FastAPI to Build Python Web APIs – Real Python](https://realpython.com/fastapi-python-web-apis/)


## Databases

Here, we apply more of the concepts we learnt before. Things should now be getting together. We see websites and they're different. Some are just pages(we call them web pages) whose data does not change and they show the same thing over and over. But most websites are more than that. They fetch data via APIs, these APIs talk to databases that are the main data stores. Here we'll learn a new language(a query language) called SQL. This is used to talk to databases.

**<span style="text-decoration:underline;">Objectives</span>**



* Understand databases and database concepts
* Setup a basic database, create tables and add fields and some data.
* Be able to write basic queries to select, insert, delete and update. Implementing [CRUD](https://developer.mozilla.org/en-US/docs/Glossary/CRUD) functionality.
* Understand relational(SQL) vs non-relational(NoSQL) databases.
* Access the databases in your API
* Fetch the data from the databases via the API

**<span style="text-decoration:underline;">Content</span>** 



* [Database Basics: Concepts & Examples for Beginners](https://www.lido.app/post/database-101)
* [An Introduction to Databases for Beginners](https://www.lifewire.com/databases-for-beginners-1019643)
* [https://wiredelta.com/databases-for-beginners/](https://wiredelta.com/databases-for-beginners/)
* [Database for Beginners(Part 1) | What is Database](https://www.analyticsvidhya.com/blog/2021/07/a-beginners-guide-to-database-part-1/)
* SQLite
    * [Introduction to SQLite in Python](https://www.pythoncentral.io/introduction-to-sqlite-in-python/)
    * [How To Use the sqlite3 Module in Python 3](https://www.digitalocean.com/community/tutorials/how-to-use-the-sqlite3-module-in-python-3)
    * [Introduction to SQLite in Python – Pythonista Planet](https://pythonistaplanet.com/sqlite-in-python/)
    * [Beginner's Guide to Using Databases with Python: Postgres, SQLAlchemy, and Alembic](https://www.learndatasci.com/tutorials/using-databases-python-postgres-sqlalchemy-and-alembic/)
* Install Postgres
    * Windows: [Install PostgreSQL on Windows](https://www.postgresqltutorial.com/install-postgresql/)
    * Linux:
    * Mac OS:
    * Tutorials:
        * [https://pynative.com/python-postgresql-tutorial/](https://pynative.com/python-postgresql-tutorial/)
        * Series
            * [PostgreSQL Python Tutorial With Practical Examples](https://www.postgresqltutorial.com/postgresql-python/)
            * [PostgreSQL Python: Connect To PostgreSQL Database Server](https://www.postgresqltutorial.com/postgresql-python/connect/)
            * [PostgreSQL Python: Create Tables](https://www.postgresqltutorial.com/postgresql-python/create-tables/)
            * [PostgresQL Python: Insert Data Into a Table](https://www.postgresqltutorial.com/postgresql-python/insert/)
            * [PostgreSQL Python: Update Data in a PostgreSQL Table](https://www.postgresqltutorial.com/postgresql-python/update/)
            * [PostgreSQL Python: Handling Transaction in Psycopg](https://www.postgresqltutorial.com/postgresql-python/transaction/)
            * [PostgreSQL Python: Call PostgreSQL Functions](https://www.postgresqltutorial.com/postgresql-python/postgresql-python-call-postgresql-functions/)
* Install MongoDB
    * Windows(Any of the below will work, just choose one)
        * [How to Download & Install MongoDB on Windows](https://medium.com/@LondonAppBrewery/how-to-download-install-mongodb-on-windows-4ee4b3493514)
        * [How to Download & Install MongoDB on Windows and Cloud](https://www.guru99.com/installation-configuration-mongodb.html)
        * [Install MongoDB Community Edition on Windows — MongoDB Manual](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-windows/)
    * MongoDB Python Tutorials
        * [Python and MongoDB: Connecting to NoSQL Databases – Real Python](https://realpython.com/introduction-to-mongodb-and-python/)
* [Getting Started with Python and MongoDB](https://www.mongodb.com/blog/post/getting-started-with-python-and-mongodb)
* [Python MongoDB](https://www.w3schools.com/python/python_mongodb_getstarted.asp)
* [What is MongoDB | MongoDB Tutorial | MongoDB In Python](https://www.analyticsvidhya.com/blog/2020/02/mongodb-in-python-tutorial-for-beginners-using-pymongo/)
* [A guide on how to interact between Python and databases using SQLAlchemy and PostgreSQL](https://towardsdatascience.com/a-guide-on-how-to-interact-between-python-and-databases-using-sqlalchemy-and-postgresql-a6d770723474)
* [Using PostgreSQL through SQLAlchemy](https://www.compose.com/articles/using-postgresql-through-sqlalchemy/)


#### Database migrations with Alembic:



* [Schema migrations with Alembic, Python and PostgreSQL](https://www.compose.com/articles/schema-migrations-with-alembic-python-and-postgresql/)
* [Flask-Migrate — Flask-Migrate documentation](https://flask-migrate.readthedocs.io/en/latest/)


## Testing

This is a more advanced topic but very important. The goal of testing is to ensure that your code does what is actually supposed to do. 



* [A simple introduction to Test Driven Development with Python](https://www.freecodecamp.org/news/learning-to-test-with-python-997ace2d8abe/)
* [Get started with Test Driven Development in Python](https://medium.com/nerd-for-tech/get-started-with-test-driven-development-in-python-88686b11cbe1)
* [Test-Driven Development With PyTest – Real Python](https://realpython.com/courses/test-driven-development-pytest/)
* [Beginning Test-Driven Development in Python](https://code.tutsplus.com/tutorials/beginning-test-driven-development-in-python--net-30137)


## Debugging

As you write code, you always run into issues like the code giving the wrong result dues to some mistakes. These are bugs and finding bugs is a skill every developer should possess.



* [Working with pdb to Debug Python Code](https://www.digitalocean.com/community/tutorials/how-to-use-the-python-debugger)


## Full Python Application Tutorials

At this point, you should be ready to write a fully functional application from beginning to end.



* [Flask by Example – Setting up Postgres, SQLAlchemy, and Alembic – Real Python](https://realpython.com/flask-by-example-part-2-postgres-sqlalchemy-and-alembic/)
* [Using SQLAlchemy with Flask and PostgreSQL](https://stackabuse.com/using-sqlalchemy-with-flask-and-postgresql/)


## Django(The big framework)



* [Introduction | Django For Beginners](https://djangoforbeginners.com/introduction/)
* [A Complete Beginner's Guide to Django](https://simpleisbetterthancomplex.com/series/beginners-guide/1.11/)


## Introduction to Front End Web Programming

Now that we know how to write code, create APIs, use databases, how do we display the data on a website in readable form? How do we add the different styles and colors etc. How do we make the system accessible and usable but common users?



* [Part 1: Your First Website | HTML & CSS Tutorial](https://code.makery.ch/library/html-css/part1/)
* [Learn HTML Basics for Beginners in Just 15 Minutes](https://www.freecodecamp.org/news/html-basics-for-beginners/)
* HTML Tutorial
    * [https://html.com/](https://html.com/)
    * [HTML Tutorial](https://www.w3schools.com/html/default.asp)
* CSS Tutorial
    * [Learn CSS in 5 minutes - A tutorial for beginners](https://www.freecodecamp.org/news/get-started-with-css-in-5-minutes-e0804813fc3e/)
    * [CSS Tutorial](https://www.w3schools.com/css/default.asp)
* JavaScript Tutorial
    * [JavaScript Tutorial for Beginners: Learn Javascript Step by Step](https://www.guru99.com/interactive-javascript-tutorials.html)
    * [JavaScript Tutorial](https://www.w3schools.com/js/default.asp)
* React
    * [React for Beginners – A React.js Handbook for Front End Developers](https://www.freecodecamp.org/news/react-beginner-handbook/)
    * [Tutorial: Intro to React – React](https://reactjs.org/tutorial/tutorial.html)
* [Getting Started with Visual Studio Code and Building HTML Websites](https://www.codecademy.com/articles/visual-studio-code)
* [https://www.better.dev/courses/getting-started-with-javascript](https://www.better.dev/courses/getting-started-with-javascript)


## Authentication and Authorization

How do we control who accesses the system, what they can see etc

What's the difference between authentication and authorization?
