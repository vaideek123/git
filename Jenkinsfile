pipeline {
    agent any
        stages{
            stage("git"){
                steps{
                     git 'https://github.com/vaideek123/git.git'
                    
                }
            }
            stage("mkdir"){
                steps{
                     sh "sudo mkdir /jk"
                }
            }
             stage("cp"){
                steps{
                     sh 'cp /var/lib/jenkins/workspace/pipe/index.html /var/www/html/'
                     sh 'systemct restart httpd'
                }
            }
        }
    }
