pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
		bat 'set MAVEN_HOME=C:\Program Files\Maven\apache-maven-3.9.6'
		bat 'set path=C:\Program Files\Maven\apache-maven-3.9.6\bin:%path%;'
                bat 'mvn compile'
		bat 'mvn package'  
            }
        }
    }
}