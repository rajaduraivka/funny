pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
            git credentialsId: '6fc1abe4-f4c7-4338-9085-1c7075dc3a4e', url: 'https://github.com/rajaduraivka/funny.git'
                echo 'Building..'
                
            }
        }
        stage('Test') {
            steps {
                sh 'mvn sonar:sonar \
  -Dsonar.projectKey=devaraj \
  -Dsonar.organization=devraj \
  -Dsonar.host.url=https://sonarcloud.io \
  -Dsonar.login=81e8f98c0e5268714442ffbacba9cd5ae739097b'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
