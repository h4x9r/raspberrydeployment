# raspberrydeployment


Example Java application for remote upload and debugging 


## Usage
The usage is shown using the Intellij IDE

0. The raspberryDeployment server must be announced in settigns.xml
<code>
<servers>
  <server>
  <id>raspberryDeployment</id>
  <username>user</username>
  <password>secret</password>
  </server>
</servers>
	</code>
1. In the pom.xml under the properties tag the corresponding data concerning server and target directory must be adapted
2. After that in the Intellij the remote server has to be announced under the Debug option

	a. To do this you go to the top link edit configuration
	
	b. Then click on the plus symbol and select Remote
	
	c. In the settings then enter the appropriate host address and port. As transport socket is chosen.
	
3. Now mvn clean install uploads the artifact to the remote machine and starts a debug session
4. In intellij now you only have to click on the debug symbol
