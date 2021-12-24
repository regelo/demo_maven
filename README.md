# demo_maven
Démonstration d'Apache Maven en Java et de l'utilisation du moteur 3D jMonkeyEngine

La commande initiale pour créer le projet avec Maven est : 

    	mvn archetype:generate -DgroupId=com.monsite -DartifactId=monprojet -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false

Vous avez ici le `pom.xml` final ainsi que le code de `App.java` final pour que ça fonctionne avec jMonkeyEngine.

Après que le `mvn package` s'est exécuté avec succès, vous devriez pouvoir lancer l'exécution avec :

    java -cp target/monprojet-1.0-SNAPSHOT.jar com.monsite.App

Ou bien :

    java -cp target/classes com.monsite.App

Ou bien en utilisant Maven et le plugin mojo.codehaus : 

    mvn java:exec
