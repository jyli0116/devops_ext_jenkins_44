pipeline {
    agent any
    tools { 
      	maven 'mvn' 
      	jdk 'Java jdk 17.0.10' 
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn compile'
		sh 'mvn package'
            }
        }
        stage('Test') { 
            steps {
                sh 'mvn test' 
            }
        }
    }
}
