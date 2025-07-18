 pipeline{
    agent{
        label 'java-slave'
    }
    environment{
       git_creds = credentials('Siva825_git_creds')
    }
    triggers{
        githubPush()
    }
    stages{
        stage('build'){
            steps{
                echo "displaying credential"
                echo "git credentials ${git_creds}"
            }
        }
    }
}
