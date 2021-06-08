pipeline {
    agent any

    stages {
        stage('.NET Build') {
            environment {
                DOTNET_CLI_HOME  = '/tmp/dotnet_cli_home'
            }   
            agent {
                docker {
                    image 'mcr.microsoft.com/dotnet/sdk:5.0'
                }
            }
            steps {
                sh 'dotnet build'
            }
        }
    }
}