pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                
         sh '''#!/bin/bash
                 mvn clean package
         '''
                
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
