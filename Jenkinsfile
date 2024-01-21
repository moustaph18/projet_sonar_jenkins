pipeline{
  agent none
    stages{
      stage("build & SonarQube Scanner"){
        agent any
        steps{
        withSonarQubeEny("SonarQube_server"){
        sh 'mvn clean package sonar:sonar'
        }
       }
      }
    }
}
