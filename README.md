#Travis CI  

This is a document that supposes to capture the basics of Travis CI.
I am learning it while writing this document.

Also please keep in mind that all the information here are based on
Travis CI documentation which could be found @[Travis CI](https://docs.travis-ci.com/)


###So what is continuous integration?

CI means to merge small code changes frequently - rather than merging in a large change at
the end of a development life cycle.

###How does Travis CI help?

It's a platform that supports your development process by automatically building and testing code
changes. It immediately notifies you of the success of the change. Travis also can automate other parts
of your development process by managing deployments and notifications.


###How does builds work? 

When you run a build, Travis CI clones your GitHub repository into a brand new virtual environment and carries out a series of tasks to build and test your code. If one or more of those tasks fails,
the build is considered broken. If none of the tasks fail, the build is considered passed, and
Travis CI can deploy your code to a web server, or application host.

##Important key words

###job:
An automated process that clones your repository into a virtual environment and then carries out a series of phases such as compiling your code, running tests, etc. A job fails if the
return code of the <script> phase is non zero.

###phase:
The sequential steps of a job. For example, the install phase comes before the script phase,
which comes before the optional deploy phase.

###build:
A group of jobs. For example, a build might have two jobs, each of which tests a project with a different version of a programming language. A build finishes when all of its jobs are finished.

###stage:
A group of jobs that run in parallel as part of a sequential build process
composed of multiple stages.


###Trouble shooting
If you have problems with broken builds, check out @[Travis CI documentation](https://docs.travis-ci.com/user/common-build-problems/)


##Getting started

check out the [prerequisites](https://docs.travis-ci.com/user/getting-started/) here

```
Add a .tarvis.yml file to your git repo, then commit and push, to trigger Travis's build
```


> We will be looking into how to customize your build shortly. I will probably give 2 examples one using Node.js and another using Java



#More than running tests

Travis enables you to do more than running tests.


>we will look into how to configure Travis to send notifications shortly
