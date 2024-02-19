pipeline{
    agent any
    stages{
        stage('checkout'){
            steps{
                checkout scmGit(branches: [[name: '*/dev']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/srinivas028/taxi-booking.git']])
            }
        }
        stage('Build'){
            steps{
                sh "mvn package"
            }
        }
       
        }
    }
}
