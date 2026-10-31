pipeline{
    agent any
    
    stages{
        stage('Welcome'){
            steps{
                echo 'Welcome to Pipeline'
                sh 'whoami'
                sh 'date'
                sh 'hostname'
            }
        }
        stage('Build'){
            steps{
                echo 'Application Builded'
                sh 'pwd'
                sh 'python --version'
            }
        }
    }
    post{
        success{
            echo 'Pipeline is completed'
        }
        failure{
            echo 'Pipeline Failed'
        }
    }
}
