pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repo....'
            }
        }

        stage('Build') {
            steps {
                echo 'dotnet build --configuration Release'
            }
        }

        stage('Test') {
            steps {
                echo 'dotnet test'
            }
        }

        stage('Publish') {
            steps {
                echo 'dotnet publish -c Release -o ./publish'
            }
        }
    }
}
