pipeline {
    agent any

    stages {
        stage('Build') {
            agent {
                docker {
                    image 'mcr.microsoft.com/dotnet/sdk'
                }
            }
            steps {
                dotnet build
            }
        }
    }
}