pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
         echo 'Building....'          
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
         sh '''#!/bin/bash
                 mvn deploy
         '''
            }
        }
    }
}
