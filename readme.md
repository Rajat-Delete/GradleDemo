## Setup of Basic Gradle Using CLI

``
gradle init --use-defaults --type java-application
``

The Above command will setup a basic gradle project


``
./gradlew build
``
The Above command will build the gradle project

``
jar{
manifest {
attributes(
'Main-Class' : 'org.example.Main'
)
}
}
``

To prepare a jar which is executable , you need to setup manifest property in build.gradle to identify from which Main class to execute the code.
The Above code can build your project.

``
./gradlew jar
``
The above command creates  new jar file in build/libs folder

``
java -jar build/jars/filename.jar 
``
The Above command will execute the main jar which is generated from build.