pipeline {
 agent any
  stages {
      stage('Pull') {
         steps {
             git 'https://github.com/vigneshwaran29/jenproj.git'
         }
      }
      stage('Package') {
         steps {
            bat 'mvn package'
         }
      }
      stage('Execute') {
         steps {
            bat 'java -jar "C:/ProgramData/Jenkins/.jenkins/workspace/webproj4/target/webcts-1.0-SNAPSHOT.jar"'
         }
      }
   }
}
