pipeline {
    agent any
    tools { 
      	maven 'mvn' 
      	jdk 'Java jdk 17.0.10' 
    }
    stages {
        stage('Build') {
            steps {
                bat 'mvn compile'
		bat 'mvn package'
            }
        }
        stage('Test') { 
            steps {
                bat 'mvn test' 
            }
        }
	stage('Deploy') {
	    steps {
		bat 'sudo cp -r target /'
	    }
	}
    }
}
