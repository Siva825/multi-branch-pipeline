 pipeline{
    agent{
        label 'java-slave'
    }
    environment{
       git_creds = credentials('Siva825_git_creds')
    }
    stages{
        stage('build'){
            steps{
                echo "displaying credentials"
                echo "git credentials ${git_creds}"
            }
        }
    }
}
