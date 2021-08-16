pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven 'Maven-3.8.2'
    }

    stages {
        stage('Build') {
            steps {
                git branch: 'main', credentialsId: 'git', url: 'https://github.com/gopikrishna214/ksapp.git'
            }
            }
        stage('Maven version')
            steps {
            sh 'mvn --version'
            }
            }
        stage('Maven Clean')
            steps {
            sh 'mvn clean'
            }
            }			 
        stage('Maven Validate')
            steps {
            sh 'mvn validate'
            }
            }
        stage('Maven Compile')
            steps {
            sh 'mvn compile'
            }
            }				
	    stage(',Maven package')
            steps {
            sh 'mvn package'
            }
            }	
         
        }
    }
	
