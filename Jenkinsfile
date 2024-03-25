pipeline{
    agent any
    environment {
        TEST= "this is first env"
        TEST1= "this is second env"
        TEST2= "this is thirst env"
        TEST3= "this is fourth env"
    }   
    stages{
        stage('Parallel Stage'){
        parallel{
                 
        stage('Build') {
                        steps {
                sh 'sleep 10'
            }

        }
             
        stage('Test') {
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
    }
}
     