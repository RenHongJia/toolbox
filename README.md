# AMIDST Toolbox
====

Analysis of data streams using expressive and flexible Bayesian networks

This is the repository for the open source code in the AMIDST project.

Install Java 8 and IntelliJ:

http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

http://www.jetbrains.com/idea/download/

In IntelliJ open the maven project by pointint at the pom file. Also you need to point to the Java 8 installation and you are ready to rock.

========================
Compiling & Running from the command line
========================

1- Install Maven: http://maven.apache.org/download.cgi
(Download binaries and copy to Applications folder)

2- Modify the file maven_startup.sh (which you can find in the root project folder) and fix the path of your maven (Line 5) and java installation (Line 9).

3- Create (or modify if already exists) a file ".profile" or ".bash_profile" in you home directory and add the following line,
which points to file "maven_startup.sh"

        source <project-folder>/maven_startup.sh

 Now after restarting the terminal, mvn should work.


4- The script "compile.sh" (which you can find in the root project folder) just compiles the whole project.


5- The script "run.sh" (which you can find in the root project folder) should be used to run some class. For example,

        ./run.sh eu.amidst.core.examples.learning.ParallelMaximumLikelihoodExample