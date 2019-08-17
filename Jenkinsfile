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
    }
}