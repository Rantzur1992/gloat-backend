# Gloat Matcher Assigment

This is the Gloat Assigment, the tool is a CLI for getting the best matches of the JSON Database which is included.

## Installation

To install run
```
pip install gloat-matcher
```

To see options and examples, run
```
matcher --help

Usage: matcher [OPTIONS]

  Returns the best matches for the provided Job

Options:
  -t, --title TEXT   The job title  [required]
  -s, --skills TEXT  Optional Skills for the job, you can add multiple skills
                     by using -s/-skill

  -h, --help         Show this message and exit.
 ````
 
 ## Examples
 Match all Automation Engineers
 ```
matcher -t automation

------------------
Candidate
------------------
Name: Dor
Title: Automation Engineer
Skills:
   - Selenium
   - TestNG
   - Java
------------------
Candidate
------------------
Name: David
Title: Automation Engineer
Skills:
   - Selenium
   - Specflow
   - C#
   - BDD
   - xUnit
------------------
Candidate
------------------
Name: Guy
Title: Automation Engineer
Skills:
   - Selenium
   - Specflow
   - C#
   - BDD
   - xUnit
   - Nunit
   - MsTest
```

Match all Software Engineers who posses the Java skill

```
matcher -t "software engineer" -s Java

------------------
Candidate
------------------
Name: Ran
Title: Software Engineer
Skills:
   - Java
   - Python
   - C#
   - Jenkins
   - API Testing
   - Microservices
   - Backend
   - Good Looking
   - Algorithms
   - Docker
   - Machine Learning
```

>You can add additional skills to the query by adding additional -s/--skill parameters.
