pipeline {
    agent any
    tools {
      	maven 'my_maven'
    }
    stages {
        stage('compile') {
            steps {
                echo 'compile job'
            }
        }

        stage('test') {
            steps {
                echo 'test job'
            }
        }
    
        stage('deploy') {
            steps {
                echo 'deploy job'
            }
        }

        post {
            always {
                junit '**/reports/junit/*.xml'
            }
        }
    }
}
