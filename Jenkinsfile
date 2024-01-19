pipeline {
    agent any
    tools { 
      	maven 'mvn' 
      	jdk 'Java jdk 17.0.10' 
    }
    stages {
        stage('Build') {
            steps {
	        git 'https://github.com/jyli0116/devops_ext_jenkins_44.git'
                bat 'mvn compile'
		bat 'mvn package'
            }
        }
        stage('Test') { 
            steps {
                bat 'mvn test' 
            }
        }
        stage('Deploy'){
            steps{
               withCredentials([usernamePassword(credentialsId: 'HerokuID', usernameVariable: 'USER', passwordVariable: 'PASS')]) {
                    bat 'git push https://$USER:$PASS@git.heroku.com/jenkins-simplewebapp.git main' } 
            }
        }
    }
}
