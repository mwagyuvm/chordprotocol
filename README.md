
# Implementation of the Chord peer-to-peer computing protocol

## BUILD

The build system used is Maven, so you need to have 
Maven installed on your system
(http://maven.apache.org/download.html)

To build, just type "mvn package" at the root directory
of the project that contains the POM (pom.xml file).

This will create the Client, SuperNode and Node jars
needed for the peer-to-peer system. The jars contain 
all needed dependencies, so they are ready to run
"out-of-the-box" using the "java" executable:
>> java -jar <insert.jar.file.here>

Before starting the system, be sure that the Java RMI
Registry is running, otherwise the Java RMI will not be
able to identify where the remote objects exist 
(and connection errors will be seen). To start the 
RMI Registry, type the following in a shell window:

>> rmiregistry

We are assuming in the system that the registry is
running on the default port (1099).

------------------------------------------------------
