What is this project about
====
The purpose of this Symfony project is simply to have a bunch of php files that simulate a website.
This website is destined to be injected into a Docker image containing an apache web server.

How is it done
===
The pipeline we are going to pursuit is the following:
1. Create code (i.e. this project) located on a git server (i.e. here on GitHub)
2. On commit/push to git server trigger a build job on a build server (i.e. JenkinsCI)
3. On "Pass all tests" on the build server, inject code into a docker image
4. Deploy docker image onto a "docker server"
5. Rejoice and drink beer