pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repo...'
            }
        }

        stage('Build') {
            steps {
                sh 'dotnet build --configuration Release'
            }
        }

        stage('Test') {
            steps {
                sh 'dotnet test'
            }
        }

        stage('Publish') {
            steps {
                sh 'dotnet publish -c Release -o ./publish'
            }
        }
    }
}
