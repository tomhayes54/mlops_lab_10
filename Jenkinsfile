pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''#!/bin/bash
                echo 'In C or Java, we can compile our program in this step'
                echo 'In Python, we can build our package here or skip this step'
                '''
            }
        }
        stage('Test') {
            steps {
                sh '''#!/bin/bash
                sudo /home/ec2-user/environment/mlops_lab_10/venv/bin/pytest
                
                # TODO fill out the path to conda here
                # sudo /home/ec2-user/environment/mlops_lab_10/venv/bin/activate
                # sudo /PATH/TO/CONDA init

                # TODO Complete the command to run pytest
                # sudo /home/ec2-user/environment/mlops_lab_10/venv/bin/python pytest

                # echo 'pytest not runned'
                # exit 1 #comment this line after implementing Jenkinsfile
                '''

            }
        }
        stage('Deploy') {
            steps {
                echo 'In this step, we deploy our porject'
                echo 'Depending on the context, we may publish the project artifact or upload pickle files'
            }
        }
    }
}
