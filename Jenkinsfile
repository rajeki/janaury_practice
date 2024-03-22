pipeline{
    agent none
    environment {
        TEST= "this is first env"
        TEST1= "this is second env"
        TEST2= "this is thirst env"
        TEST3= "this is fourth env"
    }   
    stages{
                  
        stage('Build') {
            agent{
            label 'jenkins_slave1'
        }
            steps {
                sh 'sleep 10'
            }

        }
             
        stage('Test') {
            agent {
        label 'jenkins_slave2'
    }
            steps {
                sh'''
                #!/bin/bash
                ls -ltr
                echo $TEST  
                echo $TEST4
                sleep 5
                '''
            }

        }
    }
}
     