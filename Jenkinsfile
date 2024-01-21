pipeline{
  agent none
    stages{
      stage("build & SonarQube Scanner"){
        agent any
        steps{
        withSonarQubeEny("SonarQube Scanner"){
        sh 'mvn clean package sonar:sonar'
        }
       }
      }
    }
}
