pipeline {
    agent any
    tools { 
      maven 'MAVEN_HOME' 
      jdk 'JAVA_HOME' 
    }
    stages {
        stage('Build') { 
            steps {
                bat 'C:\\Program Files\\Maven\\apache-maven-3.9.6\\bin\\mvn compile'
		bat 'C:\\Program Files\\Maven\\apache-maven-3.9.6\\bin\\mvn package'  
            }
        }
    }
}