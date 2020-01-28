pipeline {
    agent any
	tools {maven 'maven'}
    stages {
        stage('Clone') {
            steps {
                git branch: 'master', credentialsId: '90e75e74-dcea-4c4a-b0b2-fce5cc46f46c', url:'https://github.com/sivakcdev/hello-world.git'	
            }
        }
	     stage('Build') {
            steps {
                sh 'mvn clean package'	
            }
        }
