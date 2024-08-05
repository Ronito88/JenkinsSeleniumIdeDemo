pipeline {
    agent any

    stages {
        stage('Checkout code') {
            steps {
                // Checkout code from GitHub and specify the branch
                git branch: 'main', url: 'https://github.com/Ronito88/JenkinsSeleniumIdeDemo'
            }
        }
          stage('Set up .NET Core') {
            steps {
                bat '''
                echo Installing .NET SDK 6.0
                curl -l -o dotnet-sdk-6.0.132-win-x64.exe https://download.visualstudio.microsoft.com/download/pr/0c82e7e6-fdde-49f2-a69f-bd986aeafe1b/9ea7411a22e661fff0e61e56a466e484/dotnet-sdk-6.0.132-win-x64.exe
                echo installing dotnet-sdk-6.0.132-win-x64.exe   
                dotnet-sdk-6.0.132-win-x64.exe /quiet /norestart
                    '''
            }
        }
    }
}