pipeline {
    agent any   
    stages {
        stage('Build') {
            steps {
                sh 'printenv'
                withMaven(mavenSettingsConfig: 'maven-settings-global') {
                    sh 'mvn clean package'
                }
            }
        }     
    }    
}