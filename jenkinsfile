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
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
