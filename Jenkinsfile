
pipeline{
    agent {
        label 'java-slave'
    }
    triggers{
        githubPush()
    }
    stages{
        stage('build'){
            steps{
                echo 'my name is siva'
            }
        }
    }
}
