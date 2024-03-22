pipeline{
    agent none
    environment {
        TEST: "this is first env"
        TEST1: "this is second env"
        TEST2: "this is thirst env"
        TEST3: "this is fourth env"
    }   
    stages{
        agent {
        label 'Junkins_slave1'
    }
        stage('Build') {
            steps {
                sh 'sleep 10'
            }

        }
             
        stage('Test') {
            agent {
        label 'junkins_slave2'
    }
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
     