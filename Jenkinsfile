pipeline {
    agent any
        stages{
            stage('git checkout'){
                steps{
                    git branch: 'master',
                    credentialsId: '0f5a239d-86ca-4a61-bad1-a36f80b67ac6',
                    url: 'https://github.com/MahimaRajput/Youtube-clone'
                }
            }
            stage('Npm'){
            when { expression { params.action == 'create'}}    
            steps{
                npmInstall()
            }
        }
    }

}