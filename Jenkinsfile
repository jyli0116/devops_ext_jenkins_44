pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                bat 'C:\\Program Files\\Maven\\apache-maven-3.9.6\\bin\\mvn compile'
		bat 'C:\\Program Files\\Maven\\apache-maven-3.9.6\\bin\\mvn package'  
            }
        }
    }
}