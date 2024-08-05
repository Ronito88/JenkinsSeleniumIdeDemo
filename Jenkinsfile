pipeline {
    agent any
    
    stages {
        stage('Checkout code') {
            steps {
                // Checkout code from GitHub and specify the branch
                git branch: 'main', url: 'https://github.com/Ronito88/JenkinsSeleniumIdeDemo'
            }
        }
    }
}