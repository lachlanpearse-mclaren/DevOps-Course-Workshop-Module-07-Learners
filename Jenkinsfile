pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                agent {
                docker {
                    image 'mcr.microsoft.com/dotnet/sdk'
                }
                dotnet build
            }
        }
    }
}