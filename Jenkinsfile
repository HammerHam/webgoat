pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                
         sh '''#!/bin/bash
                 mvn package
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
