pipeline {
    agent any

    stages {
        stage('Compile stage') {
            steps {
                echo 'Compile stage..'
		withMaven(maven : 'apache-maven-3.5.4'){
		  sh 'mvn clean compile'	
		}
            }
        }
        stage('Test Stage') {
            steps {
                echo 'Testing..'
		withMaven(maven : 'apache-maven-3.5.4'){
		  sh 'mvn test'	
		}
            }
        }
        stage('Deploy Stage') {
            steps {
                echo 'Deploying....'
		withMaven(maven : 'apache-maven-3.5.4'){
		  sh 'mvn deployle'	
		}
            }
        }
    }
}