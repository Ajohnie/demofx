## JAVAFX APPLICATION TEMPLATE
- This is an example of a javafx modular application

![mage](https://github.com/Ajohnie/demofx/blob/master/git-hub-description.PNG)

Installing
----------
- We are using Liberica JDK because it comes bundled with JAVAFX
- [Download Liberica 17 JDK](https://bell-sw.com/pages/liberica-native-image-kit/) 
  - Add environmental variables for the JDK, (there are many resources online for how to do this)
  - set JAVA_HOME=C:\Program Files\BellSoft\LibericaNIK-Full-21-OpenJDK-17 or the directory where you installed the Liberica JDK
  - set JAVA_PATH=%JAVA_HOME%\bin
  - Add %JAVA_HOME% to the global %PATH% variable so that it is accessible globally from the command line
- [Download The Latest Version of Maven](https://maven.apache.org/download.cgi)
  - set MAVEN_HOME=C:\Program Files\maven or wherever you installed your maven binaries
  - Add %MAVEN_PATH% to the global %PATH% variable so that it is accessible globally from the command line
  - Restart Your Computer so that the above changes take effect
  - git clone http://github.com/Ajohnie/demofx
  - type cd demofx
  - run mvn install
  
Building An Executable App
----------
- Replace the paths in the batch files with paths from your own file system i.e where the project is located
- Rub pack.bat to create jar file for your app
- Run link.bat(look at this file for more details) with OPTION 1 to know module dependencies
- Run link.bat(look at this file for more details) with OPTION 2 to create a custom runtime image
- execute run-jar.bat and make sure the app runs before packaging it
- Run image.bat(look at this file for more details) to create an executable file for your app
- 
- All the steps above can be customized to create executable files for other operating systems
- I used batch files to do some tasks that can be done using maven or your favourite build tool since I was rusty on maven
- Feel free to use what works for you
- I left some useful comments allover the files for some errors I got while doing this and how I dealt with them
- I have included run configurations under .idea directory I used for IntelliJ IDE, the .idea directory is sometimes hidden so un hide it if you can't see it

Useful Links
----------
- The initial skeleton app was built with maven archetypes obtained from here [FXML based JavaFX Maven Archetype](https://github.com/openjfx/javafx-maven-archetypes/tree/master/javafx-archetype-fxml)
- [A real world use case of this template](https://github.com/Ajohnie/nfc-card-reader)


TODO
----------
- Replace the actions performed by the batch scripts with maven equivalents
- Good Luck
