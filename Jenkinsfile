pipeline{
    agent none
    environment {
        TEST= "this is first env"
        TEST1= "this is second env"
        TEST2= "this is thirst env"
        TEST3= "this is fourth env"
    }   
    stages{
                  
                  stage('Checkout') {
                    steps {
                        Checkout([$class: 'GitSCM',
                        branches: [[name: '*/main']],
                        userRemoteConfigs: [[url: 'https://github.com/rajeki/janaury_practice.git', 
                        credentialsId: 'github']]])
                    }
                  }
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
     