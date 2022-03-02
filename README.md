This is saikiran reddy gangidi

**Use the following command to generate a Maven project that contains Beam’s WordCount examples and builds against the most recent Beam release:**

 ``` PS> mvn archetype:generate `
 -D archetypeGroupId=org.apache.beam `
 -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples `
 -D archetypeVersion=2.36.0 `
 -D groupId=org.example `
 -D artifactId=java-word-count-beam `
 -D version="0.1" `
 -D package=org.apache.beam.examples `
 -D interactiveMode=false ```
 
 Create wordcount file and paste the code to run the file by taking input file 
 
 create the sample.txt which is used for input for wordcount file
 
 ** To run the WordCount pipeline, see the Maven and Gradle examples below.**
 
 ```
 $ mvn compile exec:java -Dexec.mainClass=org.apache.beam.examples.WordCount \
     -Dexec.args="--inputFile=sample.txt --output=counts" -Pdirect-runner ```
