pipeline {
   agent any
   tools {
  maven 'M2_HOME'
}
   triggers {
  pollSCM '* * * * *'
}
    stages {
        stage('maven package') {
            steps {
                echo 'Hello'
                sleep 5
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean'
                sh 'mvn install'
                sh 'mvn package'
                s
            }
        }
        stage('Test') {
            steps {
                sh 'mvn clean'
                
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy '
               
            }
        }
    }
}