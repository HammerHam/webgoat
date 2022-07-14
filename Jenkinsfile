pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                
         sh '''#!/bin/bash
                 mvn deploy
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
