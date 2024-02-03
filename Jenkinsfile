pipeline {
    agent { node { label 'agent' } }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'ls -ltr'
                sh 'pwd'
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

    post { 
        always { 
            echo 'I will always run wheather job is success or nots'
        }
         success { 
            echo 'I will always run wheather job is success '
        }
         failure { 
            echo 'I will always run wheather job is fail '
        }
    }
}