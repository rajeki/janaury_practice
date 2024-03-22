pipeline{
    agent any
    

    stages{
        stage('Build') {
            steps {
                sh 'sleep 10'
            }

        }
        stage('Build1') {
            steps {
                sh 'sleep 10'
            }

        }
        stage('Build2') {
            steps {
                sh 'sleep 10'
            }

        }
        

        stage('Test') {
            steps {
                sh'''
                #!/bin/bash
                ls -ltr
                sleep 5
                '''
            }

        }
    }
}
     