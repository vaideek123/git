pipeline {
    agent any
        stages{
            stage("git"){
                steps{
                     git 'https://github.com/vaideek123/git.git'
                    
                }
            }
             stage("cp"){
                steps{
                     sh 'sudo cp /var/lib/jenkins/workspace/pipe/index.html /var/www/html '
                     sh 'sudo systemct restart httpd'
                }
            }
        }
    }
