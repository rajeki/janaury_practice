pipeline{
    agent any
    

    stages{
        stage('Build') {
            steps {
                sh 'sleep 5'
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
     