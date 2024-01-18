pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                bat 'mvn compile'
		bat 'mvn package'  
            }
        }
    }
}