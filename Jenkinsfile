pipeline {
    agent any

    stages {
        stage('Build') {
            agent {
                docker {
                    image 'mcr.microsoft.com/dotnet/sdk:5.0'
                    reuseNode true
                }
            }
            steps {
                dotnet build
            }
        }
    }
}