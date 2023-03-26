pipeline{
    agent any 
     stages {
    stage('Build') {
      steps {
        sh './gradlew build' // run Gradle build command
      }
    }

    stage('Test') {
      steps {
        sh './gradlew test' // run Gradle test command
      }
    }

    stage('Sonar') {
      steps {
        withSonarQubeEnv('SonarQube') { // use SonarQube scanner tool
          sh './gradlew sonarqube' // run Gradle SonarQube scanner command
        }
                      }
                    }
                }
           }
 
           
    