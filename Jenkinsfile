pipeline{
    agent any 
     stages {
    stage('Build') {
      steps {
        sh 'chmod +x gradlew'
        sh './gradlew build' // run Gradle build command
      }
    }

    stage('Test') {
      steps {
        sh 'chmod +x gradlew'
        sh './gradlew test' // run Gradle test command
      }
    }

    stage('Sonar') {
      steps {
        withSonarQubeEnv('SonarQube') { // use SonarQube scanner tool
          sh 'chmod +x gradlew'
          sh './gradlew sonarqube' // run Gradle SonarQube scanner command
        }
                      }
                    }
                }
           }
 
           
    