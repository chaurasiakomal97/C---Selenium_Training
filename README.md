Stage 1 – C# Programming language

Stage 2 – Web Automation (Selenium), Windows automation (FLAUI), API Automation (RestSharp)

Stage 3 – Framework 1 – Hybrid Framework (Nunit, Data Driven Framework, Keyword Driven Framework, Page Object Model)

Stage 4 – BDD Framework

Stage 5 – CI CD Pipeline



Selenium - https://www.selenium.dev/

· Open Source

· Automates only web applications

· Language Independency – Java, C#, Python, Javascript, Ruby

Selenium – A suite of tools

1. Selenium IDE

a. No need of programming knowledge

b. Record and playback features

c. Plugin – chrome, firefox, edge

d. Use it only for simple scripting or exploratory testing

2. Selenium RC – Depreciated

a. Programming knowledge is required

b. Architecture

Source code (C#+Selenium RC lib) à RC Server (Turn ON/OFF) à Browser

3. Selenium WebDriver

a. Programming knowledge is required

b. Architecture

Source code (C#+Selenium WebDriver lib) à Browser

4. Selenium Grid

a. If you want to scale by distributing and running tests on several machines and manage multiple environments from a central point.

Selenium IDE – Overview

1. Install the plugin

2. Simple record and playback

3. Verify vs Assert

a. Soft Assertion (Verify) - The test will continue even if the verify fails.

b. Hard Assertion (Assert) - The test will stop if the assert fails.

C# Programming knowledge

1. Install Visual studio IDE (community)

2. Architecture of C#

a. Console App Project

Source code (.csproj) à .dll/.exe à O/P

.dll à platform independent code means you can move to any platform provided CLR is present in that machine to execute it.

Compile time (Source code (.csproj) à .dll/.exe)

Runtime (.dll/.exe à O/P)

b. Class lib or Unit test project

Source code (.csproj) à .dll à O/P

3. UpperCamelCase – MyFirstProject

lowerCamelCase – myFirstProject

4. Structure of C# programming

Solution Folder - UpperCamelCase

Project 1 Folder – UpperCamelCase

Namespace– UpperCamelCase

Class 1 file (.cs) – UpperCamelCase

Methods – UpperCamelCase

Variables - lowerCamelCase

Class 2 file (.cs)

Project 2 Folder

Class file (.cs)

5. Create a console app

6. Datatypes

a. Pre-defined datatypes

b. Non-predefined datatypes – collection of pre-defined datatypes

i. String

ii. Array

iii. User defined datatypes

7. Methods – building block of the program

a. Reusability

b. Maintenance

Methods:

· Static Methods – How to create and call it?

//accessmodifier static returntype methodname(arguments)

How to call the static method?

Classname.MethodName()

· Non-static methods – How to create and call it?

How to call the non-static method?

o Create object for that class

o Use objref.methodname()

8. Object

a. Declaration

b. Instantiation

c. Initialization

9. Class – A class is template or blueprint or type from which objects are created.

10. Object

a. An object is an instance of class

b. An object contains its own state (non-static variable) and behaviour (non-static methods)

11. Access Modifier

a. Private – accessible within the class

b. Internal – accessible within the assembly (project)

c. Protected

d. Protected internal

e. Public - accessible anywhere

12. Debugging

a. Step into

b. Step over

c. Terminate

d. Continue

13. this keyword à

a. helps to distinguish between instance and local variable

b. basically, this keyword points to current object.

14. Constructor – anything pre-requisite for object

a. Constructor name and class name should be same. It is kind of method without any return type which will be called on every object creation

b. There will be always a default constructor which helps to load all non-static variable with default values.

c. We can override the constructor by creating our own constructor

i. With parameter

ii. Without parameter

d. If there are any explicitly created constructor, then you must call it during object creation.

Selenium WebDriver

1. Create a console app

2. Add libraries from nuget package manager

a. Selenium.WebDriver (WebDriver.dll)

b. Selenium.Support(WebDriver.Support.dll)

3. Click, type, Select

4. Inspect à tagname, attribute, text or not

5. To inspect à f12 or ctrl+shift+c

6. Basic locators

a. Id

b. Name

c. Classname

d. Tagname e. Linktext

f. Partial link text

When there are duplicate locator then FindElement picks the first webelement

7. Advance locators

a. XPath

b. CSS

8. Synchronization

a. Unconditional wait (from C# lib)

i. Thread.sleep(ms) à not recommended

b. Conditional wait (from selenium lib)

i. Implicit wait

1. Default implicit wait – 0s

2. Applicable for all FindElement and FindElements method only

3. Example: Implicit wait – 30s

a. If element is not present, it will check for 30s and then throw exception

b. If element is present, it will proceed with the operation immediately

c. Polling time – 0.5s (how freq it checks)

ii. Explicit wait

iii. Fluent wait
