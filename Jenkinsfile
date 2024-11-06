pipeline {
    agent any
    stages{
        stage('Build'){
            steps{
                bat 'npm install'
            script {
                powershell '''
                 Write-Output "Hello, World!"
                 $date = Get-Date
                 Write-Output "Current date and time: $date"
                '''
            }
            script {
                powershell '''c:\\test-script\\myscript.ps1'''
            }
            }
        }
    }
}