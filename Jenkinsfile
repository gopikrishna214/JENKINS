pipeline {
    agent any

    stages {
        stage('Git clone') {
            steps {
                git branch: 'main', credentialsId: 'root', url: 'https://github.com/gopikrishna214/ksapp.git'
            }
            }
        stage('Maven version') {
            steps {
            sh 'mvn --version'
            }
            }
        stage('Maven Clean') {
            steps {
            sh 'mvn clean'
            }
            }			 
        stage('Maven Validate') {
            steps {
            sh 'mvn validate'
            }
            }
        stage('Maven Compile') {
            steps {
            sh 'mvn compile'
            }
            }				
	    stage('Maven package') {
            steps {
            sh 'mvn package'
            }
            }	
		stage('Maven deploy') {
            steps {
            sh 'mvn deploy'	
         
        }
    }
	
