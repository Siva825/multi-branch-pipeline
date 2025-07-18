 pipeline{
    agent{
        label 'java-slave'
    }
    environment{
       git-creds =credentials('Siva825_git_creds')
    }
    stages{
        stage('build'){
            steps{
                echo "displaying credentials"
                echo "git credentials ${git-creds}"
            }
        }
    }
}
