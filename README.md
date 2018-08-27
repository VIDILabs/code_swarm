# code_swarm: A Design Study in Organic Software Visualization
If you have used the code_swarm, please cite the follwing paper:
```bibtex
@article{Ogawa09CodeSwarm, 
    author={Michael Ogawa and Kwan-Liu Ma}, 
    title={code_swarm: A Design Study in Organic Software Visualization}, 
    journal={IEEE Transactions on Visualization and Computer Graphics}, 
    year={2009}, 
    volume={15}, 
    number={6}, 
    pages={1097-1104}, 
}
```

## Original README
```
code_swarm is an experiment in organic software visualization.

See http://vis.cs.ucdavis.edu/~ogawa/codeswarm for a picture of what we want
to produce.

Google Code Project :      http://code.google.com/p/codeswarm/
Google Group/Mailing List: http://groups.google.com/group/codeswarm 


I) How to build Java code_swarm in different environments.

Please visit http://code.google.com/p/codeswarm/w/list for more detailed and
up-to-date information.

This quick guide explains how to setup your development environment to build
the binary (ie. jar) version of code_swarm from Java sources.
Explanations require at least an understanding of computing and of your
Operating System, even if no Java skills are needed.

I.1) Setup
You will need the "Ant" software building tool, and the Java SDK from sun
(no idea if other SDK could do the job).

I.1.a) Linux
This guide is written with a Debian based Linux, Ubuntu 8.04. It would requires
some minor adaptation to use on other distribution (other packaging systems).

 * install ant with the following command (or with your favorite graphical package manager) 
    sudo apt-get install ant 

 * install sun-java-jdk 1.5 or 1.6 following your distribution recommendation 
    sudo apt-get install sun-java6-jdk 

 * configure the Java SDK to specify the new installation path, for instance on Ubuntu : 
    sudo update-java-alternatives -s java-6-sun 

   See http://doc.ubuntu-fr.org/java

I.1.b) Windows
 * download ant for all platforms at http://ant.apache.org/bindownload.cgi
 * unpack it where you want it to be installed, and add the location of
   its binaries to the the "PATH" environment variable. For instance, add at the end : 
   "C:\apache-ant-1.7.0\bin;" 

 * download Sun Java SDK at http://java.sun.com/javase/downloads/index.jsp
 * install it and add the "javac" Java compiler to the PATH : 
   "C:\Program Files\Java\jdk1.6.0_06\bin;" 

 * then create a new environment variable called JAVA_HOME and set its paht to 
   "C:\Program Files\Java\jdk1.6.0_06;" 

I.2) Getting the sources

code_swarm sources are under a Google Code Subversion repository (svn) :
http://codeswarm.googlecode.com/svn/trunk/

See Subversion homepage on tigris for all appropriate tools and documents.
I would recommend "TortoiseSVN" for Windows users. Unix-like users would get
their native "Subversion" package.

See the "Source" tab on Google Code Project for further instruction on
where to browse and checkout the sources.

I.3) Building the sources

Quick build :
 * Open a terminal/a command line shell, change directory to the root of
   the code_swarm source folder, and to launch the build, type 
   ant 

 * Then to launch code_swarm use 
   ant run Notice that you can type only the second command to do both in once 

Alternatively, you can just try the "run.sh" or "run.bat" scripts to get it
done in once, but need to rebuild manually typing "ant" if you modify sources

Other commands :
 * "ant all" will also generate the Javadoc HTML sources documentation
 * "ant clean" will delete all intermediate and binary files 
```